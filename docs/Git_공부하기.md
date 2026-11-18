## **Git 사용법 공부**

- 인프런에서 강의를 듣거나 웹에서 검색하여 공부를 하신 후, 하단에 있는 내용들을 하실 수 있어야 됩니다.

- 단계별로 하나씩 해보시면 어렵지 않게 하실 수 있습니다.

- **강의를 꼭 듣고나서 하단 내용들을 체크하셔야 이해가 됩니다.**

## **용어 설명**

- [Local] : 흔히 본인이 작업하고 있는 PC 를 로컬이라 부름.

    - 로컬에서 할 일 앞에 붙일 예정

- [GitHub] : git 서비스를 제공하는 대표적인 사이트.

    - GitHub 사이트에서 할 일 앞에 붙일 예정

## **로드맵**

1. 기초적인 사용법 익히기

    - [GitHub] GitHub 에 새로운 git repository 만들기 (GitHub 사이트에서 진행)

    - [Local] 만든 repo 를 내 컴퓨터에 clone 하기

    - [Local] clone 한 폴더에 소스코드 하나 만들기

    - [Local] 터미널이나 git UI 로 git add 하기

    - [Local] git status 명령어로 변경사항 확인하기

    - [Local] git commit 으로 커밋메시지 작성하기

    - [Local] git push 로 git respository 에 커밋하기

    - [Local] git log 로 Local(본인 컴퓨터) 에서 커밋됬는지 확인하기

    - [GitHub] GitHub 사이트에서 수정사항 확인하기

2. 한 단계 더 나아가기

    - [Local] 소스코드 내용 조금 수정하기

    - [Local] git add -> git commit -> git push 로 git repository 에 커밋하기

    - [GitHub] GitHub 사이트에서 commits 버튼 눌러서 변경사항 확인해보기

3. 특정 파일이나 폴더만 커밋하기

    - [Local] 새로운 소스코드 파일 만들기

    - [Local] git add "새로운 소스코드" 로 특정 파일만 추가하기

    - [Local] 이후 커밋

    - [GitHub] GitHub 사이트에서 commit 된 내용 확인하기

4. .gitignore 로 특정파일 혹은 폴더 제외하기

    - [Local] secret.md 파일 만들기

    - [Local] .gitignore 에 secret.md 추가

    - [Local] 기존 소스코드 내용 조금 수정하기

    - [Local] git add --all 로 변경된 모든 파일 내용 추적하기

    - [Local] git status 명령어로 secret.md 추적 안하는것 확인하기

    - [Local] 이후 커밋

5. branch 새로 만들어보기 (새로운 작업공간 만들기)

    - [Local] Local 에서 새로운 branch 명령어로 만들어보기

        - git branch 브랜치명

        - git checkout -b 브랜치명 (브랜치 없으면 생성후 브랜치 이동)

        - git checkout 브랜치명 (해당 브랜치로 이동만함. 없으면 에러뜸)

    - [Local] git branch 명령어로 Local 에 있는 브랜치 목록 및 현재 브랜치 확인해보기

    - [Local] 소스코드중 하나 조금 수정하고 커밋하기

    - [GitHub] GitHub 사이트에서 main 브랜치에서 수정안된것 확인하기

    - [GitHub] GitHub 사이트에서 새로운 브랜치가 생성된것 확인하기

    - [GitHub] 방금 수정한 내용 GitHub 사이트에서 새로운 브랜치의 commit 목록에 있는것 확인하기

6. main 브랜치에 새로만든 브랜치 합치기 (merge)

    - [Local] git checkout main 명령어로 main 브랜치로 이동

    - [Local] 5번에서 수정했던 내용 리셋된거 확인

        - 브랜치를 이동하면 새 브랜치에서 수정했던 내용들이 사라짐

        - 기존 브랜치(main)에 있던 내용으로 돌아옴

    - [Local] git merge 만들었던_브랜치명 명령어로 새로운 브랜치의 수정사항을 main 으로 합치기

    - [Local] 5번에서 수정했던 내용 돌아온것 확인

    - [Local] 커밋하기

        - Local 에서 merge 를 하면 현재 내 컴퓨터에만 합친 내용이 반영됨

        - 이를 GitHub 에 저장하려면 push 를 해줘야됨

7. 타인이 수정한 코드 Local 에 반영하기

    - [GitHub] repo 의 main 브랜치로 이동

    - [GitHub] AddFile -> Create new file 클릭

    - [GitHub] 상단에서 파일이름 TEST.md 로 설정, 텍스트 편집기에 아무 내용 입력

    - [GitHub] 우측 상단에 Commit changes 클릭하여 커밋메시지 작성하고 커밋

        - 이러면 git repo 에 TEST.md 가 기록됨

        - 이걸 Local 로 불러올거임

    - [Local] 폴더에 TEST.md 파일 없는것 확인

        - repo 에만 저장되어있고 Local 로 불러온적 없기때문

    - [Local] git pull origin main 명령어 실행

        - 현재 repo 의 main 브랜치의 내용을 Local 로 불러오는 명령어

        - Local 의 main 브랜치의 현재 커밋과, repo 의 main 브랜치의 commit 을 비교하여 수정된 내용만 바뀜

        - 여기서는 TEST.md 파일이 추가되기만 했으므로 TEST.md 파일만 새로 생성됨

    - [Local] TEST.md 파일이 생성된것 확인


    
