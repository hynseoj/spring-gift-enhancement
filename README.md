# spring-gift-enhancement

## 1단계 - 상품 카테고리
> 상품 정보에 카테고리를 추가한다.   
> 상품에는 항상 하나의 카테고리가 있어야 한다.   
> 2차 이상의 카테고리는 고려하지 않는다.   
> 
> <<카테고리 예시>>    
> _교환권, 상품권, 뷰티, 패션, 식품, 리빙/도서, 레저/스포츠, 아티스트/캐릭터, 유아동/반려, 디지털/가전, ..._
> 
> 아래 예시와 같이 HTTP 메시지를 주고 받도록 구현한다.
> ### Request
> ```
>    GET /api/categories HTTP/1.1
> ```
> ### Response
> ```
> HTTP/1.1 200
> Content-Type: application/json
> 
> [
>   {
>       "id": 91,
>       "name": "교환권",
>       "color": "#6c95d1",
>       "imageUrl": "https://gift-s.kakaocdn.net/dn/gift/images/m640/dimm_theme.png",
>       "description": ""
>   }
> ]

### 기능 요구사항 목록
- [x] 카테고리 엔티티 클래스 작성 + 카테고리 초기 데이터 삽입
- [x] 카테고리 전체 조회 기능 구현
- [ ] 상품 카테고리 지정 기능 구현
- [ ] 상품 카테고리 수정 기능 구현