# 니끌로

아이폰용 사진 필터·보정 웹앱 — 단일 `index.html`, 의존성·빌드 없음.
홈 화면 아이콘: `icon.png` (원본 디자인 `icon.svg`, 수정 후 `qlmanage -t -s 180 -o . icon.svg`로 재생성)

- 인스타 스타일 필터 5종 (Clarendon·Gingham·Juno·Lark·Valencia)
- 밝기·대비·채도·선명하게 슬라이더, crop (자유·1:1·4:5·16:9)
- 여러 장 일괄 적용 (crop 제외)
- JPG 변환 후 공유시트로 사진 앱 저장 (HEIC는 iOS가 선택 시 자동 JPEG 변환)

## GitHub Pages 배포 (웹 UI만으로 가능)

1. github.com → New repository → 이름 `photo-filter`, Public으로 생성
2. "uploading an existing file" 링크로 `index.html`과 `icon.png` 업로드 → Commit
3. Settings → Pages → Branch: `main`, `/ (root)` → Save
4. 1~2분 후 `https://{계정}.github.io/photo-filter/` 접속 — 이 링크를 지인에게 공유

수정 후에는 같은 방법으로 `index.html`을 다시 업로드하면 됨.

설계 문서: `docs/superpowers/specs/2026-07-04-photo-filter-design.md`
