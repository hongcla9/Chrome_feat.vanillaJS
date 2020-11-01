##자바스크립트를 이용한 크롬앱 기능 만들기

1. date 함수로 시계 기능 추가 - gettime함수로 실시간 가져오기 -
   setinterval로 1초에 한번씩 시간 업뎃
   (if문을 이용하여 시간을 1 -> 01 로 되도록 만들었습니다.)

2 .loadName function을 이용하여 브라우저에 입력되는 값을 가져온다.
for문을 이용하여 유저입력값이 null값일 경우와 채워졌을때(else)를 적용
-null값일 경우 askForName함수를통해 이름을 물어보게된다.

3. handleSubmit을 이용하여 이름을 입력했을때 Hello+유저네임이 나오도록하는 기능

- index.html에서 form을 만들어 이름을 적는 input을 적용
- preventDefault를 이용하여 입력되는 정보를 보내는 기본동작 이벤트를 막는다.
- 입력값을 value값으로 바꾸고 paintgreeting funtion 을 이용
- save 함수로 저장하여 새로고침을 해도 유저값이 유지되도록 한다.

4. todo list 작성기능
   할일 목록 (TODO 저장, 목록을 ARRAY로 저장)
   -- greeting과 같이 기본동작 이벤트를 막고 값이 유지되도록 설정,
   버튼추가, 목록리스트를 span 으로 설정.
   -- 목록을 적을때마다 toDoObj에 저장

5. weather API 를 이용한 날씨보여주기 기능
   다른 서버로부터 손쉽게 데이터를 가져올수있는 수단인 API를 이용

- askForCoord로 현재 위치 가져오기
- 경도와 위도를 이용해 현재 날씨를 불러오기
