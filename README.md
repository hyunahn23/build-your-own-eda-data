# 🛠️ Build Your Own EDA Data

## Overview

본 레포지토리는 **20,000,000명의 PSN(PlayStation Network) 유저 데이터를 시뮬레이션**하여, EDA(탐색적 데이터 분석) 실습용으로 사용할 수 있는 **초대규모 synthetic dataset**을 생성합니다.

---

## 📂 Dataset Features

| 컬럼명              | 설명 |
|---------------------|------|
| User ID             | 유저 고유 ID (0부터 시작하는 정수) |
| Subscription Type   | 구독 유형: `Delux`, `Special`, `Essential` |
| Monthly Revenue     | 월별 예상 매출 (KRW) |
| Quarterly Revenue   | 분기별 예상 매출 (KRW) |
| Annual Revenue      | 연간 예상 매출 (KRW) |
| Join Date           | 기기별 첫 가입일 (YYYY-MM-DD) |
| Last Payment Date   | 마지막 결제일 |
| Country             | 유저 국가 |
| Age                 | 나이 (14~50세) |
| Gender              | 성별 (`Male`, `Female`) |
| Device              | 사용 기기 (`PS4`, `PS5`, `PS5_PRO`) |
| Plan Duration       | 구독 기간 (`1 Month`, `3 Month`, `12 Month`) |

---

## ⚙️ How It Works

- **기기별 출시일 기준 가입일 생성**
- **구독 유형에 따라 매출 분기 설정**
- **현실적인 국가 분포 및 연령대 비율 반영**
- **가입일 대비 결제일 랜덤화 처리**

---

## 📁 Output

생성된 데이터는 다음 경로에 저장됩니다:

```
./data/psn.csv
```

> ⚠️ 주의: 약 20,000,000개의 행을 포함하고 있어 저장 및 처리 시 메모리 주의 필요

---
