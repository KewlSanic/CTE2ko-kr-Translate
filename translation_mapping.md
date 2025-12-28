# CTE2 퀘스트 번역 매핑 문서

## 1. 파일 비교 현황

### 원본 경로
`C:\Users\1k0j2\curseforge\minecraft\Instances\Craft to Exile 2 (VR Support)\config\ftbquests\quests\chapters\`

### 번역 경로
`F:\workspace\MCP\KewlSanicCTE2\main_quest\`

### 번역 진행률: 21/22 (95.5%) - 거의 완료!

| 상태 | 영어 파일 | 한글 파일 | 영어 크기 | 한글 크기 | 비고 |
|------|-----------|-----------|-----------|-----------|------|
| ✅ | act_0.snbt | act_0.snbt | 32KB | 35KB | 프롤로그 - 완료 |
| ✅ | act_i.snbt | act_i.snbt | 65KB | 71KB | 1막 - 완료 |
| ✅ | act_ii.snbt | act_ii.snbt | 35KB | 38KB | 2막 - 완료 |
| ✅ | act_iii.snbt | act_iii.snbt | 38KB | 40KB | 3막 - 완료 |
| ✅ | act_iv.snbt | act_iv.snbt | 43KB | 43KB | 4막 - 완료 |
| ✅ | act_v.snbt | act_v.snbt | 33KB | 34KB | 5막 - 완료 |
| ✅ | ascendancy.snbt | ascendancy.snbt | 6.4KB | 6.8KB | 전직 - 완료 |
| ✅ | campaign_talent_rewards.snbt | campaign_talent_rewards.snbt | 36KB | 39KB | 캠페인 특성 보상 - 완료 |
| ✅ | completionist.snbt | completionist.snbt | 1.7KB | 1.8KB | 완벽주의자 - 완료 |
| ✅ | culinary_delights.snbt | culinary_delights.snbt | 36KB | 38KB | 요리 퀘스트 - 완료 |
| ✅ | epilogue.snbt | epilogue.snbt | 55KB | 55KB | 에필로그 - 완료 |
| ✅ | exploration.snbt | exploration.snbt | 23KB | 24KB | 탐험 - 완료 |
| ✅ | fishing.snbt | fishing.snbt | 33KB | 35KB | 낚시 - 완료 |
| ✅ | gem_shop.snbt | gem_shop.snbt | 8.9KB | 9.4KB | 보석 상점 - 완료 |
| ✅ | homestead.snbt | homestead.snbt | 29KB | 31KB | 정착지 - 완료 |
| ✅ | jolly_cooperation.snbt | jolly_cooperation.snbt | 24KB | 26KB | 즐거운 협동 - 완료 |
| ✅ | magical_flora.snbt | magical_flora.snbt | 65KB | 70KB | 마법 식물 - 완료 |
| ✅ | other_hobbies.snbt | other_hobbies.snbt | 35KB | 38KB | 기타 취미 - 완료 |
| ✅ | professions.snbt | professions.snbt | 32KB | 35KB | 전문 기술 - 완료 |
| ✅ | repeatables.snbt | repeatables.snbt | 9.4KB | 9.7KB | 반복 퀘스트 - 완료 |
| ✅ | storage_solutions.snbt | storage_solutions.snbt | 24KB | 26KB | 저장소 - 완료 |

---

## 2. 영어-한글 키워드 매핑

### 게임 시스템 용어

| 영어 | 한글 |
|------|------|
| Character Stats | 캐릭터 스탯 |
| Talent Tree | 특성 트리 |
| Talent point(s) | 특성 포인트 |
| Ascendancy | 전직 |
| Ascendancy Points | 전직 포인트 |
| Experience | 경험치 |
| Profession | 전문 기술 |
| Party Play | 파티 플레이 |
| Level | 레벨 |
| Stat points | 스탯 포인트 |

### 전직 관련

| 영어 | 한글 |
|------|------|
| Novice Ascendancy | 초보자 전직 |
| Cruel Ascendancy | 잔혹한 전직 |
| Merciless Ascendancy | 무자비한 전직 |

### UI/메뉴 용어

| 영어 | 한글 |
|------|------|
| Table of Contents | 목차 |
| Page 2 | 페이지 2 |
| Page 2b | 페이지 2-1 |
| Page 3 | 페이지 3 |
| Complete | 완료 |
| Craft | 제작 |

### 퀘스트 지시문

| 영어 | 한글 |
|------|------|
| Craft one of each item | 각 아이템을 하나씩 제작하세요 |
| Craft 3 Crab Pots | 게 덫 3개를 만들기 |
| Right click crops with hoe | 괭이를 든 상태에서 작물을 마우스 오른쪽 버튼 클릭 |
| Kill mobs to earn experience | 몬스터를 처치하여 경험치를 얻고 |
| Better Harvesting | 더 나은 수확 |

### 퀘스트 UI 용어

| 영어 | 한글 |
|------|------|
| Challenge | 도전 |
| Achievement | 업적 |
| Click Once Read | Click Once Read (유지) |
| Click here to brag | 클릭해서 자랑하기 |
| Money | 돈 |
| Experience x Lv. | 경험치 x Lv. |

### 번역하지 않는 용어 (영어 유지)

- 모드 이름: Mine and Slash, Farmer's Delight, Crabber's Delight, FTB Teams, Lightman's Currency, Lootr, Aquaculture, MIMI, Small Ships, Doggy Talents Next, Better Archeology, Gateways to Eternity, Alex's Mobs, Stardew Fishing
- 시스템 용어: Wiki, Discord, MIDI, ATM
- 퀘스트 고유 이름 (예: "Defenders of the Nether II")
- 아이템 ID, 커맨드, 리소스 경로

### 포맷팅 코드 (보존 필수)

| 코드 | 의미 |
|------|------|
| `&e` | 금색/노란색 |
| `&r` | 색상 초기화 |
| `&n` | 굵은 글씨 |
| `&c` | 빨간색 |
| `&9` | 파란색 (링크) |

---

## 3. SNBT 파일 구조

```
{
  filename: "quest_chapter"
  id: "unique_hex_id"
  group: "group_id"
  quests: [
    {
      id: "quest_id"
      title: "퀘스트 제목"           <- 번역 대상
      subtitle: "부제목"             <- 번역 대상
      description: [                  <- 번역 대상
        "설명 라인 1",
        "설명 라인 2"
      ]
      tasks: [...]
      rewards: [...]
    }
  ]
}
```

### 번역 대상 필드
- `title` - 퀘스트/태스크/보상 제목
- `subtitle` - 부제목
- `description` - 설명 (배열)

### 번역하지 않는 필드
- `id`, `filename`, `group` - 기술적 식별자
- `item`, `icon` - 리소스 경로
- `type`, `count`, `x`, `y` - 게임 메카닉
- `command`, `stat` - 시스템 명령

---

## 4. 번역 품질 가이드라인

1. **자연스러운 한국어 사용** - 직역 대신 의역
   - ❌ "몹들을 죽여서 경험치를 벌어라"
   - ✅ "몬스터를 처치하여 경험치를 얻으세요"

2. **일관된 용어 사용** - 위 키워드 매핑 참조

3. **포맷팅 코드 보존** - `&e`, `&r` 등 유지

4. **모드 이름 영어 유지** - Mine and Slash, FTB 등

5. **파일 크기 참고** - 한글 번역은 보통 5-10% 더 커짐

6. **과장된 말투 자제** - 담백하고 간결한 표현 사용

---

## 5. 번역 완료 기록

### 2024년 12월 완료 작업
- fishing.snbt (낚시) - Aquaculture, Stardew Fishing 콘텐츠
- jolly_cooperation.snbt (즐거운 협동) - Lightman's Currency, MIMI, Lootr 콘텐츠
- exploration.snbt (탐험) - 구조물 발견, Small Ships 콘텐츠
- other_hobbies.snbt (기타 취미) - 스니퍼, Better Archeology, Gateways, Doggy Talents 콘텐츠
- completionist.snbt (완벽주의자) - 최종 도전과제

### 검수 완료
- ✅ 기존 번역과 용어 일관성 확인
- ✅ 과장된 말투 검수 (문제 없음)
