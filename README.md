# KIS_Stock_MCP

**KIS_Stock_MCP**는 한국투자증권(KIS) OpenAPI를 활용하여 국내 주식의 시세, 잔고, 주문, 호가, 일별 주가 등 다양한 정보를 비동기(Async) 방식으로 조회·주문할 수 있도록 도와주는 Python MCP(Multi-Command Processor) 툴킷입니다.

---

## 주요 기능

- **현재가 조회**: 종목코드로 실시간 주가 및 주요 지표 조회
- **잔고 조회**: 계좌의 보유 종목 및 평가금액, 손익 등 정보 조회
- **주문 실행**: 매수/매도 주문(시장가·지정가) 실행
- **주문내역 조회**: 기간별 주문 체결 내역 요약 및 상세 조회
- **호가 조회**: 실시간 매수/매도 호가 및 잔량 조회
- **일별 주가 조회**: 종목의 과거 일별 시세 데이터 조회

---

## 파일 구조 및 주요 클래스

- **KISAuthManager**  
  - 토큰 발급/갱신 및 해시키 생성, 실전/모의투자 환경 자동 분기
- **MCP Tool Functions**  
  - `get_stock_price`: 종목 현재가 조회
  - `get_account_balance`: 계좌 잔고 조회
  - `place_order`: 매수/매도 주문 실행
  - `get_order_list`: 주문내역(중요 컬럼만) 조회
  - `get_stock_ask_price`: 호가(매수/매도) 조회
  - `get_daily_price`: 일별 주가 데이터 조회

---

---

## 주의사항

- 본 코드는 KIS OpenAPI의 정책 및 응답 포맷 변경에 따라 수정이 필요할 수 있습니다.
- 실전 계좌 사용 시, API 사용량 및 주문 실수에 주의하세요.
- 환경변수 및 인증정보는 외부에 노출되지 않도록 관리하세요.

---

## 라이선스

- 본 코드는 오픈소스 예시로 제공되며, 실제 투자 및 상업적 활용 시 한국투자증권 OpenAPI의 이용약관을 반드시 준수해야 합니다.

---

## 문의

- 개선 제안, 버그 신고 등은 이슈로 남겨주세요.  
- 한국투자증권 OpenAPI 공식 문서: [https://github.com/koreainvestment/open-trading-api](https://github.com/koreainvestment/open-trading-api)

---

**KIS_Stock_MCP**로 쉽고 빠르게 주식 자동화/데이터 분석을 시작해보세요!

