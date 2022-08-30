# 게시판 구현


## 구현 해야될 리스트
- [ ] 댓글 (대댓글)
- [ ] 게시글 검색
- [x] 게시글 조회수
- [x] 페이징 기능 구현 
- [ ] 최신순, 조회수 순으로 정렬 기능    
</br>

## 문제 발생 및 해결
* ~~글쓰기 버튼 누를 시 세션 자동 생성 문제~~  &rightarrow; 해결 https://github.com/Jeongho0805/portfolio/issues/1
* 게시글 제목 글자색, 밑줄 디자인 변경 시 몇몇 게시글들은 적용이 안되는 문제 발생 https://github.com/Jeongho0805/portfolio/issues/2

</br>

## 생각해 볼 거리
* 게시글 삭제 기능을 구현할 때 꼭 post method 방식으로 요청을 전달해야 하는가?
* get방식으로 게시글 번호를 쿼리파라미터에 전달 후 Session을 통한 해당 인가를 확인하는 방법을 사용하면 않되나?
* 예외 처리 고민해보기, optional활용 방법 공부
* entity 삭제 시 연관관계 매핑된 다른 entity자동 삭제 여부 파악
</br>

## 날짜별 업데이트 내용
### 2022-08-30
* 게시글 최신순으로 기본 정렬
* 글쓰기 권한 오류 메세지 출력 버그 수정
### 2022-08-31
* 게시글 list 제목 색상 밑 디자인 변경
* 게시물 delete 기능 구현



