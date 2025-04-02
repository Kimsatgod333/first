# HTML
## Hyper Text Markup Language
### HTML은 웹문서의 구조를 담당하는 언어이다.
* HTML에서 구조는 `<>`로 묶인 태그로 작성한다.
* `<시작태그></닫기태그>`
* `<빈태그>`
* 시작과 닫기태그는 한쌍의 요소로 불린다.
### HTML 구조태그
* HTML5 버전 선언하는 `<!doctype html>`
* HTML 웹브라우저 구조 처리하는 태그들
1. `<html></html>`
2. `<head></head>`
3. `<body></body>`
----
# git&gitHub
* 버전관리 프로그램 git
* 버전 파일, 폴더들을 저장하는 장소 gitHub
## git 용어와 뜻
* 작업 디렉터리 : 실제 작업 저장소(윈도우 탐색기 개념)
* 스테이징 : 깃허브에 작업 업로드 전 파일을 대기시키는 대기소
* repository: 대기소(stage)에 파일 대기후 최종 gitHub 업로드 저장소
## 주의사항
* 당일 작업 시작 기준 gitHub 저장소와 로컬저장소와의 파일, 폴더 상태가 같아야한다.
* 동일한 저장소를 관리하는 사람일 경우 작업 컴퓨터가 달라도 gitconfig에 등록된 이름, 이메일이 반드시 동일해야 한다.
----
# 주요 단축키 모음
* `ctrl + /` 한줄 주석
* `Shift + Alt + A` 선택한 영역만 주석 
----
# 처음 git을 이용한 gitHub 저장소 업로드 시 해야하는 순서
1. 현재 사용중인 로컬 저장소를 git 저장소로 등록 `git init`
2. 위 1번을 정상 등록시 경로에 (master) 표시출력
3. master> main으로 최상위 경로명칭 변경위하여 `git branch -m main` 작성
4. gitHub 저장소 생성 후 저장소 주소 복사
5. `git remote origin https://github.com/Kimsatgod333/first.git(<<복사된 주소)`로 현재 로컬 저장소와 gitHub 저장소 연결
6. `git status` 현재 상태 확인(스테이징, 작업디렉터리, 저장소)
7. 위 6번 파일이 빨간색으로 출력될 경우`git add 파일명`으로 스테이지에 올림
8. `git status`로 재확인시 녹색으로 변경된것으로 확인
9. 올릴파일이 전부 녹색으로 변경되었을때 `git commit -m'기록메세지'` 스테이징 파일을 저장소에 올리기 위한 기록 설정.
10. 기록까지 완료 되었을때 git push origin main 으로 gitHub 최종 저장소에 폴더 업로드를 진행.
11. 위 10번 처음 진행시 깃헙 계정 인증 진행 필요. 인증완료 되면 저장소에서 F5 누르면 해당 폴더 내용이 정상적으로 저장된것이 확인.