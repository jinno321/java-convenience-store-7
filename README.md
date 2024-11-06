# Java Convenience Store Precourse

## 1. Model

### PriceCalculator (가격 계산기)
- [ ] 상품과 개수가 담긴 리스트를 받아 모든 가격을 더한 값을 리턴하는 메서드
- [ ] 프로모션 및 멤버십 할인 정책을 적용하는 메서드

### Storage (창고 - 재고 관리)
- [ ] 결제 가능 여부 확인 - 불가능시 에러 처리
- [ ] 상품 구매 시, 재고 차감
- [ ] 최신 재고 유지

### item (상품)
- [ ] 이름
- [ ] 가격
- [ ] 프로모션

### PromotionManager (프로모션 관리)
- [ ] 프로모션 재고 차감
- [ ] 프로모션 재고 확인후 가능여부 확인
- [ ] 프로모션 안내(고객이 해당 수량보다 적게 가져온 경우)

### Promotion (enum) (프로모션 종류)
- [ ] 1+1 프로모션
- [ ] 2+1 프로모션
- [ ] MD추천상품
- [ ] 반짝할인

### MembershipManager (멤버십 관리)
- [ ] 멤버십 관리 기능 구현
- [ ] 멤버십 할인 최대한도

### Receipt (영수증)
- [ ] 총 구매액 관리
- [ ] 행사 할인 금액 기록
- [ ] 멤버십 할인 금액 기록
- [ ] 최종 결제 금액 기록

## 2. View

### InputView 
- [ ] 구매할 상품명,수량 입력
- [ ] 멤버십 할인 유무 입력
- [ ] 프로모션 재고보다 적게 가져왔을 때, 혜택에 대한 안내메시지 출력 및 추가 유무 입력
- [ ] 프로모션 혜택미적용 안내 및 구매 유무 입력
- [ ] 추가 구매 희망여부 입력

### OutputView
- [ ] 재고 출력
- [ ] 영수증 출력
- [ ] 에러 출력

## 3. Service

### StorageService
- [ ] 상품명과 수량으로 구매 시도하기
- [ ] 상품명,수량만큼 재고 줄이기

### MembershipService
- [ ] 멤버십 할인 적용하기

### PromotionService 
- [ ] 프로모션 적용

## 4.Util

### Parser
- [ ] 입력받은 파일에서 띄워쓰기 기준으로 나누기
- [ ] 입력받은 상품들 , 기준으로 나누기
- [ ] 입력받은 상품명과 수량으로 분리하기

### ErrorHandler - 에러 관리
