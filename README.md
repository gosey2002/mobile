# 포유스퀘어 모바일 · 렌탈 랜딩페이지

휴대폰 개통(SKT·KT·LGU+) · 인터넷·TV 결합 · 스카이렌탈 생활가전 렌탈 상담 접수용 원페이지.

- 운영 주소: https://mobile.4usquare.co.kr/
- 호스팅: GitHub Pages (`gosey2002/mobile`) — **게시 브랜치는 `gh-pages`**, 저장소 원본은 `main`
- DNS: 호스팅케이알 `mobile` CNAME → `gosey2002.github.io`
- 상담 접수: FormSubmit → realoio@naver.com (`?submitted=1` 완료 화면)
- 디자인: 밝은 쇼핑몰·상담 허브 톤 — 화이트 + `#F4F8FF`/`#EEF4FF` 섹션 교차, 코발트 `#2563EB`·스카이 `#0EA5E9` 포인트, 민트 `#10B981` 보조, 카카오 옐로 `#FEE500`, Pretendard (2026-11-27 리스타일)

## 하위 페이지

- `internet/index.html` — 인터넷·TV 신청 전용 랜딩 (`https://mobile.4usquare.co.kr/internet/`)
  - 메인과 같은 디자인 토큰(화이트·코발트/스카이·민트, Pretendard)을 쓰지만 CSS는 페이지 안에 자체 포함돼 있습니다. 색·컴포넌트를 바꿀 때는 `index.html`과 `internet/index.html`의 `<style>`을 함께 수정하세요.
  - 상담 폼도 같은 FormSubmit(`realoio@naver.com`)으로 접수되며, 메일 제목에 `인터넷·TV 상담 신청`으로 구분됩니다.
  - 인기 조합 TOP 3 금액은 2026-11-20 인터넷 단가표 기준 예시입니다. 금액을 바꾸면 아래 고지 문구와 `sitemap.xml`도 함께 확인하세요.

## 수정할 때

```bash
# 1) main에 커밋
git add -A && git commit -m "수정 내용"
git push origin main
# 2) 게시 브랜치(gh-pages)도 같은 내용으로 맞춰야 실제 사이트에 반영됩니다
git push origin main:gh-pages
```

GitHub Pages 설정에서 Source를 `main / (root)`로 바꾸면 1번만 하면 됩니다. (API 권한이 없어 현재는 `gh-pages`로 게시 중)

## 작성 규칙

- 금액·혜택·사은품을 보장하는 문구(최저가, 공짜폰, 최대 현금 등)는 넣지 않습니다.
- 상담 폼 항목을 바꾸면 개인정보처리방침 모달의 수집 항목도 함께 수정합니다.
- 푸터에는 사업자등록번호를 표기하지 않습니다.
