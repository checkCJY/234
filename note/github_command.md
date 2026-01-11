### 이 문서는 github 명령어 모음입니다
**수정이 있거나, 추가를 원하면 말씀 해 주세요**

# !!! 반드시 git pull / push 시 branch 확인하세요

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