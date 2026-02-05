<div align="center">
  <img src="./fundraising-heart.svg" width="100" alt="Sowon's Heart" />

  <h1>Hi there, I'm Sowon Kim! 👋</h1>

  <h3>🎨 Textile Design ➔ Frontend Developer 💻</h3>

  <p>
    <b>"텍스타일의 패턴을 짜듯, 견고하고 아름다운 코드를 설계합니다."</b><br />
    사용자 경험을 최우선으로 생각하며, <b>Agile</b>한 성장과 기록을 즐기는 개발자입니다.
  </p>

  <br />

  <a href="./RESUME.pdf" target="_blank" rel="noopener noreferrer">
    <img
      src="https://img.shields.io/badge/Resume-PDF-FF4D4D?style=for-the-badge&logo=adobeacrobatreader&logoColor=white"
      alt="Resume PDF"
    />
  </a>
  &nbsp;
  <a href="https://until.blog/@sowonkim" target="_blank" rel="noopener noreferrer">
    <img
      src="https://img.shields.io/badge/Tech%20Blog-until.blog-111827?style=for-the-badge&logo=rss&logoColor=white"
      alt="Tech Blog"
    />
  </a>

  <br /><br />

  <a href="https://skillicons.dev" target="_blank" rel="noopener noreferrer">
    <img
      src="https://skillicons.dev/icons?i=html,css,js,ts,react,nextjs,vite,tailwind,reactquery,supabase,vercel,git,github,figma&perline=7"
      height="80"
      alt="Skills"
    />
  </a>

  <br />
</div>

<br />
<hr />
<br />

## ⭐ Featured Project — Play Type (Team)

> **게임 추천 + 커뮤니티** 서비스  
> 저는 **탐색(검색/필터)**부터 **마이페이지(프로필/대시보드/위시리스트/리뷰)**까지, 사용자가 “내 정보와 활동을 관리하는 흐름”을 설계·구현했습니다.

**🔗 Links**
- Live: https://oz-union-fe-14-team1.vercel.app/
- Repo: https://github.com/oz-union-14-team1/oz-union-fe-14-team1

### ✨ Key Features (Implemented)
- 🔎 **Header Search / Filter**: 검색·필터 UI와 상태 흐름을 구성해 탐색 경험 강화
- 🙍 **My Page Profile**: **프로필 업로드 + 이미지 크롭** 기능 구현
- 📊 **Dashboard**: **위시리스트 수 / 내가 쓴 리뷰 수**를 한 눈에 보여주는 대시보드
- 💖 **Wishlist**: 관심 게임 저장/해제 및 목록 관리
- 🗂️ **My Reviews**: 내가 작성한 리뷰 모아보기 페이지

### 🧩 Tech Stack
React · TypeScript · Tailwind CSS · REST API (Custom) · Vercel · Git/GitHub

---

### 🛠️ Troubleshooting — Profile Image Persistence
- **문제**: 프로필 이미지 업로드 후 로그아웃/재로그인 시 이미지가 사라짐  
- **원인**: 업로드 API는 존재했지만 **조회 API가 없고**, `/user/me` 응답에도 `profile_img_url`이 포함되지 않아 localStorage 임시저장에 의존  
- **해결**: **GET /user/me/image** API 추가 + React Query 캐싱/동기화 + 업로드 성공 시 `invalidateQueries(['profileImage'])`로 자동 갱신  
- **결과**: 재로그인 유지 · 새로고침 불필요 · 멀티 디바이스 동기화 가능  

👉 상세 정리: [docs/troubleshooting/profile-image.md](./docs/troubleshooting/profile-image.md)

<br />

## 🚀 Projects

| Project Name | Description | Links |
| :---: | :---: | :---: |
| **🎮 Play Type** | 게임 추천 및 커뮤니티 서비스 (Team) | [![Live](https://img.shields.io/badge/Live-🚀-00C853?style=flat-square)](https://oz-union-fe-14-team1.vercel.app/)
