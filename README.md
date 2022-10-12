# 게시판 구현


## 구현 해야될 리스트
- [ ] 댓글 CRUD
- [x] 게시글 조회수
- [x] 페이징 기능 구현 
- [x] 게시글 CURD 기능 구현
- [x] 게시글 검색 기능 구현
- [ ] 최신순, 조회수 순으로 정렬 기능
- [ ] 게시글 보이는 갯수 조정 기능
- [ ] HTTP API 제공    
</br>

## 문제 발생 및 해결
* ~~글쓰기 버튼 누를 시 세션 자동 생성 문제~~  &rightarrow; 해결 https://github.com/Jeongho0805/portfolio/issues/1
* ~~게시글 제목 글자색, 밑줄 디자인 변경 시 몇몇 게시글들은 적용이 안되는 문제 발생~~ &rightarrow; 해결 https://github.com/Jeongho0805/portfolio/issues/2
* ~~ajax 비동기 전달 방식 사용시 댓글이 중복되어 출력되는 문제, 첫 댓글 입력시 새로고침 해야 댓글이 보이는 문제~~ &rightarrow; 해결 https://github.com/Jeongho0805/portfolio/issues/3

</br>

## 생각해 볼 거리
* 게시글 삭제 기능을 구현할 때 꼭 post method 방식으로 요청을 전달해야 하는가?
* get방식으로 게시글 번호를 쿼리파라미터에 전달 후 Session을 통한 해당 인가를 확인하는 방법을 사용하면 않되나?
* 예외 처리 고민해보기, optional활용 방법 공부
* entity 삭제 시 연관관계 매핑된 다른 entity자동 삭제 여부 파악
* 댓글 구현에 있어서 ajax(비동기 처리방식)을 쓰는 이유?  &rightarrow; 댓글을 쓸때마다 페이지 이동이 되지 않고 바로바로 댓글 목록만 업데이트 하기 위해!
* ajax호출 이후 기존에 업로드된 댓글 내용을 자바스크립트로 지우고 전체 html이 아닌 comment section만 재요청하는식으로 동작 구현   &rightarrow; 전체 페이지가 새로고침 되지 않지만 댓글부분은 껌뻑거리면서 부드럽지 못한 현상 발생, 다른 방법이 있는지 생각해보기

## 날짜별 업데이트 내용
### 2022-08-30
* 게시글 최신순으로 기본 정렬
* 글쓰기 권한 오류 메세지 출력 버그 수정
### 2022-08-31
* 게시글 list 제목 색상 밑 디자인 변경
* 게시물 delete 기능 구현
### 2022-09-02
* 게시글 update 기능 구현
### 2022-09-09
* ajax를 활용한 댓글 작성 및 업로드 기능 구현
### 2022-10-25
* 스프링 인터셉터를 활용한 Session 공통 로직 처리
* 로그인 로그아웃 화면 페이지 구현
* 회원 정보 네비바 표시



