```text
SEPIA REVIEW — 릴리스 노트, 저장소 미상 (원문만 주어짐)
Loaded: SKILL.md, references/professional-pass.md, references/domains/release-notes.md, references/style-pass.md §2–3·§4 마지막 문단·§5, references/model-fingerprints.md (Claude)
Model: author=Claude Opus 5.5 executor=Claude Opus 5.5   (author: 이 샘플은 같은 세션에서 AI 문체를 흉내 내 일부러 작성됨)
Prose layer: author=prior executor=prior   (Opus 5.5는 전용 표가 없어 Opus 5 표를 prior로 적용)
Venue corpus: none — using domain baseline (참고할 기존 릴리스 노트 없음)
Style scan: 한국어 글이라 영어 금지어 목록을 같은 뜻의 한국어 표현으로 옮겨 적용함. §2 "X가 아니라 Y" — "단순한 업데이트가 아닌, … 여정의 한 걸음입니다"; §3 부풀린 형용사·거창한 명사 군집 — "강력한", "원활한", "끊임없는"(2회), "여정"; §5 리듬 — none (본문이 목록 위주라 측정 불가)
Failed:
 #1 챗봇 말투 — "안녕하세요! 이번 v2.3.0 업데이트를 여러분께 소개하게 되어 정말 기쁩니다", "감사합니다! 🙏"
 #2 밀도 — 전체 11줄이 담은 정보는 "v2.3.0에서 검색·성능이 개선되고 버그가 수정됨" 한 문장 분량
 #3 관련성 — 도입 문단("저희 팀의 끊임없는 노력의 결과물")과 마무리 문단이 업그레이드 판단에 쓸 정보를 주지 않음
 #5 구체성 — 버전 번호 외에 수치, 이슈/PR 번호, 바뀐 동작, 날짜가 하나도 없음: "크게 향상되어", "다양한 버그를 수정하여"
 #6 서식 — 이모지 제목("🚀", "✨"), 굵은 소제목을 단 글머리표, 정확히 3개짜리 목록
 #7 결론 상투구 — "앞으로도 더 나은 서비스를 위해 끊임없이 노력하겠습니다"
 #8 틀 반복 — "더욱 원활한 경험을 제공합니다" / "더욱 안정적인 서비스를 제공합니다"
Deferred:
 #5 구체성 — 검색 기능에서 실제로 바뀐 것, 성능 측정값과 조건, 수정한 버그 목록, 릴리스 날짜 — needs human (원문에 없어 TODO로 남김)
 release-notes 규칙 1 — 호환성이 깨지는 변경(breaking change)이 있는지 원문으로 알 수 없음 — needs human
Passed: 4, 9, 10
Verdict: cluster → recreate
```

## 처리 메모

- 저장소 규칙(CLAUDE.md 3번)에 따라 Verdict가 recreate이므로 다시 썼다.
- recreate 1단계에서 원문의 사실만 추린 목록: ① 버전 v2.3.0 ② 검색 기능 개선 ③ 성능 개선 ④ 버그 여러 건 수정. 이 외에는 원문에 사실이 없다.
- 위 네 가지에 없는 내용은 하나도 추가하지 않았고, 빠진 정보는 모두 `TODO`로 남겼다.
- 원문이 수치를 대지 않은 개선 주장("크게 향상", "빠르고 정확하게")은 근거가 없어 수정본에 옮기지 않았다.
