# cn-sh-2026 정리 구조

## 폴더 구조
- `docs/`: 일정/가이드 문서(Markdown)
- `maps/`: 지도 파일(HTML)
- `data/`: CSV 데이터(엑셀 열기용)
- `references/`: 참고 링크 원본

## 빠른 시작
1. 체력보존 상세 일정: `docs/shanghai_disney_2026-04-30_energy_save_detailed.md`
2. 실제 지도(온라인): `maps/shanghai_disney_2026-04-30_live_map.html`

## 부모님 폰에서 보기 (중요)
- `Git에 올리는 것`만으로는 오프라인 보장이 안 됩니다.
- 완전 오프라인으로 보려면 아래 파일을 폰에 직접 저장해야 합니다.
  - `docs/shanghai_disney_2026-04-30_one_day_plan.md` (텍스트)
  - `docs/shanghai_disney_2026-04-30_energy_save_detailed.md` (텍스트)
- `maps/shanghai_disney_2026-04-30_live_map.html`은 지도 타일 + Leaflet CDN이 필요해서 인터넷이 있어야 정상 동작합니다.

## Git 업로드 시 권장
- 그대로 저장소에 커밋 후 GitHub/GitLab에 업로드
- 온라인 보기: 브라우저에서 바로 가능
- 오프라인 보기: 폰에 파일 내려받아 열기

## 다음 개선 아이디어
- `offline_pack/` 폴더를 만들어 부모님용 파일만 복사
- Markdown 대신 PDF로 내보내서 열기 쉽게 통일
