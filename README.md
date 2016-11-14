# 사용하는 방법

## 실행 

이것은 원본의 `myFridge` 앱을 Meteor Version 1.4.2.1로 수정해 본 것이다. 


이 깃저장소를 클론닝 한 이후에 다음과 같이 시행한다. `jQuery UI`는 Atmosphere의 `linto:jquery-ui` 패키지를 사용하였다.

    $ git clone https://github.com/koseokbum/chap2_kr_myFridge.git
    $ meteor npm install
    $ meteor add linto:jquery-ui
    $ meteor run

## 바꾼 부분

책의 앞 부분에 있는 저자 부록 부분에서 설명한 미티어 공식 사이트의 `simple-todos` 앱과 같이 `imports` 등의 디렉터리를 만들어 다시 정리했다. 주로 바뀐 부분은 다음과 같다. 

- `if(Meteor.isClient){...}` 부분을 `client` 디렉터리로, `if (Meteor.isServer) {...}` 부분은 `server` 디렉터리로 보낸다. 

- 컬렉션을 `imports/api/projects.js` 파일에 만들고 이것을 클라언트와 서버에서 임포트한다. 

- 드래그 앤 드롭을 구현하기 위해서 `jQuery UI`를 사용했는데, 이것은 Atmosphere의 `linto:jquery-ui` 패키지를 사용하였다.

