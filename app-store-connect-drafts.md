# App Store Connect Drafts

## Read First

These drafts assume the current native macOS app:

- does not require sign-in
- does not upload user files to a server
- does not use analytics, ads, or crash-reporting SDKs
- uses user-selected background images only on-device

If any of those change, the App Privacy answers and privacy policy should be updated before submission.

One note worth checking before release:

- `/Users/hanjungoo/workspace/blackhole/styles.css` still imports Google Fonts.
- If the shipped macOS app never loads the bundled web UI, this is likely irrelevant.
- If any bundled web view is exposed in production, it is safer to remove that external font import before submission.

## Category

- Primary category: `Graphics & Design`

## App Description Draft

### English

Blackhole is a cinematic black hole simulator for macOS.

Explore gravitational lensing, accretion disk motion, celestial infall events, and NASA image backdrops in a native desktop experience designed for visual immersion.

Features:

- Single black hole mode and experimental binary mode
- Adjustable computation presets for performance tuning
- Pointer, hover, and flyby camera controls
- NASA background image selection and custom background support
- Accretion disk color controls, visibility toggle, and disk orientation controls
- Real-time HUD for FPS, CPU, GPU, and render statistics

Blackhole is designed as a visual simulation and desktop art experience inspired by relativistic black hole imagery. It is not intended to be a scientific instrument.

### Korean

Blackhole은 macOS용 블랙홀 시네마틱 시뮬레이터입니다.

중력렌즈 효과, 강착원반의 흐름, 천체 유입 이벤트, NASA 배경 이미지를 네이티브 앱에서 몰입감 있게 감상할 수 있습니다.

주요 기능:

- 싱글 블랙홀 모드와 실험적인 바이너리 모드
- 성능에 맞게 조절 가능한 계산 프리셋
- 마우스 시점, 자동 호버링, 플라이바이 카메라
- NASA 배경 이미지 선택 및 사용자 배경 지원
- 강착원반 색상, 표시 여부, 방향 제어
- FPS, CPU, GPU, 렌더 통계를 보여주는 실시간 HUD

Blackhole은 상대론적 블랙홀 이미지를 바탕으로 한 시각적 시뮬레이션이자 데스크톱 아트 경험이며, 과학 측정 도구를 목표로 하지는 않습니다.

## Keywords Draft

### English

`blackhole,space,simulation,lensing,accretion,nasa,desktop,wallpaper,relativity`

### Korean

`블랙홀,우주,시뮬레이션,중력렌즈,강착원반,NASA,배경화면,데스크톱`

## Screenshot Plan

Use at least 4 to 6 screenshots.

Recommended set:

1. Single black hole with a strong accretion disk and NASA background
2. Close-up lensing view with the disk clearly wrapping above and below the shadow
3. Flyby view passing near the accretion disk
4. Background picker with NASA previews visible
5. Color and helper controls visible
6. Experimental binary mode

Suggested captions:

- `Relativistic black hole visuals on your desktop`
- `Explore lensing, accretion flow, and flyby camera motion`
- `Choose NASA backdrops and tune the scene in real time`
- `Monitor GPU, CPU, FPS, and render quality live`

## Support URL Draft

Recommended final URL pattern:

- `https://your-domain.example/support`

Or, if you do not buy a domain:

- `https://<username>.github.io/blackhole/support`

Support page should include:

- short app description
- supported macOS version
- contact email
- basic troubleshooting
- note that custom background images stay local

## Privacy Policy URL Draft

Recommended final URL pattern:

- `https://your-domain.example/privacy`

Or, if you do not buy a domain:

- `https://<username>.github.io/blackhole/privacy`

## App Privacy Answers Draft

Assuming the current app behavior stays the same:

- Does this app collect data from users? `No`
- Does this app use tracking? `No`

This means the App Privacy section should be submitted as:

- `Data Not Collected`

Use this only if you continue shipping without:

- analytics SDKs
- ad SDKs
- crash-reporting services
- account sign-in
- cloud sync
- server upload of user-selected files

## Publishing Guidance For URLs

You do **not** need to buy a domain just to submit the app.

The Support URL and Privacy Policy URL only need to be:

- public
- reachable without login
- stable
- ideally HTTPS

Acceptable practical options:

- GitHub Pages
- a simple static site host
- a public Notion page
- a public Carrd or similar page

Buying your own domain is better for trust and branding, but it is not required.
