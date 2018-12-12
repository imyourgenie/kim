1. 영화진흥위원회 오픈 API를 활용해 input으로 날짜를 받아 targetDt를 설정한 후 requests로 해당 날짜에 상영하는 영화들에 관한 data를 불러온다.
2. requests로 가져온 data를 for문과 slicing을 활용해 각 영화 별로 정리한다.
3. find와 slicing을 활용해 데이터에서 영화 제목, 순위, 누적관객수, 개봉일을 추출한다.
4. 추출한 영화 제목, 순위, 누적관객수, 개봉일을 tuple로 묶어 한눈에 보기 쉽게 정리한다.
