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
----
## 다른 환경에서 이어서 작업해야하는 경우
1. 폴더 생성하기(영어로만)> vs code 폴더 연결
2. gitHub 저장소 주소 복사
3. vs code로 돌아와서 ctrl + J 터미널 실행, bash 환경 변경
4. `git clone 저장주소붙여넣기`
5. 터미널 경로 오른쪽에 `main` 또는 `master` 표시가 있는지 확인
6. 위 5번에서 표시가 없다면 `cd 복제한 폴더명` 을 터미널에 입력
7. 자유롭게 수정 후 파일저장
8. 터미널에 `git status` 업로드 안된 파일 빨간색 확인
9. `git add 파일명` 수정한 파일 스테이지에 업로드
10. `git status` 9번 내용 정상 처리 확인(초록색으로 됨)
11. `git commit -m'메세지'` 수정 파일에 대한 기록 메세지 작성
12. `git push origin main` 깃허브 업로드 후 깃허브 새로고침 해서 확인 
----
# html, meta에 작성하는 속성의 뜻
* `<html lang="ko">` 에서 `lang` 은  language(언어)를 뜻하며, `""` 에 원하는 언어를 집어넣을수 있다. 언어를 집어넣는 이유는, 웹접근성중 하나인 화면 낭독 소프트웨어 스크린 리더를 작동시키기 위하여 언어를 집어넣는다.
* `<meta charset="utf-8">` 에서 `charset` 은 속성을 뜻하며, `""` 에 있는 utf-8은 다국어 지원을 하겠다는 내용을 집어넣은것이다.
* `<meta name="keywords" content="">` 에서 `keyword` 는 웹에서 어떠한 단어를 검색하였을때, 그 단어에대한 연관검색어로 사이트가 나오게끔 키워드를 정하게 하는것이며, `""`에 키워드를 집어 넣을수 있다.(""에 들어가는 키워드의 갯수 제한은 없음.)
* `<meta name="description" content="">` 에서 `description` 은 요약, 설명을 의미하며, 웹에서 어떠한 단어를 검색하면, 사이트 밑에 써져있는 설명을 부여할수 있다. 예시로 스타벅스를 검색하면, 스타벅스 라는 사이트 바로 밑에 해당 사이트에 대한 설명이 쓰여있는 것을 확인할수 있다. `""`에 사이트에 대한 설명을 쓸수 있다.