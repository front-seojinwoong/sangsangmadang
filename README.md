# 참고) checkout 명령어가 Git 2.23 버전부터 switch, restore로 분리

## git init
- git init 명령어를 선언하면, git으로 프로젝트로 관리하는 것을 의미한다. (작업의 history는 .git 폴더안에 저장되어 있음)
![non-zero vs even odd](./images/6.png)
- 주의! .git 폴더를 삭제하면 그동안의 형상관리가 다 날라가니 의도적으로 삭제하는 상황 외에는 삭제하지 말것.

## .gitignore : git에서 버전관리를 하지 않을 파일,폴더를 적어놓는 곳
```js   
    # 모든 file.yaml
    file.yaml

    # 최상위 폴더의 file.yaml
    /file.yaml

    # 모든 .yaml 확장자 파일
    *.yaml

    # .yaml 확장자이지만 index.yaml은 무시하지 않을 때
    *.yaml
    !index.yaml

    # logs라는 이름의 파일 또는 폴더와 그 내용들
    logs

    # logs란 이름의 폴더와 그 내용들
    logs/

    # logs 폴더 바로 안의 index.html 과 data.java 파일
    logs/index.html 
    logs/data.java

    # logs 폴더 바로 안, 또는 그 안의 다른 폴더(들) 안의 debug.log
    logs/**/debug.log
```

