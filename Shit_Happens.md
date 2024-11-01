# Git & GitHub 게임 답안지

## Shit Happens

### 1. Restore a deleted file

**답: git checkout <파일명> 명령어로 삭제된 파일 복구**

### 2. Restore a file from the past

**답:**
1. git checkout <해시> <파일명> 명령어로 특정 커밋의 특정 파일로 복구
2. 복구한 파일로 새로 커밋하기

### 3. Undo a bad commit

**답:**
1. git reset <해시> 또는 git reset HEAD^ 명령어로 이전 커밋으로 이동
2. 파일 내용을 1~10으로 채우도록 수정
3. git commit -am 'More numbers' 명령어로 커밋
4. 과정 1~3의 목적은 main 브랜치가 기존의 잘못된 커밋을 더 이상 안 가리키도록 하기 위함

### 4. I pushed something broken

**답:**
1. 잘못된 내용을 추가해버린 커밋의 해시로 git revert <해시> 명령어를 사용해서 잘못된 내용을 제외시킨 상태로 새 커밋하기
2. git push 명령어로 team(원격 저장소)의 main 브랜치가 잘못된 내용이 없는 새 커밋을 가리키도록 수정

### 5. Go back to where you were before

**답:**
1. git reflog 명령어를 사용하여 과거에 어떤 브랜치로 git checkout 명령어를 통해 이동했는지 로그 확인
2. git checkout 명령어로 과거에 이동했던 브랜치로 다시 이동