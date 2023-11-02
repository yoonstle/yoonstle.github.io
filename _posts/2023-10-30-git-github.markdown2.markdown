---
layout: post
title:  "git과 git hub를 다루는 방법 -김은지"
date:   2023-10-30 21:42:00 
categories: vs-code markdown
---
어떤 Markdown 에디터를 사용해도 되고 텍스트 파일을 생성하는 어떤 편집틀이라도 마크다운 파일을 만들수 있지만 vs code로 작성하는 방법을 알아본다

<!--주석으로 사용함 -->
### git 
분산 버전 관리 시스템(DVCS)으로 소스 코드의 비전을 관리하는 툴이다. 
- 분산형 시스템, 비선형적 개발, 삐른 성능, 데이터 무결성, 작업 병합 


### github
git을 기반으로 한 웹 기반의 호스팅 서비스이다. 
소프트웨어 개발 프로젝트를 위한 소스 코드 관리 서비스이다. 


### github를 다루기 위한 사전 지식 
*커밋(commit) : 파일을 추가하거나 변경 내용을 저장소에 저장하는 작업
*푸시(push) : 파일을 추가하거나 변경 내용을 원격 저장소에 업로드하는 작업 
*저장소 : 파일이나 디렉토리를 저장하는 장소(로컬저장소 : 내 컴퓨터에 저장, 원격저장소 : 네트워크상에 저장)


### github 다루는 방법
기본적인 git의 작업은 아래와 같은 흐름이된다. 
1. github에 저장소 작성 (git init) 또는 복제 (git clone)
2. 파일의 작성, 편집
3. 파일의 생성/변경/삭제를 git 인덱스에 추가 (git add)
4. 변경 결과를 로컬 저장소에 커밋 (git commit)
5. 로컬 저장소를 푸쉬해 원격 저장소에 반영 (git push)


##  1.github에 저장소 작성 
- github 메인화면에서 Create New Repository을 누른다.
- Repository name에 이름을 입력하고 Description에 저장소 설명을 입력한다.
- 저장소 유형에는 Public을 선택한다. 
- gitignore이나 license에 대해서는 나중에 추가하거나 변경할 수 있으므로 None을 선택한다. 
- 필요 항목의 입력을 마친 후 Create repository을 누르면 저장소 생성이 완료된다. 
 

## 2. 파일의 작성, 편집 
- PC에 로컬 저장소를 만든다.
- (예시) 'helloworld'라는 디렉토리를 만든다. 
  mkdir helloworld 
  cd helloworld
  git init 
   *mkdir : 새로운 디렉토리를 만드는 명령
    cd : 디렉토리를 이동하는 명령
    get init : git 저장소를 새로 만드는 명령 (이 명령을 실행하면 현재 디렉토리를 git 저장소로 변환한다.)


## 3. 파일의 생성/변경/삭제 git 인덱스에 추가 (git add)
- (예시) hello.html 파일을 로컬 저장소에 추가한다.
- 아래의 명령으로 인덱스(임시로 저장할 위치)에 추가한다. 
   git add hello.html


- (예시) hello.html 파일을 로컬 저장소에 추가한다.
- 아래의 명령으로 인덱스(임시로 저장할 위치)에 추가한다. 
   git add hello.html

## 4. 변경 결과를 로컬 저장소에 커밋 (git commit)
- 아래의 명령으로 인덱스에 추가된 파일을 커밋한다. 
- 커밋은 파일이나 디렉토리의 추가 또는 변경을 저장소에 기록하는 작업이다. 
  git commit -m "new file"
- 이제 파일이 추가되어 있는지 확인한다. 
  git status 
-원격 저장소에 반영하기 전에 원격 저장소의 정보를 추가한다. 
  git remote add origin https://github.com/username/repositaryName


## 5. 로컬 저장소를 푸쉬해 원격 저장소에 반영 (git push) 
- 로컬 저장소의 변경 사항을 github에 있는 원격 저장소에 반영하기 위해 아래의 명령을 실행한다. 
 git push origin master 
- github의 사용자 이름과 암호를 입력하면 github에 푸쉬하고 원격 저장소에 반영할 수 있다. 
- 작업이 끝났다면 github.com페이지로 가서 파일이 잘 푸쉬가 됐는지 확인한다. 

##### 추가 조사 
원래 만들려고 했던 OCR을 만들려고 했던 목적은 이렇다. 
***시각장애인을 위한 텍스트 음성 변환***
***OCR로 의료 라벨 전사*** 
약물의 중복 투약 등을 예방하기 위해 의료 데이터가 캡쳐된다.
간호사들의 실수를 줄이는데 도움이 된다. (실제로 세브란스 병원에서 사용중이기도 하다)

[git-hub-repo]: https://jekyllrb.com/docs/home
