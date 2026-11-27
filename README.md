# 포유스퀘어 모바일 · 렌탈 랜딩페이지

휴대폰 개통(SKT·KT·LGU+) · 인터넷·TV 결합 · 스카이렌탈 생활가전 렌탈 상담 접수용 원페이지.

- 운영 주소: https://mobile.4usquare.co.kr/
- 호스팅: GitHub Pages (`gosey2002/mobile`) — **게시 브랜치는 `gh-pages`**, 저장소 원본은 `main`
- DNS: 호스팅케이알 `mobile` CNAME → `gosey2002.github.io`
- 상담 접수: FormSubmit → realoio@naver.com (`?submitted=1` 완료 화면)
- 디자인: `4usquare.co.kr`, `fund.4usquare.co.kr`와 동일 토큰(네이비·스틸블루·세이지, Pretendard)

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
