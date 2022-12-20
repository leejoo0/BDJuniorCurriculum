# Quest 00. 형상관리 시스템

## Introduction

* git은 개발 생태계에서 가장 각광받고 있는 버전 관리 시스템입니다. 이번 퀘스트를 통해 git의 기초적인 사용법을 알아볼 예정입니다.

## Topics

* git
  * `git clone`, `git add`, `git commit`, `git push`, `git pull`, `git branch`, `git stash` 명령
  * `.git` 폴더
* GitHub

## Resources

* [Resources to learn Git](https://try.github.io)
* [Learn Git Branching](https://learngitbranching.js.org/?locale=ko)
* [Inside Git: .Git directory](https://githowto.com/git_internals_git_directory)

## Checklist

* 형상관리 시스템은 왜 나오게 되었을까요?
  	* 수많은 개발자가 프로젝트를 가지고 협업을 진행. 초반에는 압축 파일을 가지고 합치며 협업했다. 수정충돌 등으로 소스코드를 관리하기 위함.
* git은 어떤 형상관리 시스템이고 어떤 특징을 가지고 있을까요? 분산형 형상관리 시스템이란 무엇일까요?
  	*  git은 분산 버전 관리 시스템으로 GPL 라이센스를 가지고 있음. 
  	* 소스코드 저장소를 사용자가 각자 저장하고 있음. 로컬과 원격 모두 히스토리를 가지고 있다.  
* git은 어떻게 개발되게 되었을까요? git이 분산형 시스템을 채택한 이유는 무엇일까요?
  	* bitkeeper 상용프로그램을 사용하다 유료화 진행으로 bitkeeper의 기술 바탕으로 부족한점을 보완하고 기능 업그레이드 해서 만든 버전관리시스템 
  	* 소스코드 저장소를 각자 컴퓨터에 저장 가능
  	* 변경사항을 공유 가능
  	* 버전 관리가 가능 
* git과 GitHub은 어떻게 다를까요?
  	* Git은 소프트웨어 개발 프로젝트에서 소스 코드를 관리하기 위해 사용되는 형상관리 시스템이고, GitHub는 웹 기반의 소스 코드 관리 시스템 
* git의 clone/add/commit/push/pull/branch/stash 명령은 무엇이며 어떨 때 이용하나요? 그리고 어떻게 사용하나요? 
  	* 실습 
* git의 Object, Commit, Head, Branch, Tag는 어떤 개념일까요? git 시스템은 프로젝트의 히스토리를 어떻게 저장할까요?
  	* Object: Git은 소스 코드를 저장할 때 이를 개별 객체(Object)로 저장
	* Commit: 소스 코드의 변경 사항을 저장하기 위해서는 커밋
  	* Head: Head는 소스 코드 저장소의 현재 상태를 가리키는 포인터
  	* Branch: Branch는 소스 코드 저장소의 상태를 저장하고 관리하기 위해 사용
  	* Tag: Tag는 소스 코드 저장소의 특정 상태를 저장하고 관리하기 위해 사용

* 리모트 git 저장소에 원하지 않는 파일이 올라갔을 때 이를 되돌리려면 어떻게 해야 할까요?
  	* `git reset --hard HEAD~2` `git push -f origin master`
  	* `git revert`


## Quest

* GitHub에 가입한 뒤, [이 커리큘럼의 GitHub 저장소](https://github.com/BD-AP2/BDJuniorCurriculum)의 우상단의 Fork 버튼을 눌러 자신의 저장소에 복사해 둡니다.
* Windows의 경우 같이 설치된 git shell을, macOS의 경우 터미널을 실행시켜 커맨드라인에 들어간 뒤, 명령어를 이용하여 복사한 저장소를 clone합니다.
  * 앞으로의 git 작업은 되도록 커맨드라인을 통해 하는 것을 권장합니다.
* 이 문서가 있는 폴더 바로 밑에 있는 sandbox 폴더에 파일을 추가한 후 커밋해 보기도 하고, 파일을 삭제해 보기도 하고, 수정해 보기도 하면서 각각의 단계에서 커밋했을 때 어떤 것들이 저장되는지를 확인합니다.
* `clone`/`add`/`commit`/`push`/`pull`/`branch`/`stash` 명령을 충분히 익혔다고 생각되면, 자신의 저장소에 이력을 push합니다.

## Advanced

* Mercurial은 어떤 형상관리 시스템일까요? 어떤 장점이 있을까요?
	* 머큐리얼(Mercurial)은 소프트웨어 개발을 위한 크로스-플랫폼 분산 버전 관리 도구이다. 대부분은 파이썬을 사용하여 개발되었다.
	* 빠르고 사용하기 쉬우며 깨끗하고 직관적인 명령줄 인터페이스를 가지고 있다.
* 실리콘밸리의 테크 대기업들은 어떤 형상관리 시스템을 쓰고 있을까요?
	* AWS CodeCommit은 클라우드에서 자산(예: 문서, 소스 코드, 바이너리 파일)을 비공개로 저장하여 관리할 수 있도록 Amazon Web Services에서 호스팅되는 버전 관리 서비스
