# 모드팩 수정 가이드

Craft to Exile 2의 다양한 설정을 커스터마이징하는 방법을 안내합니다.

---

## HUD 위치 조정

### Mine & Slash 바 위치 변경

Mine & Slash 바(체력, 마나, 에너지 바)의 위치를 변경할 수 있습니다.

**설정 방법**:
1. **Options** → **Mod Options** 이동
2. **Mine & Slash** 선택
3. **HUD Position** 옵션에서 선택:
   - **Bottom Center**: 화면 하단 중앙
   - **Over Vanilla**: 바닐라 UI 위에 표시
   - 기타 옵션

### Combat Roll 아이콘 위치

Combat Roll 아이콘은 드래그로 위치 변경이 가능합니다.

1. 게임 플레이 중 해당 아이콘에 마우스 커서 이동
2. 드래그하여 원하는 위치로 이동

### Inventory HUD+ 구성

Inventory HUD+ 모드의 각 구성 요소를 개별적으로 위치 변경할 수 있습니다.

1. **Options** → **Mod Options** → **Inventory HUD+**
2. 각 구성 요소(갑옷, 아이템, 상태 효과 등) 위치 개별 설정

---

## 음악 변경

### 바닐라 음악으로 변경하기

모드팩의 커스텀 음악 대신 바닐라 마인크래프트 음악을 사용하려면:

1. **바닐라 음악 리소스팩** 다운로드
2. 다음 경로로 파일 복사:
   ```
   .minecraft/config/openloader/resources
   ```
3. 기존 음악 리소스팩을 덮어쓰기
4. 게임 재시작

---

## 모드 제거

### 몹 파밍 제한 제거

몹 파밍 제한 기능을 원하지 않는 경우:

1. `/mods/` 폴더 이동
2. 관련 jar 파일 삭제 (파일명 확인 필요)
3. 게임 재시작

> **주의**: 멀티플레이어에서는 서버와 클라이언트 모두에서 동일하게 제거해야 합니다.

### 비활성화된 아이템 다시 활성화

일부 아이템이 의도적으로 비활성화되어 있습니다. 다시 활성화하려면:

1. 다음 파일 열기:
   ```
   scripts/disabled.zs
   ```
   또는
   ```
   kubejs/scripts/disabled.js
   ```
2. 해당 아이템 관련 줄을 주석 처리하거나 삭제
3. 게임 재시작 또는 `/reload` 명령어 실행

---

## 데이터팩 커스터마이징

### 데이터팩 위치

Mine & Slash 관련 데이터팩은 다음 경로에 있습니다:

```
configs/openloader/data/cte_mns
```

### 수정 가능한 항목

| 항목 | 설명 |
|------|------|
| **통계** | 아이템/몹 스탯 조정 |
| **아이템** | 아이템 속성 변경 |
| **드롭률** | 드롭 확률 조정 |
| **밸런스** | 전체적인 게임 밸런스 |

### 데이터팩 수정 방법

1. 해당 폴더의 JSON 파일 열기
2. 원하는 값 수정
3. 게임 재시작 또는 `/reload`

> **팁**: 수정 전 원본 파일을 백업해두세요.

---

## 키 바인딩 변경

### Mine & Slash 키 바인딩

1. **Options** → **Controls** → **Key Binds**
2. **Mine & Slash** 카테고리 찾기
3. 원하는 키로 변경

### 주요 기본 키

| 기능 | 기본 키 |
|------|---------|
| 스킬 메뉴 | K |
| 특성 메뉴 | N |
| 허브 메뉴 | H |
| 분해 메뉴 | G |

---

## 난이도 조정

### 월드 생성 시 설정

1. 월드 생성 화면에서 **More World Options**
2. 난이도 관련 설정 조정

### 게임 중 설정

일부 난이도 설정은 게임 중에도 변경 가능:
- `/difficulty` 명령어 사용
- Mod Options에서 Mine & Slash 난이도 스케일링 조정

---

## 그래픽 설정 최적화

### 권장 설정 (성능 중심)

| 설정 | 권장값 |
|------|--------|
| Render Distance | 8 청크 |
| Simulation Distance | 6 청크 |
| Graphics | Fast |
| Particles | Minimal |
| Entity Distance | 75% |
| Smooth Lighting | Off |

### 권장 설정 (품질 중심)

| 설정 | 권장값 |
|------|--------|
| Render Distance | 12-16 청크 |
| Simulation Distance | 8-10 청크 |
| Graphics | Fancy |
| Particles | All |
| Entity Distance | 100% |
| Smooth Lighting | Maximum |

---

## 설정 파일 직접 편집

### 설정 파일 위치

| 모드 | 파일 경로 |
|------|-----------|
| Mine & Slash | `config/minesandslash-common.toml` |
| Curios | `config/curios-common.toml` |
| 일반 설정 | `options.txt` |

### 편집 시 주의사항

1. 게임 종료 상태에서 편집
2. 수정 전 파일 백업
3. 올바른 형식 유지 (TOML, JSON 등)

---

## 추가 리소스

- [공식 Discord](https://discord.gg/crafttoexile) - 커스터마이징 관련 질문
- [CurseForge 페이지](https://www.curseforge.com/minecraft/modpacks/craft-to-exile-2) - 최신 업데이트 확인

---

*[메인 페이지로 돌아가기](README.md)*
