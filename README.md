# pygame_project

* 최종 결과물 -> Play_Game.py


1. **사용언어** : Python

   

2. **pygame 라이브러리** 사용

   

3. **게임을 만들기 위한 설정**

   * 기본 설정

     * 화면 크기 설정
     * 화면 타이틀 설정
     * FPS 설정

   * 사용자 설정

     * 게임 배경화면, 캐릭터, 무기, 장애물 등의 이미지 설정

     * 키보드, 마우스 등의 이벤트 처리

     * 게임 속 캐릭터, 장애물, 무기 등의 위치 정의

     * 충돌 처리

     * 화면에 그리기

     * 폰트 정의 및 시간 정보 설정

       

4. **게임 설명**

   - 캐릭터를 좌우 방향키로 움직이며 스페이스바로 무기 발사

   - 공을 맞출시에 공이 한단계 작은 공 두개로 분리

   - 게임 종료 조건

     - 100초 경과시 실패
     - 캐릭터가 공에 맞으면 실패
     - 무기로 모든 공을 맞춰 없애면 성공

     

5. **exe 실행 파일 생성** -> 파이썬이 설치되지 않은 환경에서도 게임 실행 가능

   * pyinstaller 사용 (pip install pyinstaller)
   * exe 실행 파일 만들기 위해 기본 파일 구조 변경
   * game 폴더 생성하고 코드와 이미지 파일을 같은 폴더에 위치
   * pyinstaller -w --add-data game\*.png;game -F .\game.Play_Game.py 명령어 실행
   * dist 폴더 안에 exe 실행 파일 생성 (파일 용량이 큰 관계로 git에 업로드 X)