# 설치 가이드

Craft to Exile 2 모드팩을 설치하는 방법을 안내합니다.

---

## 기본 요구사항

| 항목 | 요구사항 |
|------|----------|
| **마인크래프트 계정** | 유효한 Minecraft 계정 필요 (크랙 버전 미지원) |
| **Java** | Java 17 설치 필요 |
| **RAM** | 4-8GB 권장 |

---

## Java 성능 최적화 설정

런처의 JVM 인자(Arguments)에 다음 설정을 추가하면 성능이 향상됩니다:

```
-XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M
```

> **참고**: 기존 JVM 인자를 위 설정으로 대체하세요.

---

## 설치 방법

### 방법 1: CurseForge (가장 쉬운 방법)

1. [CurseForge 앱](https://www.curseforge.com/download/app) 다운로드 및 설치
2. 앱 실행 후 **Minecraft** 선택
3. 검색창에 **"Craft to Exile 2"** 입력
4. **Install** 클릭
5. 첫 실행 시 필요한 컴포넌트가 자동 설치됨

### 방법 2: Prism Launcher

1. [Prism Launcher](https://prismlauncher.org/) 다운로드 및 설치
2. Java 17 설정 확인
3. RAM 할당: **4096-8192 MB** 설정
4. **CurseForge** 탭에서 **"Craft to Exile 2"** 검색
5. 다운로드 및 설치
6. 차단된 모드가 있다면 Downloads 폴더에 저장

> **참고**: Prism Launcher는 오픈소스 런처로, 다양한 커스터마이징이 가능합니다.

### 방법 3: ATLauncher

1. [ATLauncher](https://atlauncher.com/) 다운로드 및 설치
2. Microsoft/Minecraft 계정으로 로그인
3. **Packs** → **CurseForge** 탭 이동
4. **"Craft to Exile 2"** 검색
5. 다운로드 클릭
6. 설치 중 모드 링크 열기가 필요할 수 있음 (수동 다운로드)

### 방법 4: GDLauncher

1. [GDLauncher](https://gdlauncher.com/) 다운로드 및 설치
2. 런처가 자동으로 Java 및 RAM 할당 (4-8GB)
3. **"Twitch"** 탭에서 **"Craft to Exile 2"** 검색
4. 설치 클릭
5. 완전 자동 설정으로 바로 플레이 가능

---

## RAM 할당 방법

각 런처에서 RAM을 할당하는 방법:

### CurseForge
1. 설정(Settings) → Minecraft
2. **Allocated Memory** 슬라이더 조정 (6-8GB 권장)

### Prism Launcher
1. 설정(Settings) → Java
2. **Maximum memory allocation** 설정

### ATLauncher
1. Settings → Java/Minecraft
2. **Maximum Memory/RAM** 조정

### GDLauncher
1. 인스턴스 우클릭 → Manage
2. Override Java Memory 체크
3. RAM 할당량 설정

---

## 설치 후 확인사항

1. **첫 실행**: 첫 실행 시 로딩 시간이 오래 걸릴 수 있습니다 (5-10분)
2. **셰이더 설정**: 기본적으로 셰이더가 꺼져 있습니다. Options → Video Settings → Shader Packs에서 활성화 가능
3. **키 설정 확인**: Controls에서 주요 키 바인딩 확인

---

## 문제 발생 시

설치 중 문제가 발생하면 [문제 해결 가이드](troubleshooting.md)를 참고하세요.

---

*[메인 페이지로 돌아가기](README.md)*
