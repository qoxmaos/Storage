# 📚오픈소스 정리
## 버전관리 개요
**버전관리의 정의**
- 시간 흐름에 따라 파일 집합에 대한 변경 사항을 추적, 관리

**버전관리의 필요성**
- 과거 지점의 버전으로 돌아가 누가, 무엇을 수정했는지 파악 가능

**버전관리 도구의 인터페이스방식**
- CLI와 GUI
- > Working folder, Working tree, Working space

**커밋**
- 저장소의 현 상태를 저장하는 행위이자 깃 명령어

**HEAD**
- 가장 최근의 커밋을 가리키는 포인트

**저장소**
- 파일이나 폴더, 버전관리를 위한 관련 파일을 저장해 두는 곳

## 깃 설정과 저장소 생성
### 지역 저장소 생성 전 다음 설정 반드시 수행!
▶️**사용자 설정**
``` git
$ git config --global user.name "이름"
$ git config --global user.email "메일주소"
```
▶️**맥(IF)과 윈도(CRLF) 간의 자동 변환**
```git
$ git config --global core.autocrlf true
```
▶️**뉴라인 경고 발생 없애기(옵션)**
```git
$ git config --global safecrlf false
```
▶️**기본 편집기 설정**
```git
$ git config --global core.edlitor 'code --wait'
```
▶️**깃 저장소 기본 브랜치 이름 설정**
```git
$ git config --global init.defaultBranch main
```
▶️**깃 저장소 생성**
```git
$ git init (폴더명)
```
> 현재 폴더 하부에 폴더를 생성하고 깃 저장소로 만들기 위해서 사용

## 깃 커믹과 로그
**커밋**
- 버전 관리를 위해 현재 스테이지 영역의 내용에 대해 스냅샷을 찍는 명령
- > 증 커밋으로 버전 고나릴르 위해 인덱스에 추가된 파일들의 현재 상태를 저장
- 커밋에는 이력을 관리하기 위해 반드기 커밋 메세지의 저장이 필요
