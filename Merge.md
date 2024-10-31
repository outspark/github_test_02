# Git & GitHub 게임 답안지

## Merge

### 1. Merging timelines

**답:**
```
git checkout 28c9f8dc4542c5ba75dfc4f6eabc1ed395503849 (You buy a baguette)
git merge ec0fcdcff46c181f8d990f0d46a48ecf2d30b523 (You buy a donut)
git merge 70e6ba8e04ed9f15999ecbec821b54921b16642a (You drink a coffe)
git merge f47523e7566e77b423ecc197a6a3f74c17cc3183 (You eat the baguette)
git merge c42a74b5cad1b96556c6d304f0984a0df4839a19 (You eat the donut)
``` 

### 2. Contradictions
    ```
    git merge bf9ffcc0a3c090947712efc13809aad355899b90
    git merge 81db091310eefbd7319259d9157fae41a8f53a37
    충돌 발생(내용 수정 후)
    git add sam
    git commit -m "merged"
    ```
**답:**