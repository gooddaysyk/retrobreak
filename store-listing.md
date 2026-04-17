# 📱 RETROBREAK 2P — 구글 플레이 스토어 등록 자료

---

## ✅ 앱 기본 정보

| 항목 | 내용 |
|------|------|
| **앱 이름** | RETROBREAK 2P |
| **패키지명** | com.retrobreak.twoplayer |
| **카테고리** | 게임 > 아케이드 |
| **콘텐츠 등급** | 전체 이용가 (IARC 3+) |
| **유료/무료** | 무료 |
| **광고 포함** | 없음 |
| **인앱결제** | 없음 |

---

## 📝 짧은 설명 (80자 이내)

```
두 명이 폰 하나로! 레트로웨이브 감성의 2인 대결 벽돌깨기 게임
```

---

## 📄 전체 설명 (4,000자 이내)

```
🎮 RETROBREAK 2P — 한 폰으로 즐기는 2인 대결 벽돌깨기

스마트폰 하나만 있으면 OK!
테이블에 폰을 놓고 마주 앉아 즐기는 레트로웨이브 감성의 대결 벽돌깨기 게임입니다.

━━━━━━━━━━━━━━━━━━━━━━━
🕹️ 게임 방법
━━━━━━━━━━━━━━━━━━━━━━━
• P1 (아래쪽 플레이어): 화면 아래쪽을 손가락으로 밀어 패들 조작
• P2 (위쪽 플레이어): 화면 위쪽을 손가락으로 밀어 패들 조작
• 가운데 벽돌 지대를 통과시켜 상대방 진영으로 공을 보내세요
• 공이 상대 영역을 통과하면 1점 획득
• 먼저 5점을 획득한 플레이어가 승리!

━━━━━━━━━━━━━━━━━━━━━━━
⚡ 주요 특징
━━━━━━━━━━━━━━━━━━━━━━━
✦ 공 속도 3단계 조절 (느림 / 보통 / 빠름)
✦ 교대 서브 시스템 — 공정한 대결 보장
✦ 레트로웨이브 네온 비주얼
✦ 득점 시 네온 플래시 효과 & 효과음
✦ 풀스크린 지원 (주소창 없이 게임만 표시)
✦ 인터넷 연결 불필요

━━━━━━━━━━━━━━━━━━━━━━━
👥 이런 분께 추천
━━━━━━━━━━━━━━━━━━━━━━━
• 30~40대 아케이드 게임 향수를 느끼고 싶은 분
• 커플, 친구, 가족과 간단한 대결 게임을 즐기고 싶은 분
• 별도 장비 없이 스마트폰 하나로 2인 게임을 원하는 분
• 카페, 식당에서 기다리는 시간을 게임으로 채우고 싶은 분

━━━━━━━━━━━━━━━━━━━━━━━
🔒 개인정보
━━━━━━━━━━━━━━━━━━━━━━━
• 개인정보 수집 없음
• 인터넷 연결 불필요 (오프라인 플레이 가능)
• 광고 없음 · 인앱결제 없음
```

---

## 🔑 키워드 (ASO 최적화)

```
벽돌깨기, 2인용게임, 아케이드, 레트로게임, 대결게임, 
breakout, 2player, arcade, retro, 친구게임, 커플게임,
오프라인게임, 가족게임, 간단게임, 파티게임
```

---

## 🖼️ 필요한 그래픽 에셋

| 에셋 | 크기 | 형식 | 비고 |
|------|------|------|------|
| 앱 아이콘 | 512 × 512 px | PNG (32-bit) | 배경 포함 |
| 기능 그래픽 | 1024 × 500 px | PNG/JPG | 스토어 상단 배너 |
| 스크린샷 (세로) | 1080 × 1920 px | PNG/JPG | 최소 2장, 최대 8장 |

### 아이콘 디자인 방향
- 배경: 짙은 네이비/퍼플 (#040010)
- 중앙: 네온 핑크(P2) + 시안(P1) 패들이 공을 주고받는 미니멀 아이콘
- 텍스트: "2P" 네온 글로우 효과

---

## 📋 스토어 등록 체크리스트

### 필수 준비물
- [ ] APK 또는 AAB 파일 (서명된 릴리즈 빌드)
- [ ] 앱 아이콘 512×512 PNG
- [ ] 기능 그래픽 1024×500
- [ ] 스크린샷 최소 2장
- [ ] 개인정보처리방침 URL (privacy-policy.html 호스팅)
- [ ] 구글 플레이 개발자 계정 ($25 1회 등록비)

### 콘텐츠 등급 설문 (IARC)
- 폭력: 없음
- 성인 콘텐츠: 없음
- 도박: 없음
- 언어: 없음
→ **예상 등급: 전체이용가 (Everyone)**

### 타겟 연령
- 주 타겟: 13세 이상 전체
- 어린이 대상 여부: 아니오

---

## 🛠️ APK 제작 방법 (3가지 옵션)

### Option A: Capacitor (권장) — WSL2 환경
```bash
# 1. 프로젝트 폴더 생성
mkdir retrobreak && cd retrobreak
cp retrobreak-2p.html index.html
cp manifest.json .

# 2. Capacitor 설치
npm init -y
npm install @capacitor/core @capacitor/cli @capacitor/android

# 3. 초기화
npx cap init "RETROBREAK 2P" "com.retrobreak.twoplayer" --web-dir "."

# 4. Android 플랫폼 추가
npx cap add android

# 5. Android Studio에서 APK 빌드
npx cap open android
# → Build > Generate Signed Bundle/APK
```

### Option B: PWABuilder (가장 쉬움) — 코딩 불필요
```
1. 파일을 GitHub Pages 또는 Netlify에 호스팅
2. https://www.pwabuilder.com 접속
3. 사이트 URL 입력
4. "Package for stores" → Android → Download
5. 생성된 AAB 파일을 플레이 스토어에 업로드
```

### Option C: Kodular Creator — 코딩 불필요
```
1. kodular.io 접속 후 새 프로젝트 생성
2. WebViewer 컴포넌트 추가
3. Assets에 retrobreak-2p.html 업로드
4. WebViewer URL = "file:///android_asset/retrobreak-2p.html"
5. Screen1 → ShowStatusBar: false
6. APK 다운로드
```

---

## 📌 개인정보처리방침 URL 준비

Google Play는 개인정보처리방침 URL을 반드시 요구합니다.
`privacy-policy.html` 파일을 아래 중 하나에 무료 호스팅:
- **GitHub Pages**: yourname.github.io/retrobreak/privacy-policy.html
- **Netlify**: app.netlify.com (드래그&드롭 배포)
- **Google Sites**: sites.google.com (구글 계정으로 간편 생성)
