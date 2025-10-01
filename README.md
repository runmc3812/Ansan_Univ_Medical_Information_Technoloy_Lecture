# 진료정보교류(HIE) 요약 — GitHub Pages

강의 자료 **[진료정보교류]**를 바탕으로 만든 한 페이지 요약(site). 학생 복습용으로 제작되었습니다.

## 파일
- `index.html` — 메인 페이지
- `style.css` — 스타일(인쇄 친화)

---

## GitHub Pages 배포 방법

### A. 웹 UI로 바로 배포
1. GitHub에서 **새 저장소** 생성 (Public 권장, 예: `hie-summary`).
2. 위 2개 파일(`index.html`, `style.css`)을 저장소 **루트**에 업로드 후 **Commit**.
3. 저장소 **Settings → Pages** 이동  
   - **Build and deployment** → **Source = Deploy from a branch**  
   - **Branch = `main` / Folder = `/ (root)`** 설정 → **Save**
4. 잠시 후 상단에 사이트 주소가 표시됩니다.  
   예: `https://<USER>.github.io/hie-summary/`

### B. 로컬에서 git으로 푸시
```bash
git clone https://github.com/<USER>/<REPO>.git
cd <REPO>

# 다운로드한 파일 2개를 이 폴더에 복사
git add .
git commit -m "Add HIE summary site"
git push origin main
# 이후 Settings → Pages에서 Source/Branch/Folder 설정
```

### C. QR 코드 만들기 (Chrome)
배포된 주소에서 주소창 **Share → QR code**를 선택해 PNG를 저장하고 슬라이드에 삽입하세요.

---

## 내용 수정
- `index.html`의 섹션 텍스트를 직접 편집하고 Commit하면 곧바로 반영됩니다.
- 퀴즈 페이지를 연결하려면 `/quiz/` 같은 하위 폴더에 별도 페이지를 추가하고 링크를 달면 됩니다.
