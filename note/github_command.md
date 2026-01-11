### 이 문서는 github 명령어 모음입니다
**수정이 있거나, 추가를 원하면 말씀 해 주세요**

# !!! 반드시 git pull / push 시 branch 확인하세요
```
흐름 설명 
1. 로컬 branch를 생성한다 main / develop / feature
2. 로컬 branch에 원격 저장소 내용을 pull로 받는다 ( 3곳 모두 )
3. 로컬 branch에서 작업한다. (주로 feature 또는 develop)
4. 작업한 내용을 원격 저장소에 올린다 (local feature -> feature / local devleop -> develop)
5. 원격 저장소에 모든 내용이 저장이 확인되면, 다시 pull로 개발환경을 맞춘다
    (origin develop -> local develop pull)
6. 개발을 끝내고 version이 완성되면, origin/main 에 push로 원격저장소에 저장한다
    !! 이 6번 과정은 한명만 해도 상관 없습니다. 
    !! 아마 팀장인 제가 하거나, 다른 분께 부탁할 수 있어요
7. 처음 local branch 개발환경과 원격 저장소 branch들의 내용이 다르므로
   2번으로 돌아가서 local branch와 origin branch의 내용을 맞추고 pull한다
    !! 이 과정에서 오류발생할 수 있습니다.
    !! 먼저 코드를 작성하거나, 추가를 했을 경우 데이터가 날아갈 수 있습니다
    !! 따라서 백업폴더를 만들어 별도 관리를 하거나, feature_v1~?? 이런식으로 관리하셔도 좋습니다.
```




참고자료
링크 : https://rogerdudler.github.io/git-guide/index.ko.html

### git push / 관련
```
# 원격 저장소 feature에 내 브란치에서 push
git push origin feature
```

### git branch 관련
```
# branch 확인, 순서대로 로컬, 원격, 전체 
git branch -v , -r, -a

# branch 생성, 생성 후 바로변경

# < test 생성 >
git branch test 

# < test2 생성 후 브란치 변경 >
git checkout -b test2 

#  < branch변경 >
git switch "브란치명"
```

### git remote 관련 
```
# 원격 저장소를 추가
git remote add origin <github.com>

# 원격 저장소


# 아래 두 내용은 프로젝트시 사용 안합니다.
# 프로젝트 원격저장소 (github) 에 연결
git remote add origin https://github.com/checkCJY/confused_project.git

# 원격 저장소 연결 끊기
git remote remove origin (프로젝트 중에는 안씁니다)
``