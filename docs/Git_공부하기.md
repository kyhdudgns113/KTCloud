<details>
<summary><h2><strong>📚 Git 사용법 공부</strong></h2></summary>

- 인프런에서 강의를 듣거나 웹에서 검색하여 공부를 하신 후, 하단에 있는 내용들을 하실 수 있어야 됩니다.

- 단계별로 하나씩 해보시면 어렵지 않게 하실 수 있습니다.

- **강의를 꼭 듣고나서 하단 내용들을 체크하셔야 이해가 됩니다.**

</details>

<details>
<summary><h2><strong>🏷️ 용어 설명</strong></h2></summary>

- 💻 [Local] : 흔히 본인이 작업하고 있는 PC 를 로컬이라 부름.

    - 💻 가 붙어 있으면 내 컴퓨터에서 하는 일입니다.

- 🐙 [GitHub] : git 서비스를 제공하는 대표적인 사이트.

    - 🐙 가 붙어 있으면 GitHub 사이트에서 하는 일입니다.

</details>

<details>
<summary><h2><strong>🗺️ 로드맵</strong></h2></summary>

<details>
<summary><strong>1. 기초적인 사용법 익히기</strong></summary>

- 🐙 [GitHub] GitHub 에 새로운 git repository 만들기 (GitHub 사이트에서 진행)

- 💻 [Local] 만든 repo 를 내 컴퓨터에 clone 하기

- 💻 [Local] clone 한 폴더에 hello.md 만들기

- 💻 [Local] 터미널이나 git UI 로 git add 하기

- 💻 [Local] git status 명령어로 변경사항 확인하기

- 💻 [Local] git commit 으로 커밋메시지 작성하기

- 💻 [Local] git push 로 git respository 에 커밋하기

- 💻 [Local] git log 로 Local(본인 컴퓨터) 에서 커밋됬는지 확인하기

- 🐙 [GitHub] GitHub 사이트에서 수정사항 확인하기

</details>

<details>
<summary><strong>2. 한 단계 더 나아가기</strong></summary>

- 💻 [Local] hello.md 내용 조금 수정하기

- 💻 [Local] git add -> git commit -> git push 로 git repository 에 커밋하기

- 🐙 [GitHub] GitHub 사이트에서 commits 버튼 눌러서 변경사항 확인해보기

</details>

<details>
<summary><strong>3. 특정 파일이나 폴더만 커밋하기</strong></summary>

- 💻 [Local] second.md 파일 만들기

- 💻 [Local] git add second.md 로 이 파일만 추가하기

- 💻 [Local] 이후 커밋

- 🐙 [GitHub] GitHub 사이트에서 commit 된 내용 확인하기

</details>

<details>
<summary><strong>4. .gitignore 로 특정파일 혹은 폴더 제외하기</strong></summary>

- 💻 [Local] secret.md 파일 만들기

- 💻 [Local] .gitignore 에 secret.md 추가

- 💻 [Local] hello.md 내용 조금 수정하기

- 💻 [Local] git add --all 로 변경된 모든 파일 내용 추적하기

- 💻 [Local] git status 명령어로 secret.md 추적 안하는것 확인하기

- 💻 [Local] 이후 커밋

</details>

<details>
<summary><strong>5. branch 새로 만들어보기 (새로운 작업공간 만들기)</strong></summary>

- 💻 [Local] Local 에서 새로운 branch 명령어로 만들어보기

    - git branch practice-branch

    - git checkout -b practice-branch (브랜치 없으면 생성후 브랜치 이동)

    - git checkout practice-branch (해당 브랜치로 이동만함. 없으면 에러뜸)

- 💻 [Local] git branch 명령어로 Local 에 있는 브랜치 목록 및 현재 브랜치 확인해보기

- 💻 [Local] practice-branch 에서 hello.md 를 조금 수정하고 커밋

- 💻 [Local] git push -u origin practice-branch

- 🐙 [GitHub] GitHub 사이트에서 main 브랜치에서 수정안된것 확인하기

- 🐙 [GitHub] GitHub 사이트에서 practice-branch 브랜치가 생성된것 확인하기

- 🐙 [GitHub] 방금 수정한 내용이 practice-branch 의 commit 목록에 있는지 확인하기

</details>

<details>
<summary><strong>6. main 브랜치에 새로만든 브랜치 합치기 (merge)</strong></summary>

- 💻 [Local] git checkout main 명령어로 main 브랜치로 이동

- 💻 [Local] 5번에서 수정했던 내용 리셋된거 확인

    - 브랜치를 이동하면 새 브랜치에서 수정했던 내용들이 사라짐

    - 기존 브랜치(main)에 있던 내용으로 돌아옴

