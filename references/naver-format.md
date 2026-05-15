# Naver Manuscript Format

## Purpose

Use this file for 네이버 연재 원고 표기, 상태창, 메모, 카톡, 문자, 단톡방, 파일명, and upload-safe manuscript cleanup.

## General Rule

Avoid backticks in story manuscripts unless the user explicitly wants code-like formatting. Backticks read like programming notation and can break immersion.

## Status / System Blocks

Use `《》` for status, system, warning, skill, item, quest, and readout blocks. Put every entry on its own bullet line and do not add empty lines between entries.

```text
《상태 정보 : 유진혁》
- 근육 0.6212
- 신경 0.5868
- 세포 0.6461
- 지능 0.9360
- 감각 0.7090
- 의지 0.5039
```

```text
《상태 정보 재호출》
- 조건: 최근 인과 기록 회상
- 정확도: 낮음
```

After the block, add body feedback, desire, anxiety, or next action.

## Memo / Written Record

Use square brackets for notes, filenames, folder names, labels, written marks, phone memo content, notebook entries, and short record-like text created by a character.

```text
[계단/언덕: 이전보다 덜 힘듦]
[목표: 입구 근처 표시, 발소리/냄새 기록]
[상담실_백서진_협박프레임]
```

## KakaoTalk / SMS / Group Chat

Use angle brackets for chat, SMS, group chat, unknown number, and video captions.

```text
〈김도윤〉 원본 옮길 수 있음.
〈유진혁〉 내일.
〈모르는 번호〉 너 오늘 봤지?
〈단톡방〉 와 진짜 피곤하다.
〈영상 자막〉 강도현 지시 녹음 원본
```

Do not wrap these in quotation marks. Keep them short and dry.

## Speech / Recording

Use ordinary dialogue quotation marks for spoken lines and recorded speech:

```text
“너 지금 그 말 책임질 수 있어?”
```

## Sound And Hard Beats

Use standalone sound lines sparingly.

```text
쿵.
```

Do not overuse sound effects as substitutes for action consequences.

## Upload Cleanup

Before finalizing a Naver-ready manuscript:

- Search for leftover backticks.
- Normalize status blocks to `《》`.
- Normalize memo/file/written records to `[]`.
- Normalize chat/SMS/group messages to `〈〉`.
- Remove excessive blank lines inside system or chat blocks.
- Confirm the title line is separate from the manuscript body if upload requires it.
