# 문제 해결 & 성능 최적화

Craft to Exile 2의 일반적인 문제 해결 방법과 성능 최적화 가이드입니다.

---

## 기본 문제 해결 단계

문제가 발생하면 먼저 다음 단계를 시도하세요:

1. **Java 17 재설치** - 최신 버전으로 재설치
2. **모드팩 복구** - 런처에서 모드팩 복구(Repair) 실행
3. **RAM 할당 확인** - 6-8GB RAM 할당
4. **모드팩 버전 확인** - 최신 버전인지 확인
5. **FPS Reducer 확인** - End 키로 FPS Reducer 설정 확인

---

## JVM 최적화 인자

다음 JVM 인자를 사용하여 성능을 향상시킬 수 있습니다:

```
-XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M
```

---

## 서버 & 연결 문제

### 레지스트리 동기화 오류
**증상**: "Incomplete set of tags received from server" 또는 레지스트리 동기화 실패

**원인**: 서버와 클라이언트의 버전이 다르거나 모드가 일치하지 않음

**해결**:
- 서버와 클라이언트 버전을 동일하게 맞추기
- 모드 목록 확인 및 동기화

### 무한 로딩
**증상**: 서버 접속 시 무한 로딩

**해결**:
1. 월드 폴더의 `serverconfigs` 디렉토리 이동
2. `curios-server.toml` 파일 삭제
3. 서버 재시작

### 연결 거부
**증상**: 서버 연결 실패

**해결**:
시작 인자에 다음 추가:
```
-Djava.net.preferIPv4Stack=true
```

### Watchdog 크래시
**증상**: "A single server tick took x seconds" 오류로 서버 크래시

**원인**: 극심한 렉으로 인한 워치독 타임아웃

**해결**:
1. `server.properties` 파일 열기
2. `max-tick-time` 값을 `-1`로 변경 (워치독 비활성화)

---

## GPU & 하드웨어 문제

### EXCEPTION_ACCESS_VIOLATION 오류
**원인**: GPU 드라이버 문제

**해결**:
1. 그래픽 드라이버 최신 버전으로 업데이트
2. 노트북의 경우 전용 GPU 사용 설정 확인
   - NVIDIA: NVIDIA 제어판 → 3D 설정 관리 → 고성능 NVIDIA 프로세서 선택
   - AMD: AMD 소프트웨어 → 게임 → 게임에 추가 후 고성능 설정

---

## 성능 진단 도구

### MCA Selector
- 손상된 청크 제거에 사용
- [다운로드](https://github.com/Querz/mcaselector)

### NBTExplorer
- 손상된 NBT 데이터 수정
- [다운로드](https://github.com/jaquadro/NBTExplorer)

### Observable
- 렉 유발 블록 시각화
- 200us/t 이상의 블록/엔티티 모니터링

---

## 성능 향상을 위한 모드 제거

다음 모드들은 멀티플레이어 호환성에 영향을 주지 않고 제거할 수 있습니다:

| 우선순위 | 모드 이름 | 효과 |
|----------|-----------|------|
| 높음 | AmbientSounds | 환경음 제거 |
| 높음 | Fallingleaves | 낙엽 효과 제거 |
| 높음 | SoundPhysics | 사운드 물리 효과 제거 |
| 중간 | Better Foliage | 나뭇잎 효과 제거 |

> **참고**: 이 모드들은 시각/청각 효과만 담당하므로 게임플레이에 영향 없음

---

## 일반적인 오류 메시지

### "Out of Memory"
- RAM 할당을 늘리세요 (6-8GB 권장)
- 다른 프로그램 종료

### "Ticking Entity"
- 특정 엔티티로 인한 크래시
- NBTExplorer로 해당 엔티티 제거

### "Ticking Block Entity"
- 특정 블록으로 인한 크래시
- MCA Selector로 해당 청크 제거 또는 수정

### 검은 화면 / 멈춤
- FPS Reducer 비활성화 (End 키)
- 풀스크린 대신 창 모드로 시도

---

## 추가 성능 팁

1. **청크 로딩 거리 줄이기**: Options → Video Settings → Render Distance (8-10 권장)
2. **파티클 줄이기**: Options → Video Settings → Particles (Minimal)
3. **엔티티 거리 줄이기**: Options → Video Settings → Entity Distance
4. **셰이더 비활성화**: 성능 문제 시 셰이더 끄기
5. **VSync 끄기**: 입력 지연 감소

---

## 도움 요청

위 방법으로 해결되지 않는 문제는:
- [공식 Discord](https://discord.gg/crafttoexile) 커뮤니티에서 도움 요청
- 크래시 로그 및 상세 정보 포함

---

*[메인 페이지로 돌아가기](README.md)*
