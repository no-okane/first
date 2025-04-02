# HTML
## Hyper Test Markup Language
### HTML은 웹문서의 구조를 담당하는 언어
* HTML에서 구조는 `<>` 로 묶인 태그로 작성
* `<시작태그></닫기태그>`
* `<빈태그>`
* 시작과 닫기 태그는 한 쌍의 요소
### HTML 구조 태그
* HTML5 버전 선언하는 `<!doctype html>`
* 이하 HTML 웹 브라우저 구조 처리 태그
1. `<html></html>`
2. `<head></head>`
3. `<body></body>`
----
# git&gitHub
* 버전 관리 프로그램 git
* 버전 파일, 폴더 저장 저장소 gitHub
## git 용어와 뜻
* 작업 디렉터리 : 실제 작업 저장소 (윈도우 탐색기 개념)
* 스테이징 : 깃허브에 작업 업로드 전 파일 대기, 대기소
* repository : 대기소 (stage)에 파일 대기 후 최종 gitHub 업로드 저장소
## 주의사항
* 당일 작업 시작 기준 gitHub 저장소와 로컬저장소의 파일, 폴더 상태가 같아야 함
* 동일한 저장소를 관리하는 사람일 경우 gitconfig에 등록된 이름, 이메일이 동일해야 함
----
# 주요 단축키 모음
* `crtl+/` 한 줄 통으로 주석
* `shift+alt+a` 선택한 영역(드래그)만 주석
----
# 맨 처음 git을 이용한 gitHub 저장소 업로드 시 해야하는 순서 (세팅 포함)
1. 현재 사용중 로컬 저장소를 git 저장소 등록 `git init`
2. 1번 정상 등록 시 경로에 (master) 표시 출력
3. master -> main으로 최상위 경로 명칭 변경 위해 `git branch -m main`
4. gitHub 저장소 생성 후 저장소 주소 복사
5. 현재 로컬 저장소 gitHub 저장소 연결 `git remote add origin 주소 붙여넣기`
6. `git status` 현재 상태 확인 (스테이징, 작업 드렉터리, 저장소)
7. 위 6번 결과 파일이 빨간색으로 출력될 경우 `git add 파일명`
8. `git status` 위 7번에서 올린 파일이 초록색으로 변경된 걸 확인
9. `git commit -m '기록 메시지'` 스테이징 파일을 저장소에 올리기 위한 기록 설정
10. `git push origin main` 깃허브 저장소에 최종 파일, 폴더 업로드
11. 위 10번 처음 진행 시 깃허브 계정 인증 화면 나오니 인증 진행 후 저장소 F5
12. 