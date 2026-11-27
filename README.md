# Set — 공용 3D 모델

Project Harbor(sangsangbaksa-dev/GTA-)와 이후 합칠 게임이 같이 쓰는 소품 **46종**, 차량 **1종**, 인물 **5종**, 주인공 모션 **9종**. 소품은 전투 커버, 경제 상호작용, 항구 시설을 포함한다.

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
| `prop_dock_power_pedestal` | 항구 | `decor` | 부두 전원함 |
| `prop_dock_access_gate` | 항구 | `decor` | 부두 출입문 — 닫힌 고정형 |
| `prop_dock_safety_rail` | 항구 | `decor` | 부두 안전 난간 |
| `prop_mooring_fender` | 항구 | `cover_low` | 접안용 고무 방충재 |
| `prop_loading_ramp` | 항구 | `decor` | 강철 하역 경사판 |
| `prop_dock_cargo_net` | 항구 | `cover_low` | 그물로 고정한 팔레트 화물 |
| `prop_harbor_gantry_crane` | 항구 | `decor` | 부두 갠트리 크레인 — 하부 통행 가능 |
| `prop_harbor_pilot_tug` | 항구 | `decor` | 부두 작업선 — 원점은 수선, 선수는 Blender -Y / glTF +Z |
| `prop_dock_inspection_terminal` | 항구 | `decor` | 부두 점검 단말기 — 화면 및 점검 위치 마커 포함 |
| `prop_harbor_beacon` | 항구 | `decor` | 항만 등대 — 프레넬 렌즈와 등화 마커 포함 |

`props/manifest.json`에서 모델 경로와 게임플레이 태그를 확인할 수 있다. Harbor의 `data/props/props.json`과 같은 목록이다.

## 차량

| 파일 | 설명 |
|---|---|
| `vehicles/veh_calloway_compact.glb` | Calloway Pip 소형차. 차체와 네 바퀴 피벗을 포함한다. |

차량 원점은 지면 중심이고 glTF에서 전방은 +Z, 위쪽은 +Y다. `WheelFL`과 `WheelFR`은 로컬 Y축으로 조향하고 각 바퀴의 `Roll` 자식 노드는 로컬 X축으로 구른다.

Harbor 리포에서 차량을 재생성한다.

```bash
blender -b --factory-startup -P tools/blender/build_vehicles.py -- --out ../set/vehicles
```

## Harbor Front 인물

![Harbor Front 인물 얼굴과 전신](previews/harbor_people.png)

| 모델 | 역할과 디자인 |
|---|---|
| `characters/chr_harbor_clerk.glb` | 토마스 레예스. 화물 서기이자 주인공. 스킨드 메시에 Mixamo 클립 9종이 들어 있다 |
| `characters/chr_harbor_rook.glb` | 룩. 바랜 청록 작업 재킷과 캔버스 슬링을 멘 배달원 |
| `characters/chr_harbor_officer.glb` | 마라 베일. 남색 근무복, 모자와 방파제 배지를 착용한 항만 경찰 |
| `characters/chr_harbor_crew.glb` | 니코 보스. 넓은 체형, 짧은 머리와 턱수염, 적갈색 조끼를 입은 라이벌 크루 |
| `characters/chr_harbor_dockhand.glb` | 아마라 콜. 작업복, 반사 조끼와 헤드램프를 착용한 항만 전기 기술자 |

각 GLB는 하나의 스킨드 메시와 공용 51본 골격을 포함한다. 원점은 발밑이고 앞쪽은 glTF +Z다. [Harbor 생성 스크립트](https://github.com/sangsangbaksa-dev/GTA-/blob/main/tools/blender/harbor_people.py)

```bash
blender -b --factory-startup -P tools/blender/build_assets.py -- --out ../set --only harbor_people
```

## 주인공 모션

클립은 토마스 레예스(`characters/chr_harbor_clerk.glb`)에 붙어 재생한다. 같은 9종이 그 GLB의 NLA 트랙으로도 들어 있다. `motions/`의 파일은 메시 없이 공용 51본 아마추어만 담는다. `motions/harbor_mixamo_motions.glb`는 9종을 한 파일에 묶은 것이고, 나머지는 클립마다 하나다.

30 FPS이고 발은 glTF `Y = 0`에 붙는다. 걷기·조깅·달리기·웅크린 걷기는 제자리 루프다. 좌우 회전은 누적 요를 빼 컨트롤러가 방향을 돌린다.

| 파일 (`motions/<id>.glb`) | 클립 | 용도 |
|---|---|---|
| `mixamo_idle` | `Idle` | 제자리 호흡 대기 |
| `mixamo_walk` | `Walk` | 제자리 걷기 |
| `mixamo_jog` | `Jog` | 제자리 조깅 |
| `mixamo_run` | `Run` | 제자리 달리기 |
| `mixamo_turn_left` | `TurnLeft` | 제자리 좌회전 |
| `mixamo_turn_right` | `TurnRight` | 제자리 우회전 |
| `mixamo_dance` | `Dance` | 브루클린 업록 |
| `mixamo_crouch_idle` | `CrouchIdle` | 웅크린 대기 |
| `mixamo_crouch_walk` | `CrouchWalk` | 제자리 웅크린 걷기 |

`motions/manifest.json`에서 클립 이름, 프레임 수, 경로를 확인할 수 있다. Harbor의 `tools/blender/mixamo_mocap.py`가 이 51본 리그로 리타겟한다.

## 규칙
- 생성: GTA- 리포 `tools/blender/build_props.py` (블렌더 4.2 헤드리스). **.glb를 손으로 고치지 말고** 스크립트 수정 후 재생성:
  `blender -b --factory-startup -P tools/blender/build_props.py -- --out ../set/props --manifest ../set/props/manifest.json`
- 1단위 = 1m, 바닥 중심 원점, 정면 -Y(Blender) → glTF에선 +Z. 작업선 원점은 수선 중앙에 있다.
- 충돌: 시각 메시와 별개인 단순한 `*-colonly` 메시를 Godot이 정적 충돌체로 가져온다.
- 빈 오브젝트(empty) 마커: `interact`(상호작용 지점), `loot_socket`, `light`, `sit`, `door_interact`.
- Godot 임포트 시 LOD가 자동 생성된다. 일반 소품은 시각 메시를 6천 삼각형 이하로 유지한다.
- 오리지널 디자인만. 실존 브랜드·로고 금지.
