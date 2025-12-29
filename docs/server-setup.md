# 서버 설정 가이드

Craft to Exile 2 서버 설정, 업데이트, LAN 플레이, 관리 명령어에 대한 가이드입니다.

---

## 서버 호스팅 옵션

### 공식 서버
다음 공식 서버에서 바로 플레이할 수 있습니다:

| 서버 이름 | 주소 |
|-----------|------|
| Oriath | crafttoexile2-oriath.g.akliz.net |
| Wraeclast | crafttoexile2-wraeclast.g.akliz.net |
| Tristram | crafttoexile2-tristram.g.akliz.net |
| Harrogath | crafttoexile2-harrogath.g.akliz.net |
| POE Servers | poeservers.ddns.net:25566 |

### 상용 호스팅 서비스
Akliz와 같은 상용 호스팅 서비스를 이용하면 자동 설정이 가능합니다.

---

## 서버 요구사항

| 항목 | 요구사항 |
|------|----------|
| **RAM** | 최소 4-8GB 할당 권장 |
| **Java** | Java 17 64-bit |
| **자동 재시작** | 6시간마다 자동 재시작 권장 (성능 유지) |

> **중요**: 정기적인 재시작 없이는 성능 저하가 발생합니다.

---

## 개인 PC에서 서버 호스팅

### 설정 단계

1. **Java 17 64-bit 설치**
   - [Adoptium](https://adoptium.net/) 또는 [Oracle](https://www.oracle.com/java/technologies/downloads/)에서 다운로드

2. **서버 파일 추출**
   - CurseForge에서 서버 파일 다운로드
   - 원하는 폴더에 추출

3. **서버 실행**
   - Windows: `run.bat` 실행
   - Linux/Mac: `run.sh` 실행

4. **EULA 동의**
   - `eula.txt` 파일을 열고 `eula=false`를 `eula=true`로 변경

5. **명령 블록 활성화**
   - `server.properties`에서 `enable-command-block=true` 설정

6. **포트 포워딩**
   - 라우터에서 25565 포트 포워딩 설정
   - 외부 접속을 위해 필요

---

## LAN 플레이 (Essential 모드)

Essential 모드를 사용하면 서버 없이 친구와 함께 플레이할 수 있습니다.

### 설정 방법
1. Essential 모드가 이미 포함되어 있음
2. 게임 내에서 친구 추가
3. 월드 열기 → 친구 초대

---

## 상용 호스팅 설정

### 파일 관리
- FTP 클라이언트 사용: [FileZilla](https://filezilla-project.org/) 또는 [WinSCP](https://winscp.net/)
- 호스팅 서비스의 파일 관리자 사용

### 설정 업로드
1. FTP로 서버에 연결
2. 모드팩 파일 업로드
3. 서버 시작

---

## 서버 업데이트

### 업데이트 절차

1. **백업 생성** (중요!)
   - `world` 폴더 백업
   - `server.properties` 백업

2. **기존 폴더 삭제**
   다음 폴더들을 삭제합니다:
   - `config`
   - `defaultconfig`
   - `kubejs`
   - `mods`
   - `scripts`

3. **새 버전 복사**
   - 새 모드팩 버전에서 위 폴더들을 복사
   - 백업해둔 `server.properties` 복원

4. **서버 재시작**

---

## 관리자 명령어

### 기본 명령어

| 명령어 | 설명 |
|--------|------|
| `/flan bypass` | 클레임(점유) 영역 강제 진입 |
| `/spark profiler open` | 렉 원인 분석 도구 실행 |
| `/cu inventory read <플레이어>` | 플레이어 인벤토리 확인 |
| `/pregen start <반경>` | 월드 청크 미리 생성 |

### Crash Utilities (F12)
- 서버 성능 문제 진단
- 렉 유발 요소 확인

### Spark 프로파일러
- `/spark profiler` - 프로파일링 시작
- `/spark profiler open` - 결과 확인
- 성능 임계값을 통해 렉 원인 파악

---

## 성능 최적화 팁

1. **청크 미리 생성**: `/pregen` 명령어로 플레이 영역 청크를 미리 생성
2. **정기 재시작**: 6시간마다 자동 재시작 스크립트 설정
3. **플레이어 제한**: 서버 사양에 맞게 최대 플레이어 수 제한
4. **뷰 거리 조정**: `server.properties`에서 `view-distance` 조정 (8-10 권장)

---

## 문제 해결

서버 관련 문제가 발생하면 [문제 해결 가이드](troubleshooting.md)를 참고하세요.

---

*[메인 페이지로 돌아가기](README.md)*
