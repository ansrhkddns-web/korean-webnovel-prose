# korean-webnovel-prose

한국 상업 웹소설 원고를 작성, 수정, 진단하기 위한 Codex 스킬입니다.  
문체, 문장 길이, 줄바꿈, 대화체, 묘사 방식, 상태창/카톡 표기, 회차 훅, 장르별 보상 루프를 하나의 일관된 작업 방식으로 묶습니다.

## 목표

- 모바일에서 읽기 쉬운 한국 웹소설 문장과 문단 호흡을 유지합니다.
- 학생, 어른, 빌런, 계산형 인물, 코믹 인물의 말투를 구분합니다.
- 던전/헌터, 아포칼립스, 게임/탑, 무협, 현대 직업물, 학교/아카데미, 판타지/영지물의 장르 보상 구조를 반영합니다.
- 회차마다 압박, 선택, 보상, 새 압박이 생기도록 설계합니다.
- 네이버 연재 원고에 맞는 상태창, 메모, 카톡, 문자 표기를 유지합니다.
- 특정 작가의 문장을 모방하지 않고, 장르 작동 원리와 품질 규칙만 사용합니다.

## 설치

Codex 스킬 폴더에 이 저장소를 복사하거나, 스킬 설치 기능에서 이 GitHub 저장소를 지정합니다.

기본 위치 예시:

```text
C:\Users\<USER>\.codex\skills\korean-webnovel-prose
```

필수 파일:

```text
korean-webnovel-prose/
├─ SKILL.md
├─ agents/
│  └─ openai.yaml
└─ references/
   ├─ style-system.md
   ├─ dialogue-voice.md
   ├─ description-engine.md
   ├─ genre-persona.md
   ├─ episode-engine.md
   ├─ naver-format.md
   └─ revision-rubric.md
```

## 사용 예시

```text
$korean-webnovel-prose 35화 초안을 써줘. 던전 비중을 높이고 학생 대사는 평범하게 해줘.
```

```text
$korean-webnovel-prose 이 장면 문체를 네이버 웹소설처럼 가볍고 읽기 좋게 고쳐줘.
```

```text
$korean-webnovel-prose 대화가 너무 책처럼 느껴져. 학생 말투로 자연스럽게 바꿔줘.
```

```text
$korean-webnovel-prose 상태창, 메모, 카톡 표기 규칙을 지키면서 업로드 전 원고를 점검해줘.
```

## 핵심 규칙

- 일반 서술은 완성문 중심의 2-4문장 문단으로 씁니다.
- 이동, 준비물, 관찰, 방향을 단어 단위로 끊어 쓰지 않습니다.
- 대사는 관계, 압박, 정보, 지위, 욕망 중 하나를 움직여야 합니다.
- 묘사는 분위기가 아니라 행동, 위험, 보상, 감정, 공간 이해를 돕는 용도로 씁니다.
- 설명은 독자가 알고 싶어진 뒤에 넣습니다.
- 회차 끝에는 다음 화를 누르게 만드는 구체적인 물체나 변화가 있어야 합니다.

## 네이버 원고 표기

상태창:

```text
《상태 정보 : 유진혁》
- 근육 0.6212
- 신경 0.5868
- 세포 0.6461
```

메모/파일명:

```text
[계단/언덕: 이전보다 덜 힘듦]
[상담실_백서진_협박프레임]
```

카톡/문자:

```text
〈김도윤〉 원본 옮길 수 있음.
〈단톡방〉 와 진짜 피곤하다.
```

본문에서는 백틱 사용을 피합니다.

## 레퍼런스 설계

`SKILL.md`는 가볍게 유지하고, 실제 세부 규칙은 `references/` 아래에 분리했습니다.

- `style-system.md`: 문체, 문단, 내면 독백, 스타일 통일
- `dialogue-voice.md`: 말투, 대화체, 카톡/단톡, 대사 수정
- `description-engine.md`: 감각, 공간, 위협, 아이템, 전투, 감정 묘사
- `genre-persona.md`: 장르별 보상과 작가 페르소나
- `episode-engine.md`: 회차 구조, 보상, 훅, 다음 화 클릭 이유
- `naver-format.md`: 네이버 원고 표기 규칙
- `revision-rubric.md`: 수정 단계와 진단 체크리스트

## 검증

스킬 유효성 검사는 Codex의 `quick_validate.py`로 수행할 수 있습니다.

```powershell
python -X utf8 "$env:USERPROFILE\.codex\skills\.system\skill-creator\scripts\quick_validate.py" "C:\Users\<USER>\.codex\skills\korean-webnovel-prose"
```

## 저작권 원칙

이 스킬은 레퍼런스 작품의 원문을 저장하거나 복제하지 않습니다.  
작품별 고유 문장, 고유 설정, 고유 농담을 따라 하지 않고, 상업 웹소설 작법의 일반화된 패턴만 사용합니다.
