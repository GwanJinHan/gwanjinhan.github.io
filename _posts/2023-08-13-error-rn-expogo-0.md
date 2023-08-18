---
title: "[Expo] There was a problem loading the requested app. 에러"
excerpt: ""

category:
  - error

date: 2023-08-13
last_modified_at: 2023-08-13
---

React Native 개발을 위해 Expo를 세팅하다가 막혔다. 
"There was a problem loading the requested app." 이라는 문구와 함께 앱이 실행되지 않았다. <br> <br>
로컬 네트워크 권한도 허용된 상태라서 약간의 구글링을 통해 문제를 해결했다. ([스택 오버플로우 링크](https://stackoverflow.com/questions/56715203/there-was-problem-loading-requested-app-it-looks-like-you-may-be-using-lan-url))
expo-cli는 더 이상 지원되지 않아서, npx 를 활용해 에러를 해결해보자.

![image](/assets/images/error-rn-expogo-0-0.png){: .align-center width="30%"}


1. 커맨드를 열고 프로젝트가 있는 디렉터리로 이동한다. (cd 명령어 사용)

2. 다음 커맨드를 입력한다

    ```bash
    npx expo start --tunnel
    ```

3. @expo/ngrok 패키지를 설치하겠냐는 문구가 나온다. 엔터를 눌러 설치해준다.

    ![image](/assets/images/error-rn-expogo-0-1.png)

4. 정상적으로 실행되는 모습을 볼 수 있다.