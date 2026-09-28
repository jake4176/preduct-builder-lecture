# preduct-builder-lecture

**Live site / 사이트 바로가기:** https://jake4176.github.io/preduct-builder-lecture/

[English](#english) · [한국어](#한국어)

---

## English

### Lotto 6/45 Number Generator

A browser-based simulator that draws Korean Lotto 6/45 numbers with an animated reveal. The interface is in Korean.

#### Features

- **1 to 5 sets per draw** (sets A–E; 5 sets = one full ticket)
- **Optional bonus number**: draw 6 numbers, or 6 + 1 bonus
- **Custom filters**
  - Pin up to 5 numbers that must appear in every set
  - Exclude numbers you never want drawn
- **Color-coded balls** by range: 1–10 yellow, 11–20 blue, 21–30 red, 31–40 gray, 41–45 green
- **Sound effects** during the draw (can be turned off)
- **Copy results** to the clipboard in one click
- **Recent draw history**: the last 25 sets, saved in your browser (`localStorage`)

#### How it works

Everything is in a single `index.html` file: no build step, no framework, no server. Each set is drawn by shuffling the remaining numbers (Fisher–Yates) after applying your include/exclude filters.

To run it locally, just open `index.html` in a browser.

> This is for fun only. Every draw is random, and no method can predict winning numbers.

---

## 한국어

### 행운의 로또 6/45 번호 추첨기

애니메이션과 함께 로또 6/45 번호를 뽑아 주는 웹 추첨 시뮬레이터입니다.

#### 주요 기능

- **한 번에 1~5세트 추첨** (A~E 세트, 5세트 = 1게임)
- **보너스 번호 선택**: 6개만 뽑거나, 보너스 포함 6+1개 추첨
- **맞춤 번호 필터**
  - 모든 세트에 반드시 포함할 번호 최대 5개 지정
  - 추첨에서 제외할 번호 지정
- **번호대별 공 색상**: 1~10 노랑, 11~20 파랑, 21~30 빨강, 31~40 회색, 41~45 초록
- **효과음** (끄기 가능)
- **결과 복사**: 클릭 한 번으로 클립보드에 복사
- **최근 추첨 기록**: 최근 25세트를 브라우저(`localStorage`)에 저장

#### 동작 방식

모든 코드가 `index.html` 파일 하나에 들어 있어 빌드 과정, 프레임워크, 서버가 필요 없습니다. 포함/제외 필터를 적용한 뒤 남은 번호를 무작위로 섞어(Fisher–Yates) 각 세트를 뽑습니다.

내 컴퓨터에서 실행하려면 `index.html` 파일을 브라우저로 열면 됩니다.

> 재미로만 사용해 주세요. 모든 추첨은 무작위이며, 당첨 번호를 예측할 수 있는 방법은 없습니다.