- 💻 [Local] git merge practice-branch 명령어로 practice-branch 의 수정사항을 main 으로 합치기

- 💻 [Local] 5번에서 수정했던 내용 돌아온것 확인

- 💻 [Local] 커밋하기

    - Local 에서 merge 를 하면 현재 내 컴퓨터에만 합친 내용이 반영됨

    - 이를 GitHub 에 저장하려면 push 를 해줘야됨

</details>

<details>
<summary><strong>7. 타인이 수정한 코드 Local 에 반영하기</strong></summary>

- 🐙 [GitHub] repo 의 main 브랜치로 이동

- 🐙 [GitHub] AddFile -> Create new file 클릭

- 🐙 [GitHub] 상단에서 파일이름 TEST.md 로 설정, 텍스트 편집기에 아무 내용 입력

- 🐙 [GitHub] 우측 상단에 Commit changes 클릭하여 커밋메시지 작성하고 커밋

    - 이러면 git repo 에 TEST.md 가 기록됨

    - 이걸 Local 로 불러올거임

- 💻 [Local] 폴더에 TEST.md 파일 없는것 확인

    - repo 에만 저장되어있고 Local 로 불러온적 없기때문

- 💻 [Local] git pull origin main 명령어 실행

    - 현재 repo 의 main 브랜치의 내용을 Local 로 불러오는 명령어

    - Local 의 main 브랜치의 현재 커밋과, repo 의 main 브랜치의 commit 을 비교하여 수정된 내용만 바뀜

    - 여기서는 TEST.md 파일이 추가되기만 했으므로 TEST.md 파일만 새로 생성됨

- 💻 [Local] TEST.md 파일이 생성된것 확인

</details>

<details>
<summary><strong>8. 같은 줄을 서로 다르게 고쳐서 충돌 해결해보기</strong></summary>

- 💻 [Local] 시작 전에 `git status` 실행

    - 수정 중인 파일이 없어야 합니다. 남아 있으면 커밋하거나 되돌려 두고 진행합니다.

- 💻 [Local] `note.md` 파일을 만들고 내용은 한 줄만 적기

    - `색상: 파랑`

- 💻 [Local] `git add note.md` 후 커밋하고 `git push`

- 🐙 [GitHub] main 에서 `note.md` 를 열어 `색상: 파랑` 인지 확인

    - 여기서부터 로컬과 GitHub 가 같은 내용입니다. 이 공통 지점이 있어야 충돌을 만들 수 있습니다.

- 💻 [Local] `note.md` 를 `색상: 빨강` 으로 수정

- 💻 [Local] `git add note.md` 후 커밋

    - 이 커밋은 push 하지 않습니다. 내 컴퓨터에만 있게 둡니다.

- 🐙 [GitHub] main 의 `note.md` 에서 연필 아이콘(Edit) 클릭

- 🐙 [GitHub] 같은 줄을 `색상: 초록` 으로 바꾸고 Commit changes

    - 같은 줄을 빨강(로컬)과 초록(GitHub)으로 갈라 놓은 상태입니다.

- 💻 [Local] `git pull origin main` 실행

    - `CONFLICT` 라는 문구가 나오면 실습이 된 것입니다.

    - 자동으로 합쳐지면, 빨강 커밋을 이미 push 했거나 GitHub 에서 다른 줄을 고친 경우입니다. 같은 줄인지 다시 확인합니다.

- 💻 [Local] `git status` 로 `note.md` 가 충돌 상태인지 확인

    - both modified, Unmerged paths 같은 표시가 보입니다.

- 💻 [Local] `note.md` 를 열어 충돌 표시 읽기

    - 파일 안에는 아래처럼 적혀 있습니다.

    - `<<<<<<< HEAD` 부터 `=======` 앞까지가 내 컴퓨터 커밋(빨강)입니다.

    - `=======` 부터 `>>>>>>>` 앞까지가 GitHub 커밋(초록)입니다.

    - `<<<<<<<`, `=======`, `>>>>>>>` 줄은 Git 이 넣어 준 표식입니다. 내용이 아닙니다.

- 💻 [Local] 표식 세 종류를 모두 지우고, 남길 문장만 적기

    - 한쪽만 골라도 되고, 두 내용을 섞어도 됩니다.

    - 예: `색상: 빨강`

    - 표식을 지우지 않으면 그 기호가 그대로 코드에 남습니다.

- 💻 [Local] `git add note.md`

- 💻 [Local] `git status` 로 충돌 표시가 빠졌는지 확인

- 💻 [Local] `git commit` 으로 합치기 마무리

    - 이 커밋은 새 기능이 아니라, 충돌을 해결했다는 기록입니다.

- 💻 [Local] `git push`

