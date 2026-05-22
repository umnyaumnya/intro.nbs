# 네이버 비즈니스 스쿨 정적 사이트

## GitHub Pages로 배포하는 방법

1. GitHub에서 새 저장소를 만듭니다.
   - 예: `naver-business-school-site`
   - 공개 저장소로 생성하세요.

2. 터미널에서 프로젝트 폴더로 이동합니다.

```bash
cd /Users/user/Desktop/dawoon_github/naver-business-school-site
```

3. Git 초기화 및 커밋을 합니다.

```bash
git init
git add index.html
# 필요하면 추가 파일도 git add .
git commit -m "Add GitHub Pages site"
```

4. GitHub 원격 저장소를 연결합니다.

```bash
git branch -M main
git remote add origin https://github.com/<username>/naver-business-school-site.git
git push -u origin main
```

5. GitHub 저장소 설정에서 Pages를 활성화합니다.
   - `Settings` > `Pages` 또는 `Pages` 탭으로 이동
   - `Source`를 `main` 브랜치, `root`로 설정
   - 저장하면 배포 URL이 표시됩니다.

6. 배포가 완료되면 공유 가능한 링크가 생성됩니다.
   - 예: `https://<username>.github.io/naver-business-school-site/`

## 로컬에서 미리 보기

```bash
python3 -m http.server 8000
```

그런 다음 브라우저에서 `http://localhost:8000`로 열어 확인할 수 있습니다.

---

## 추가 옵션

- `index.html` 외에 스타일을 분리하려면 `styles.css`를 만들고 `<link>`로 연결하세요.
- 여러 페이지를 만들려면 추가 HTML 파일과 링크를 추가하면 됩니다.
