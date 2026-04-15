# Likey Assistant - Figma Plugin

Likey 팀을 위한 Figma 디자인 워크플로우 플러그인입니다.

## 기능

### 1. Data Fill
- Google Sheets 연동으로 더미 데이터 자동 채우기
- 크리에이터/팬 카테고리별 데이터 관리
- 레이어 이름 기반 자동 매칭
- 아바타 이미지 자동 채우기 (프로필 이미지 레이어 감지)
- 랜덤 채우기로 여러 레이어 한 번에 적용

### 2. Text Editor
- **텍스트 찾기**: 검색어 입력 시 현재 페이지의 일치하는 모든 텍스트 노드 목록 표시, 클릭하면 해당 노드로 이동·선택
- 찾아서 변경 기능 (기존텍스트>새텍스트)
- 네이버 맞춤법 검사 연동

### 3. Rename
- 선택 레이어 일괄 이름 변경
- 자동 네이밍 (Content, Section, Item, Image, Text)

### 4. Code2Design
- HTML/CSS 코드를 Figma 디자인으로 변환
- Tailwind CSS 지원 (클래스 자동 감지)
- Claude·Gemini 등 AI가 생성한 코드 붙여넣기 바로 사용 가능
- 마크다운 코드펜스(```html ... ```) 자동 제거

### 5. Checker
- 디자인 시스템 컴포넌트 적용 여부 확인
- 베리어블(변수) 적용 여부 확인
- 텍스트 스타일 적용 여부 확인

### 공통
- **탭 순서 변경**: 탭을 드래그해 원하는 순서로 재배치, 순서는 자동 저장되어 재시작 후에도 유지

---

## 설치 방법

### 1. 플러그인 파일 다운로드

**방법 A: ZIP 다운로드**
1. 이 저장소 페이지에서 녹색 `Code` 버튼 클릭
2. `Download ZIP` 선택
3. 다운로드된 ZIP 파일 압축 해제

**방법 B: Git Clone**
```bash
git clone https://github.com/design-neal/TPC-figma-plugin.git
```

### 2. Figma에서 플러그인 설치

1. Figma Desktop 앱 실행
2. 상단 메뉴에서 `Plugins` > `Development` > `Import plugin from manifest...` 클릭
3. 다운로드한 폴더에서 `manifest.json` 파일 선택
4. 플러그인이 `Development` 메뉴에 추가됨

### 3. 플러그인 실행

- `Plugins` > `Development` > `Likey Assistant` 클릭
- 또는 `Cmd/Ctrl + /` 눌러서 "Likey Assistant" 검색

---

## 파일 구조

```
plugin/
├── manifest.json    # 플러그인 설정 파일
├── code.js          # 플러그인 백엔드 로직
├── ui.html          # 플러그인 UI
└── README.md        # 이 문서
```

---

## 업데이트 방법

```bash
cd TPC-figma-plugin
git pull origin main
```

Figma를 재시작하면 변경사항이 자동으로 적용됩니다.

---

## 문의

문제가 있거나 기능 요청이 있으면 Issues에 등록해주세요.
