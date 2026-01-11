# note 폴더에 프로젝트 진행시 읽고 따라주셔야 합니다

```
project(폴더명)
├── note
│   └── ref_docx
│        ├── "이니셜"_ref.docx.md   #4.1
│   ├── commit_message_rules    #1
│   ├── github_command  #2
│   ├── setting_manual  #3
│   └── reference       #4
├── app.py
└──  requirements.txt   #5

#1 commit_message_rules
- 반드시 읽어주세요
- commit시 해당 문서의 양식대로 작성
- git pull/push 시 branch 확인 후 진행해야 합니다

#2 github_command
- 프로젝트 진행하면서 github 또는 git과 관련된 명령어 모음 문서입니다
- 추가하고 싶은 내용, 또는 알게 된 내용은 작성해주시면 됩니다

#3 setting_manual
- git clone 후 여러분들이 해야하는 기초세팅입니다
- window 운영체제에서 진행했으므로, mac이신분은 추가로 확인하셔야 합니다

#4, #4.1 reference, "이니셜"_ref.docx.md
- 프로젝트를 진행하면서 검색 또는 AI를 통해 얻은 자료 #4.1에 모아둡니다
- 추후 프로젝트 마무리 단계에서 취합후 #4 에 분류별로 작성합니다

#5 requirements.txt
- 제가 가상환경 세팅 후 설치한 pip 들의 version 입니다
- #3 , 또는 아래에서 사용됩니다. 설치 후 확인해보시길 바랍니다
```


# 이 글은 git clone 으로 접속 후, 환경 설정에 관한 내용입니다.


```
- cd ~
- mkdir "폴더명"
- cd "폴더명"
- git clone "주소"

----------------------------------
- 여기까지 진행된 상태입니다.    -
- 아래부터 시작하시면 됩니다.    -
----------------------------------

# uv 실행 전 상태확인
uv --version
uv venv

!!! 가상환경 켜진 상태를 확인
source .venv/bin/activate

git branch -M main
# 원격저장소 설정
git remote add origin https://github.com/checkCJY/confused_project.git

# github 설치환경과 동일하게 pip설치
uv pip install -r requirements.txt
----------------------------------
- 여기까지 설치세팅 끝난 상태.    -
----------------------------------

+ 익스텐션에서 해당 확장자 설치
Commit Message

메세지 입력 칸에 마우스를 가져다 대면 연필모양이 나옵니다
버튼을 누르면 commit 메세지를 길게 작성할 수 있어요
```