# 교과학점제 과목 안내

과목을 검색·필터로 살펴보고, 관심 과목을 담아 이수 학점을 미리 계산해 보는 정적 웹페이지입니다.

## GitHub Pages로 배포하기

1. GitHub에서 새 저장소(Repository)를 만듭니다. (예: `course-guide`)
2. 이 폴더의 파일(`index.html`, `README.md`, `.nojekyll`)을 저장소 최상위에 올립니다.
   - 웹에서: **Add file → Upload files** 로 끌어다 놓고 **Commit changes**
3. 저장소의 **Settings → Pages** 로 이동합니다.
4. **Build and deployment → Source** 를 `Deploy from a branch` 로 선택합니다.
5. Branch를 `main`, 폴더를 `/ (root)` 로 지정하고 **Save** 를 누릅니다.
6. 1~2분 뒤 아래 주소로 접속할 수 있습니다.

   `https://<GitHub아이디>.github.io/<저장소이름>/`

## 과목 데이터 수정

`index.html` 안의 `COURSES` 배열을 학교 교육과정 편성표에 맞게 수정하세요.

| 항목 | 의미 |
|------|------|
| n | 과목명 |
| t | 유형 (공통 / 일반선택 / 진로선택 / 융합선택) |
| g, s | 개설 학년, 학기 |
| c | 학점 |
| tr | 추천 진로 계열 |
| d | 과목 설명 |

수정 후 GitHub에서 파일을 다시 커밋하면 자동으로 반영됩니다.
