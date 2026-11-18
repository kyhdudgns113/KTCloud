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

    - [Local] 소스코드중 하나 조금 수정하고 커밋, 푸쉬하기

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

8. 같은 줄을 서로 다르게 고쳐서 충돌 해결해보기

    - 충돌은 같은 파일의 같은 부분을, 서로 다른 커밋에서 둘 다 고쳤을 때 납니다.

    - 다른 파일을 고치거나, 같은 파일의 다른 줄을 고치면 보통 `git pull` 이 알아서 합칩니다.

    - 아래는 팀원이 GitHub 에서 고친 척하고, 내 컴퓨터에서도 같은 줄을 고친 뒤 받아보는 실습입니다.

    - [Local] 시작 전에 `git status` 실행

        - 수정 중인 파일이 없어야 합니다. 남아 있으면 커밋하거나 되돌려 두고 진행합니다.

    - [Local] `note.md` 파일을 만들고 내용은 한 줄만 적기

        - `색상: 파랑`

    - [Local] `git add note.md` 후 커밋하고 `git push`

    - [GitHub] main 에서 `note.md` 를 열어 `색상: 파랑` 인지 확인

        - 여기서부터 로컬과 GitHub 가 같은 내용입니다. 이 공통 지점이 있어야 충돌을 만들 수 있습니다.

    - [Local] `note.md` 를 `색상: 빨강` 으로 수정

    - [Local] `git add note.md` 후 커밋

        - 이 커밋은 push 하지 않습니다. 내 컴퓨터에만 있게 둡니다.

    - [GitHub] main 의 `note.md` 에서 연필 아이콘(Edit) 클릭

    - [GitHub] 같은 줄을 `색상: 초록` 으로 바꾸고 Commit changes

        - 같은 줄을 빨강(로컬)과 초록(GitHub)으로 갈라 놓은 상태입니다.

    - [Local] `git pull origin main` 실행

        - `CONFLICT` 라는 문구가 나오면 실습이 된 것입니다.

        - 자동으로 합쳐지면, 빨강 커밋을 이미 push 했거나 GitHub 에서 다른 줄을 고친 경우입니다. 같은 줄인지 다시 확인합니다.

    - [Local] `git status` 로 `note.md` 가 충돌 상태인지 확인

        - both modified, Unmerged paths 같은 표시가 보입니다.

    - [Local] `note.md` 를 열어 충돌 표시 읽기

        - 파일 안에는 아래처럼 적혀 있습니다.

        - `<<<<<<< HEAD` 부터 `=======` 앞까지가 내 컴퓨터 커밋(빨강)입니다.

        - `=======` 부터 `>>>>>>>` 앞까지가 GitHub 커밋(초록)입니다.

        - `<<<<<<<`, `=======`, `>>>>>>>` 줄은 Git 이 넣어 준 표식입니다. 내용이 아닙니다.

    - [Local] 표식 세 종류를 모두 지우고, 남길 문장만 적기

        - 한쪽만 골라도 되고, 두 내용을 섞어도 됩니다.

        - 예: `색상: 빨강`

        - 표식을 지우지 않으면 그 기호가 그대로 코드에 남습니다.

    - [Local] `git add note.md`

    - [Local] `git status` 로 충돌 표시가 빠졌는지 확인

    - [Local] `git commit` 으로 합치기 마무리

        - 이 커밋은 새 기능이 아니라, 충돌을 해결했다는 기록입니다.

    - [Local] `git push`

    - [GitHub] `note.md` 가 내가 남긴 문장인지 확인

    - 해결이 막히면 [Local] `git merge --abort`

        - 이번 `git pull` 이 시작했던 합치기를 취소하고, 충돌 나기 전 커밋으로 돌아갑니다.

        - 내 빨강 커밋과 GitHub 의 초록 커밋은 그대로 있습니다. 파일만 다시 정리하면 됩니다.

