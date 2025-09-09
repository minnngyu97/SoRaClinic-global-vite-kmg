# 🌟 프로젝트 개요

**SoraClinic 글로벌 웹사이트** 프로젝트입니다.  
현대적인 UI, 반응형 디자인, 예약 시스템, 관리자 대시보드 등 완전한 웹 플랫폼을 제공합니다.

---

## 👥 Team

<ul>
    <li>조태정 – 기획/디자인</li>
    <li>수산나 – 개발/디자인</li>
    <li>김민규 – 개발</li>
</ul>
 
---

## 🔑 주요 기능

<ul>
  <li><strong>다중 페이지 네비게이션</strong>: 홈, 이벤트, 소개, 치료</li>
  <li><strong>관리자 대시보드</strong>: 미리보기 모드 사용 가능</li>
  <li><strong>예약 시스템</strong>: 모달 기반 예약 시스템</li>
  <li><strong>반응형 디자인</strong>: 모바일 우선 접근법</li>
  <li><strong>현대적인 UI</strong>: Radix UI 컴포넌트와 Tailwind CSS로 구축</li>
  <li><strong>Supabase 통합</strong>: 백엔드 서비스 및 데이터베이스</li>
</ul>

---

## 📄 사용 가능한 페이지

<table>
  <thead>
    <tr>
      <th>페이지</th>
      <th>경로</th>
      <th>설명</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>홈 페이지</strong></td>
      <td><code>/</code></td>
      <td>연락처 섹션이 있는 메인 랜딩 페이지</td>
    </tr>
    <tr>
      <td><strong>이벤트 페이지</strong></td>
      <td><code>/event</code></td>
      <td>이벤트 정보 및 업데이트</td>
    </tr>
    <tr>
      <td><strong>소개 페이지</strong></td>
      <td><code>/about</code></td>
      <td>회사 정보</td>
    </tr>
    <tr>
      <td><strong>치료 페이지</strong></td>
      <td><code>/treatments</code></td>
      <td>서비스 제공 내용</td>
    </tr>
    <tr>
      <td><strong>관리자 대시보드</strong></td>
      <td>–</td>
      <td>관리 인터페이스 (미리보기 모드 사용 가능)</td>
    </tr>
  </tbody>
</table>

---

## ⚙️ 개발 명령어

<pre>
npm run dev   # 개발 서버 시작
npm run build # 프로덕션용 빌드
</pre>

> 기본적으로 서버는 **포트 3000**에서 실행됩니다.

---

## 🛠 기술 스택

<ul>
  <li><strong>프론트엔드</strong>: React 18, TypeScript</li>
  <li><strong>빌드 도구</strong>: Vite</li>
  <li><strong>UI 컴포넌트</strong>: Radix UI, Tailwind CSS</li>
  <li><strong>스타일링</strong>: CSS 모듈, Tailwind CSS</li>
  <li><strong>백엔드</strong>: Supabase 통합</li>
  <li><strong>폼 관리</strong>: React Hook Form</li>
  <li><strong>아이콘</strong>: Lucide React</li>
</ul>

<pre><code>
{
  "dependencies": {
    "react": "^18.3.1",
    "react-dom": "^18.3.1"
  },
  "devDependencies": {
    "@eslint/js": "^9.13.0",
    "@types/react": "^18.3.12",
    "@types/react-dom": "^18.3.1",
    "@vitejs/plugin-react": "^4.3.3",
    "eslint": "^9.13.0",
    "eslint-plugin-react-hooks": "^5.0.0",
    "eslint-plugin-react-refresh": "^0.4.14",
    "globals": "^15.11.0",
    "typescript": "~5.6.2",
    "typescript-eslint": "^8.11.0",
    "vite": "^5.4.10"
  }
}
</code></pre>

<h2>:file_folder: Folder Structure (Simplified)</h2>
<pre><code>
App.tsx (메인 컨테이너)
├── Navigation.tsx (상단 네비게이션)
│   ├── LanguageSelector.tsx (언어 선택)
│   └── Mobile Menu (Sheet 컴포넌트)
│
├── 페이지 라우팅 (동적 렌더링)
│   ├── HomePage.tsx
│   │   ├── BeautyCarousel.tsx (메인 캐러셀)
│   │   └── ContactSection.tsx
│   │       ├── ContactInfo.tsx
│   │       ├── ContactMap.tsx
│   │       └── SocialMedia.tsx
│   │
│   ├── EventPage.tsx (이벤트 페이지)
│   ├── AboutPage.tsx (소개 페이지)
│   ├── TreatmentsPage.tsx (트리트먼트 페이지)
│   └── AdminPage.tsx (관리자 대시보드)
│       └── AdminLoginPage.tsx (로그인)
│
├── BookingModal.tsx (예약 모달)
│   └── 예약 폼 (shadcn/ui 컴포넌트들)
│
├── Footer.tsx (푸터)
│   └── 연락처 정보
│
└── Toaster (알림 시스템)
    └── sonner 컴포넌트

</code></pre>

## :흰색_확인_표시: Git 단독 커밋 체크리스트
### 1. 초기 세팅
<pre><code>
| 버전 | 상태 | 항목 |
|------|------|
| - [ ] | chore: initialize vite react-ts project |
| - [ ] | chore: add tailwindcss + postcss + autoprefixer |
| - [ ] | chore: add eslint + prettier |
</code></pre>
---
<pre><code>
### 2. 공용 설정
| 버전 | 상태 | 항목 |
|------|------|
| - [ ] | chore: add global styles and fonts (Pretendard) |
| - [ ] | chore: configure tsconfig paths and aliases |
</code></pre>
---
<pre><code>
### 3. 타입 & 유틸
| 버전 | 상태 | 항목 |
|------|------|
| - [ ] | feat(types): add common interfaces (user, auth, board) |
| - [ ] | feat(utils): add api client and helpers |
</code></pre>
---
<pre><code>
### 4. UI 레이아웃
| 버전 | 상태 | 항목 |
|------|------|
| - [ ] | feat(layout): add header and footer |
| - [ ] | feat(layout): add global navigation |
| - [ ] | feat(layout): add container and responsive grid |
</code></pre>
---
<pre><code>
### 5. 주요 기능
| 버전 | 상태 | 항목 |
|------|------|
| - [ ] | feat(auth): add login component |
| - [ ] | feat(auth): add register component |
| - [ ] | feat(board): add board list and detail |
| - [ ] | feat(reservation): add reservation form |
| - [ ] | feat(reservation): integrate calendar/time picker |
</code></pre>
---
<pre><code>
### 6. 스타일 & UI 개선
| 버전 | 상태 | 항목 |
|------|------|
| - [ ] | style: apply tailwind theme tokens (colors, spacing) |
| - [ ] | style: add button and input components |
| - [ ] | style: add responsive hero section |
</code></pre>
---
<pre><code>
### 7. 기타 관리
| 버전  | 상태 | 항목 |
|------|------|
| - [ ] | docs: add README with project setup instructions |
| - [ ] | chore: add gitignore and editorconfig |
| - [ ] | chore: add vercel deployment config |
| - [ ] | test: add sample unit tests (if applicable) |
</code></pre>
---
<pre><code>
### :압정: 커밋 컨벤션
- **feat:** 새로운 기능 추가
- **fix:** 버그 수정
- **style:** 스타일/레이아웃 수정 (기능 영향 없음)
- **chore:** 환경 세팅/빌드/패키지 관리
- **docs:** 문서 작업 (README, 주석)
- **refactor:** 리팩토링 (기능 변화 없음)
- **test:** 테스트 코드
</code></pre>