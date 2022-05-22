## githubBranchConflict
- github 사용시, branch에 유의하라고 한다.
- 왜 유의해야하는지에 대해 알아보고자 이 리포지토리를 만들게 됨.

### 과정 설명
리포지토리 collaborator들 간에 순서를 정하여 일부로 **충돌**을 일으킬 것임.
1. `chapdo` 리포지토리 개설
2. `and` test 파일 main branch에 업로드 
```
1
2
3
4
```
3. `chapdo `와 `and` 각자 branch 생성
4. `and` branch에서 test 파일 수정
```
1
2
3
4
4 + 4
```
5. `chapdo` branch에서 test 파일 수정
```
1
2
3
4
4 - 4
```
6. `and`가 먼저 pull requests를 진행
7. 다음으로 `chapdo`가 pull requests 진행. 하지만    
This branch has conflicts that must be resolved
Use the web editor or the  to resolve conflicts.
Conflicting files
test
알림과 함께  충돌이 일어남

### 논의 사항
- main branch에는 과정2 상태로 test가 남아있지만, 각자의 branch에서 수정이 일어나면서 충돌이 발생함.
- 따라서 앞으로 리포지토리에 pull requests를 할 경우 branch 설정에 유의해야 함.