# basic command
> Git 기본 문법 정리

## 초기 설정
```bash
git config --global user.email <이메일>
git config --global user.name <이름>
```

## git 저장소 만들기
- `git init`(생성)
    - `.git directory`를 생성해주는 명령어
    - 관리하고 싶은 최상위 위치에서 실행
- `git clone`(복제)
    - ``git clone <원격저장소URL>`
    - 프로젝트 히스토리를 전부 받아온다.
    - 

## 코드 수정하고 저장소에 저장하기

- `git add`
    - `git add <파일/폴더이름>`
    - `working directory`에서 `stagin area`로 추가
    - 일반적으로 모든 파일, 폴더를 추가하기 위해 아래의 코드를 사용
        - `git add .`

- `git commit`
    - `git commit -m "메세지"`
    - `staging area`에 올라간 파일들의 스냅샷을 찍어서 `.git directory`에 저장
    - 옵션
        - `-m` : 메세지를 추가하여 등록
        - `--amend` : 가장 최근의 commit 수정 

## 원격저장소에 업로드하기

- `git remote add <원격저장소이름> <URL>`
    - 원격 저장소 주소를 origin 이라는 이름으로 저장

- `git push <원격저장소이름> <브랜치이름>`
    - 원격저장소에 브랜치를 업로드

## git 상태 체크

- `git status`
    - 현재 git으로 관리되고 있는 파일/폴더의 상태를 출력
    - 옵션
        - `-a` : commit하기 전에 모든 파일이 자동으로 추가된다.
            - ex) git commit -a -m 'update'

## 

## 참고자료

> [공식 사이트](https://git-scm.com/)
>
> [Git Documentation](https://git-scm.com/doc)
>
>[ERROR!](https://github.com/ompangyji/TIL/tree/master/Git/ERROR.md)