- 🐙 [GitHub] `note.md` 가 내가 남긴 문장인지 확인

- 해결이 막히면 💻 [Local] `git merge --abort`

    - 이번 `git pull` 이 시작했던 합치기를 취소하고, 충돌 나기 전 커밋으로 돌아갑니다.

    - 내 빨강 커밋과 GitHub 의 초록 커밋은 그대로 있습니다. 파일만 다시 정리하면 됩니다.

</details>

<details>
<summary><strong>9. 커밋 되돌리기</strong></summary>

- 아직 push 하지 않은 커밋은 `git reset` 으로 커밋 자체만 취소할 수 있습니다.

- 이미 push 한 커밋은 `git revert` 로 되돌립니다. 기존 커밋은 기록에 남고, 그 변경을 취소하는 커밋이 새로 추가됩니다.

- push 한 커밋을 `reset` 으로 지우면 GitHub 의 기록과 내 컴퓨터의 기록이 어긋납니다. 올린 커밋은 revert 로 되돌립니다.

- 💻 [Local] main 브랜치에서 `undo.md` 를 만들고 한 줄만 적기

    - `되돌리기 실습`

- 💻 [Local] `git add undo.md` 후 커밋

    - 이 커밋은 push 하지 않습니다.

- 💻 [Local] `git log -1 --oneline` 으로 방금 커밋이 맨 위에 있는지 확인

- 💻 [Local] `git reset --soft HEAD~1`

    - `HEAD~1` 은 현재 커밋의 한 단계 전입니다.

    - `--soft` 는 맨 위 커밋만 취소하고, 파일 내용은 스테이징에 남겨 둡니다.

    - `--hard` 는 파일 수정까지 지웁니다. 이번 실습은 `--soft` 만 사용합니다.

- 💻 [Local] `git log -1 --oneline` 으로 방금 커밋이 없어졌는지 확인

- 💻 [Local] `git status` 로 `undo.md` 가 아직 남아 있는지 확인

- 💻 [Local] 같은 내용으로 다시 커밋하고 `git push`

- 🐙 [GitHub] main 에 `undo.md` 가 생겼는지 확인

- 💻 [Local] `git revert HEAD --no-edit`

    - 방금 push 한 커밋의 변경을 취소하는 커밋을 만듭니다.

    - `--no-edit` 는 기본 메시지로 그 커밋을 완료합니다.

- 💻 [Local] `undo.md` 가 없어졌는지 확인

- 💻 [Local] `git log -2 --oneline` 으로 되돌리는 커밋이 위에 추가됐는지 확인

    - 이전에 push 한 커밋도 기록에는 남아 있습니다.

- 💻 [Local] `git push`

- 🐙 [GitHub] main 에서 `undo.md` 가 사라졌는지 확인

</details>

<details>
<summary><strong>10. Pull Request 로 합치기</strong></summary>

- 6번은 내 컴퓨터에서 `git merge` 로 합치는 연습입니다.

- 팀 작업은 브랜치를 GitHub 에 올린 뒤 Pull Request 를 만들고, 변경 내용을 확인한 다음 main 에 합칩니다.

- 💻 [Local] `git checkout main`

- 💻 [Local] `git pull origin main`

- 💻 [Local] `git checkout -b practice-pr`

- 💻 [Local] `pr.md` 를 만들고 한 줄 적기

    - `PR 실습`

- 💻 [Local] `git add pr.md` 후 커밋

- 💻 [Local] `git push -u origin practice-pr`

    - 새 브랜치를 처음 올릴 때는 `-u` 로 이 브랜치와 GitHub 브랜치를 연결합니다.

- 🐙 [GitHub] 저장소 페이지 위쪽에 Compare & pull request 가 보이면 클릭

    - 버튼이 없으면 Pull requests 탭에서 New pull request 를 누릅니다.

- 🐙 [GitHub] base 는 main, compare 는 practice-pr 인지 확인

- 🐙 [GitHub] 제목에 무엇을 고쳤는지 적고 Create pull request

- 🐙 [GitHub] Files changed 탭에서 내가 고친 내용만 있는지 확인

- 🐙 [GitHub] Merge pull request 를 누르고 Confirm merge

    - 연습 저장소라서 본인이 바로 합칩니다. 팀 저장소에서는 리뷰가 끝난 뒤에 합칩니다.

- 💻 [Local] `git checkout main`

- 💻 [Local] `git pull origin main`

- 💻 [Local] practice-pr 에서 고친 내용이 main 에 반영됐는지 확인

- 💻 [Local] `git branch -d practice-pr` 로 로컬 브랜치 삭제

- 🐙 [GitHub] Delete branch 가 보이면 눌러서 GitHub 의 브랜치도 삭제

</details>

</details>
