# 셰이더 & 옵티파인 가이드

Craft to Exile 2에서 셰이더를 사용하고 그래픽 설정을 최적화하는 방법을 안내합니다.

---

## 셰이더 (Shaders)

### 기본 지원
이 모드팩에는 **Oculus** 모드가 포함되어 있어 별도 설치 없이 바로 셰이더를 사용할 수 있습니다.

### 기본 포함 셰이더

| 셰이더 이름 | 특징 |
|-------------|------|
| **Complementary Unbound** | 고품질 그래픽, 다양한 설정 옵션 |
| **Complementary Reimagined** | 최적화된 성능, 아름다운 조명 |

### 셰이더 활성화 방법

1. **Options** → **Video Settings** → **Shader Packs** 이동
2. 원하는 셰이더 선택
3. **Done** 클릭

### 추가 셰이더 설치

1. [Modrinth](https://modrinth.com/shaders) 또는 [CurseForge](https://www.curseforge.com/minecraft/search?class=shaders)에서 셰이더 다운로드
2. `.minecraft/shaderpacks` 폴더에 파일 추가
   - 런처에서 해당 폴더 열기: **Options** → **Resource Packs** → **Open Pack Folder** 후 상위 폴더로 이동
3. 게임 내 Shader Packs 메뉴에서 선택

### 권장 셰이더

| 셰이더 | 성능 | 설명 |
|--------|------|------|
| Complementary Reimagined | 중간 | 균형 잡힌 성능과 품질 |
| Complementary Unbound | 높음 | 최고 품질의 그래픽 |
| BSL Shaders | 중간 | 인기 있는 범용 셰이더 |
| Sildur's Vibrant | 낮음-중간 | 가벼운 셰이더 |

---

## 옵티파인 (Optifine)

### 사용 비권장

개발팀은 **옵티파인 설치를 권장하지 않습니다**.

### 비권장 이유

1. **렌더링 시스템 충돌**: 렌더링 시스템 개편으로 인해 블록과 아이템이 보이지 않을 수 있음
2. **게임 크래시 위험**: 다른 모드와의 호환성 문제로 크래시 발생 가능
3. **문제 진단 어려움**: 옵티파인이 설치된 경우 문제 원인 파악이 어려움

### 대체 솔루션

모드팩에는 이미 옵티파인의 주요 기능이 포함되어 있습니다:

| 기능 | 대체 모드 |
|------|-----------|
| 셰이더 | Oculus |
| FPS 카운터 | 기본 포함 |
| 그래픽 설정 | Embeddium/Rubidium |
| 성능 최적화 | 다수의 최적화 모드 |

> **참고**: 포함된 성능 최적화 모드들은 바닐라 및 옵티파인보다 빠른 성능을 제공합니다.

---

## 셰이더 성능 최적화

셰이더 사용 시 성능이 낮다면 다음 설정을 조정하세요:

### 셰이더 내부 설정

1. **Shader Options** 메뉴 열기
2. 다음 항목 조정:
   - **Shadow Quality**: 낮춤
   - **Shadow Distance**: 줄임
   - **Bloom**: 끄기
   - **Motion Blur**: 끄기
   - **Volumetric Lighting**: 끄기 또는 낮춤

### 게임 비디오 설정

| 설정 | 권장값 |
|------|--------|
| Render Distance | 8-10 청크 |
| Simulation Distance | 6-8 청크 |
| Graphics | Fast |
| Smooth Lighting | Minimum |
| Entity Shadows | Off |

---

## 일반적인 셰이더 문제

### 화면이 깜빡임
- 다른 셰이더로 변경
- 그래픽 드라이버 업데이트

### 블록 텍스처 오류
- 셰이더 설정에서 PBR 텍스처 끄기
- 다른 셰이더 시도

### 낮은 FPS
- 셰이더 품질 설정 낮추기
- 그림자 해상도 줄이기
- Render Distance 줄이기

---

*[메인 페이지로 돌아가기](README.md)*
