1. npm i -g json-server
터미널에 실행

2. json-server --watch db.json --port 3001
json 서버 3001번으로 실행

사용법

axios 로 요청을 할텐데
axios.post , axios.get , axios.delete
가 있을건데 밑에 명세서를 보고 post , get ,delete 에 맞춰서 요청을 보낼것
post 요청시 body에 key,value 값으로 데이터를 넣어서 요청해줘야함


명세서


GET

전체 게시글 가져오기

http://localhost:3001/board

특정 게시글 한개 가져오기
http://localhost:3001/board/id

id에 게시글 번호를 넣으면 된다.

예시
http://localhost:3001/board/1
하면 1번 아이디 게시글 내용을 가져옴


POST

게시글 저장하기
http://localhost:3001/board

필요 데이터 
body 안에 

title : '제목'
content : '내용'
user : '유저 아이디'

DELETE

게시글 삭제하기
http://localhost:3001/board/id

id에 게시글 번호를 넣으면 된다.

예시
http://localhost:3001/board/1
하면 1번 아이디 게시글이 삭제가 된다.
