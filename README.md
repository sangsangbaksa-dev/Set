# Set — 공용 소품(props)

Project Harbor(sangsangbaksa-dev/GTA-)와 이후 합칠 게임이 같이 쓰는 소품 모델. 전투 커버용 위주.

| 파일 | 용도 |
|---|---|
| `props/prop_crate_wood.glb` | 나무 상자 1.2m — 하이 커버 |
| `props/prop_barrel_explosive.glb` | 빨간 드럼통 — 폭발물 |
| `props/prop_concrete_barrier.glb` | 콘크리트 바리케이드 2m — 로우 커버 |
| `props/prop_sandbag_wall.glb` | 모래주머니 벽 — 로우 커버 |
| `props/prop_dumpster.glb` | 대형 쓰레기통 — 하이 커버 |
| `props/prop_ammo_box.glb` | 탄약 상자 — 픽업 |
| `props/prop_traffic_cone.glb` | 라바콘 — 장식 |

- 생성: GTA- 리포의 `tools/blender/build_assets.py` (블렌더 헤드리스). 손으로 고치지 말고 스크립트 수정 후 재생성:
  `blender -b --factory-startup -P tools/blender/build_assets.py -- --only props --props-out ../set/props`
- 규칙: 1단위 = 1m, 바닥 중심 원점, 정면 -Y(Blender). 메시 이름 `-col` → Godot가 충돌 생성.
- 오리지널 디자인만. 미리보기: `preview_props.png`.
