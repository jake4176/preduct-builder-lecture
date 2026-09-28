# preduct-builder-lecture

**Live site / 사이트 바로가기:**
- 🎰 Lotto 6/45 / 로또 번호 추첨기: https://jake4176.github.io/preduct-builder-lecture/
- 🐶 Animal face test / 동물상 테스트: https://jake4176.github.io/preduct-builder-lecture/animal-test.html

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
- **Dark / light mode**: toggle with the button in the top-right corner; follows your system setting until you choose, then remembers your choice
- **Partnership inquiry form**: visitors can send partnership or collaboration requests; submissions are delivered through [Formspree](https://formspree.io)
- **Comments**: visitor comments at the bottom of the page, powered by [Disqus](https://disqus.com); loads only when you scroll near it and matches the dark/light theme

### Animal Face Test (`animal-test.html`)

Upload a photo and an image model tells you whether you look more like a dog or a cat.

- Built on a [Teachable Machine](https://teachablemachine.withgoogle.com/) image model trained on dog and cat photos
- Shows dog/cat percentages, a result type (dog, cat, or half-and-half), and a short description
- **Photos never leave your device**: the model runs in your browser with TensorFlow.js
- Upload by tapping or drag-and-drop, **or use your webcam** with a live dog/cat meter and one-tap capture
- Share the result with one click
- Same dark/light theme as the lotto page

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
- **다크 / 라이트 모드**: 오른쪽 위 버튼으로 전환. 처음에는 기기 설정을 따르고, 한 번 선택하면 그 선택을 기억
- **제휴 문의 폼**: 방문자가 광고·협업·제휴 제안을 보낼 수 있으며, [Formspree](https://formspree.io)를 통해 전달
- **댓글**: 페이지 맨 아래에 [Disqus](https://disqus.com) 댓글. 근처까지 스크롤하면 불러오며, 다크/라이트 모드에 맞춰 표시

### 동물상 테스트 (`animal-test.html`)

사진을 올리면 AI가 강아지상인지 고양이상인지 알려 주는 테스트입니다.

- 강아지·고양이 사진으로 학습한 [Teachable Machine](https://teachablemachine.withgoogle.com/) 이미지 모델 사용
- 강아지상/고양이상 비율(%), 결과 유형(강아지상·고양이상·반반상), 한 줄 설명 표시
- **사진은 서버로 전송되지 않음**: TensorFlow.js로 방문자 브라우저 안에서만 분석
- 눌러서 올리기, 끌어다 놓기, 또는 **웹캠 모드**(실시간 강아지/고양이 비율 표시 후 버튼 한 번으로 결과 보기)
- 결과 공유 버튼 지원
- 로또 페이지와 같은 다크/라이트 테마

#### 동작 방식

모든 코드가 `index.html` 파일 하나에 들어 있어 빌드 과정, 프레임워크, 서버가 필요 없습니다. 포함/제외 필터를 적용한 뒤 남은 번호를 무작위로 섞어(Fisher–Yates) 각 세트를 뽑습니다.

내 컴퓨터에서 실행하려면 `index.html` 파일을 브라우저로 열면 됩니다.

> 재미로만 사용해 주세요. 모든 추첨은 무작위이며, 당첨 번호를 예측할 수 있는 방법은 없습니다.
