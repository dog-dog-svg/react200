# git
  ## clone
* https://github.com/[USERNAME]/[REPOSITORY_NAME].git
  * https://github.com/dog-dog-svg/react200.git
* git clone [REPO_URL] [DIR]
  * git clone https://github.com/dog-dog-svg/react200.git
  ## config 설정
  * git config --global user.name "dog-dog-svg"
  * git config --global user.email "support@webisfree.com"
  * git config --local user.name "dog-dog-svg"
  * git config --local user.email "qwerew369@gmail.com"
  ## config 삭제
  * git config --unset user.name
  * git config --unset user.email
  ## remote등록
  git remote add origin https://github.com/dog-dog-svg/react200.git

  ## branch 이름 변경하기
   git branch -m master main
  ## [GitHub] The requested URL returned error: 403
  git remote set-url origin https://dog-dog-svg@github.com/dog-dog-svg/react200.git

  ## pull
  git pull origin main
  git pull origin main --allow-unrelated-histories
==========================================================================================================================
# yarn 설치

* npm install -g yarn
* npm install -g create-react-app
  * 2번 안되면 시도 **npx create-react-app client**

-----------------------------------------------------------------------------------------------------------------------
### This version of tar is no longer supported, and will not receive security updates. Please upgrade asap. 오류
npm 버전이 낮아서 생김 버전 업그레이드
npm install -g npm

===================================================================================================================

# react 서버실행
* cd client
* yarn start
  * 1번안되면 시도 **npm start**

-------------------------------------------------------------------------------------------------------------------
## 파일준비
### client / src / index.js 수정
* `<React.StrictMode>` 삭제
* **index.js**
    import React from 'react';
    import ReactDOM from 'react-dom';
    import './index.css';
    import App from './App';
    import reportWebVitals from './reportWebVitals';

    ReactDOM.render(  
        <App />,
      document.getElementById('root')
    );

    // If you want to start measuring performance in your app, pass a function
    // to log results (for example: reportWebVitals(console.log))
    // or send to an analytics endpoint. Learn more: https://bit.ly/CRA-vitals
    reportWebVitals();
