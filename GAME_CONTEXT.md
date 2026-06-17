# 게임 개발 컨텍스트

> **Claude에게**: 이 파일을 먼저 읽고 프로젝트 상태를 파악하세요. 작업 후에는 변경사항을 이 파일에 업데이트하세요.

---

## 개발 환경

- **메인 작업**: Windows Desktop (MSW Maker + Git)
- **외부 작업**: MacBook (코딩 전용)
- **동기화**: GitHub (`https://github.com/Byoengmen/Make_Game_Maple_World_MGMW`)
- **플랫폼**: MapleStory Worlds (MSW), mLua 스크립트

### Git 작업 흐름
```
작업 후 저장: git add . && git commit -m "내용" && git push
다른 기기에서 받기: git pull
```

---

## 현재 프로젝트 구조

```
RootDesk/MyDesk/
  Monster.mlua       - 몬스터 HP/피격/사망/리스폰 컴포넌트
  MonsterAttack.mlua - 몬스터 공격 컴포넌트
  PlayerAttack.mlua  - 플레이어 공격 (데미지 50, 치명타 30% / 2배)
  PlayerHit.mlua     - 플레이어 피격 (무적시간 1초)
  UIPopup.mlua       - 확인/취소 팝업 (트윈 애니메이션)
  UIToast.mlua       - 토스트 메시지 (페이드 인/아웃)

map/map01.map        - 메인 맵 (MapleTile 사이드뷰)
ui/
  DefaultGroup.ui    - 기본 HUD
  PopupGroup.ui      - 팝업 UI
  ToastGroup.ui      - 토스트 UI
```

---

## 구현된 기능

- [x] 몬스터 HP / 피격 / 사망 / 리스폰 시스템
- [x] 플레이어 공격 (근접, BoxShape)
- [x] 플레이어 피격 무적시간
- [x] UI 팝업 / 토스트 메시지

---

## 미구현 / 예정 기능

> 작업하면서 이 목록을 업데이트하세요.

- [ ] (게임 방향 미정 - 사용자와 논의 필요)

---

## 주요 결정사항 / 메모

- 맵 타입: MapleTile (TileMapMode = 0), 사이드뷰 플랫포머
- 플레이어 기본 데미지: 50, 치명타 확률 30%, 치명타 배율 2x
- 몬스터 기본 HP: 100, 리스폰 딜레이: 5초

---

## 마지막 작업 (업데이트 필요)

- 날짜: 2026-06-17
- 작업 내용: 개발환경 구축 (GitHub 연동), 기존 코드 파악
- 다음 할 일: 게임 방향 결정 후 개발 시작
