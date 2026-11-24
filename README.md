# Set — 공용 소품(props)

Project Harbor(sangsangbaksa-dev/GTA-)와 이후 합칠 게임이 같이 쓰는 소품 모델 **36종**. 전투(커버)·경제(상호작용) 중심.

![cover](previews/cover.png)
![large](previews/large.png)
![loot](previews/loot.png)
![economy & street](previews/economy_street.png)

| 파일 (`props/<id>.glb`) | 분류 | 게임플레이 태그 | 용도 |
|---|---|---|---|
| `prop_crate_wood` | 커버·지형 | `cover_high` | 나무 상자 1.2m — 하이 커버, 파괴 가능 |
| `prop_crate_stack` | 커버·지형 | `cover_high` | 상자 더미 — 하이 커버, 올라설 수 있음 |
| `prop_barrel_explosive` | 커버·지형 | `explosive` | 빨간 드럼통 — 사격 시 폭발 |
| `prop_barrel_oil` | 커버·지형 | `cover_low` | 파란 드럼통 — 로우 커버, 관통됨 |
| `prop_concrete_barrier` | 커버·지형 | `cover_low` | 저지형 콘크리트 방호벽 2m — 로우 커버, 관통 불가 |
| `prop_sandbag_wall` | 커버·지형 | `cover_low` | 모래주머니 호형 벽 — 로우 커버 |
| `prop_dumpster` | 커버·지형 | `cover_high` | 대형 쓰레기통 — 하이 커버, 밀 수 있음 |
| `prop_shipping_container` | 커버·지형 | `cover_full` | 20피트 선적 컨테이너 — 벽, 문 열림 |
| `prop_pallet_stack` | 커버·지형 | `cover_high` | 랩 감은 팔레트 화물 — 하이 커버 |
| `prop_gas_cylinder_cage` | 커버·지형 | `explosive` | 가스통 보관함 — 연쇄 폭발 |
| `prop_cable_spool` | 커버·지형 | `cover_high` | 케이블 드럼 — 하이 커버, 굴릴 수 있음 |
| `prop_scaffold_section` | 커버·지형 | `vantage` | 비계 한 칸 — 고지대 포지션 |
| `prop_ammo_box` | 픽업 | `pickup_ammo` | 탄약 상자 — 탄약 보급 |
| `prop_medkit` | 픽업 | `pickup_health` | 구급 상자 — 체력 회복 |
| `prop_armor_vest` | 픽업 | `pickup_armor` | 방탄 조끼 — 방어구 충전 |
| `prop_cash_bag` | 전리품 | `loot_carry` | 현금 가방 — 습격 전리품, 들고 뛰면 느려짐 |
| `prop_cash_stack` | 전리품 | `loot_small` | 현금 다발 — 즉시 획득 |
| `prop_bond_case` | 전리품 | `loot_carry` | 채권 서류가방 — 고가 전리품 |
| `prop_weapon_crate` | 전리품 | `supply_drop` | 무기 보급 상자 — 공중 보급/이벤트 |
| `prop_atm` | 경제·상호작용 | `atm` | ATM — 입출금, 해킹 대상 |
| `prop_vending_machine` | 경제·상호작용 | `shop_small` | 자판기 — 소모품 구매 |
| `prop_cash_register` | 경제·상호작용 | `register` | 계산대 — 상점 강도 대상 |
| `prop_safe` | 경제·상호작용 | `safe` | 금고 — 습격 목표, 드릴/다이얼 |
| `prop_workbench` | 경제·상호작용 | `workbench` | 작업대 — 무기 개조 |
| `prop_laptop_hack` | 경제·상호작용 | `hack_terminal` | 해킹 노트북 — 습격 준비 미션 |
| `prop_traffic_cone` | 거리 | `decor_physics` | 라바콘 — 물리 소품 |
| `prop_street_lamp` | 거리 | `decor_light` | 가로등 5.6m — 조명 |
| `prop_fire_hydrant` | 거리 | `decor_breakable` | 소화전 — 차로 치면 물 분출 |
| `prop_bench` | 거리 | `decor_sit` | 공원 벤치 — 앉기 |
| `prop_trash_bin` | 거리 | `decor_physics` | 가로 쓰레기통 |
| `prop_bus_shelter` | 거리 | `cover_high` | 버스 정류장 — 유리 파괴 |
| `prop_parking_meter` | 거리 | `decor_breakable` | 주차 미터기 — 부수면 잔돈 |
| `prop_newspaper_box` | 거리 | `cover_low` | 신문 가판함 — 로우 커버 |
| `prop_dock_bollard` | 항구 | `cover_low` | 부두 계류주 — 로우 커버 |
| `prop_life_ring_stand` | 항구 | `decor` | 구명환 거치대 |
| `prop_road_barricade` | 거리 | `decor_physics` | 도로 바리케이드 — 경찰 검문 |

`props/manifest.json` = 위 표의 기계용 버전. 게임은 `tag`로 동작을 붙인다 (Harbor `data/props/` 참조).

## 규칙
- 생성: GTA- 리포 `tools/blender/build_props.py` (블렌더 4.2 헤드리스). **.glb를 손으로 고치지 말고** 스크립트 수정 후 재생성:
  `blender -b --factory-startup -P tools/blender/build_props.py -- --out ../set/props --manifest ../set/props/manifest.json`
- 1단위 = 1m, 바닥 중심 원점, 정면 -Y(Blender) → glTF에선 +Z.
- 충돌: 시각 메시와 별개인 단순 박스/원기둥 `*-colonly` 메시 → Godot이 정적 충돌체로 만들고 화면엔 안 그림.
- 빈 오브젝트(empty) 마커: `interact`(상호작용 지점), `loot_socket`, `light`, `sit`, `door_interact`.
- LOD는 Godot 임포트가 자동 생성. 시각 메시는 6k 트라이 이하.
- 오리지널 디자인만. 실존 브랜드·로고 금지.
