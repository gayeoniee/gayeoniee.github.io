# THUS FAR — thusfar.cloud

포트폴리오 첫 화면. **정적 HTML 한 장**이고 GitHub Pages 가 그대로 서빙한다 — 빌드도 프레임워크도 없다.

| 파일 | 역할 |
|---|---|
| `index.html` | 화면. 프로젝트 카드 4개는 이 파일 안의 `<article class="project-card">` 블록 — 링크·문구를 여기서 고친다 |
| `styles.css` | 스타일 (Next.js 버전의 `globals.css` + `status.css` 를 그대로 합침) |
| `CNAME` | 커스텀 도메인 `thusfar.cloud`. **지우면 도메인 연결이 풀린다** |

## 이 레포가 특별한 이유

이름이 `gayeoniee.github.io` 라서 GitHub 이 **사용자 사이트**로 취급한다. 여기 붙인 도메인은
다른 레포의 Pages 에도 자동으로 이어진다:

```
thusfar.cloud/                  ← 이 레포
thusfar.cloud/dog-care-agent/   ← gayeoniee/dog-care-agent 의 Pages (트레이스 뷰어)
```

## 로컬에서 보기

```bash
python -m http.server 8000     # http://localhost:8000
```

## DNS (도메인 등록처에서)

| 종류 | 이름 | 값 |
|---|---|---|
| A | `@` | 185.199.108.153 / 185.199.109.153 / 185.199.110.153 / 185.199.111.153 |
| CNAME | `www` | `gayeoniee.github.io` |

넣고 나면 Settings → Pages 에서 `Enforce HTTPS` 를 켠다 (인증서는 GitHub 이 발급한다).
