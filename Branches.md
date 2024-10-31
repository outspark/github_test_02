# Git & GitHub 게임 답안지

## Branches

### 1. Moving through time

**답:**
1. git checkout 명령어로 브랜치 전환하면서 발생한 상황 확인
2. 마지막 커밋으로 이동해서 문제 해결(문서 수정 - 동전 다시 저금통에 넣기)
3. 해결 후 새로 커밋하기

### 2. Make parallel commits

**답:**
1. git checkout HEAD^ 명령어로 이전에 발생한 사건들 확인
2. 사건이 발생하기 전의 커밋으로 이동
3. 문제 해결(문서 수정 - 아이가 행복한 상태이고, 사자가 무언가를 먹은 상태로 수정)
4. 해결 후 새로 커밋하기

### 3. Creating branches

**답:**
1. git branch 명령어로 2개 브랜치 생성(birthday, concert)
2. git checkout <브랜치명> 명령어 사용해서 브랜치로 이동
3. git reset --hard <해시>를 통해 생성한 브랜치를 각 커밋 상태로 포인터 전환
4. 2~3번째 과정을 반복해서 2개의 브랜치를 각각 어울리는 커밋 상태로 포인터 전환

### 4. Branches grow with you!

**답:**
1. git checkout <해시>로 birthday 브랜치가 있는 마지막 커밋으로 이동
2. 파일 내용을 수정/추가 후 커밋
3. git checkout concert로 concert 브랜치가 가리키는 커밋으로 이동
4. 파일 내용을 수정/추가 후 커밋

### 5. Deleting branches

**답:**
1. git checkout 명령어로 이동하면서 문제가 있는 브랜치 요소(파일)를 확인
2. 해당 브랜치가 가리키는 커밋 내용이 문제 있는 경우, git branch -d 명령어로 브랜치 삭제
3. 1~2의 과정을 반복하여 문제 없는 브랜치 제외한 나머지 브랜치 전부 삭제(leap 브랜치 제외한 나머지 브랜치 제거)

### 6. Moving branches around

**답:**
1. git checkout <브랜치명> 명령어로 이동해서 각 브랜치가 가리키고 있는 커밋 확인
2. 확인 후 각 브랜치를 git reset --hard <해시> 명령어로 어울리는 커밋을 가리키도록 포인터를 수정
3. (1~2의 과정) 'baguette', 'coffee' 브랜치가 가리키는 커밋이 서로 반대가 되었으므로 이 부분을 수정
4. (1~2의 과정) 'donut' 브랜치의 경우 donut 구입한 커밋에서 donut 구입 후 먹은 내용을 추가, 그리고 커밋한 다음 해당 커밋으로 'donut' 브랜치가 가리키도록 수정
