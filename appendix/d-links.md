# 부록 D — 관련 사이트와 저장소

이 아카이브가 참고하거나 가리키는 외부 사이트와 깃허브 저장소를 모았다. 이 아카이브는 직접 증명하거나 검증하지 않는다. 실제 증명과 검증, 그리고 그 진행 상황은 아래 사이트들이 1차로 다룬다. 링크가 끊기거나 내용이 바뀌면 이슈로 알려 달라.

## 공식 난제 목록

| 사이트 | 다루는 내용 |
|---|---|
| [Clay Mathematics Institute — Millennium Problems](https://www.claymath.org/millennium-problems/) | 밀레니엄 문제 7개의 공식 설명과 규정. [1부 정수론](../part1/01-number-theory.md)의 리만 가설, [2부 복잡도 이론](../part2/01-complexity-theory.md)의 P 대 NP 등 여러 문제의 1차 출처다 |
| [erdosproblems.com](https://www.erdosproblems.com/) | 토머스 블룸이 만든 폴 에르되시의 미해결 문제 목록. 2023년 시작했고 2026년 기준 1,000건을 훌쩍 넘는 문제가 등재돼 있다. 문제별로 상태(미해결/주장됨/해결)와 관련 논문을 보여 준다 |
| [FrontierMath — Open Problems (Epoch AI)](https://epoch.ai/frontiermath/open-problems) | AI 모델이 실제로 공개 난제를 풀었다고 주장할 때마다 등재하고 검증 상태를 갱신하는 추적 사이트. [8부 8.11](../part8/02-2026-second-half.md)의 아다마르 행렬 668차 항목도 여기서 가져왔다 |
| [위키백과 — List of unsolved problems in mathematics](https://en.wikipedia.org/wiki/List_of_unsolved_problems_in_mathematics) | 수학 전반의 미해결 문제를 분야별로 정리한 목록 |
| [위키백과 — List of unsolved problems in physics](https://en.wikipedia.org/wiki/List_of_unsolved_problems_in_physics) | [3부 물리학](../part3/01-particle-and-field.md)보다 훨씬 넓은 물리학 미해결 문제 목록 |
| [위키백과 — List of unsolved problems in computer science](https://en.wikipedia.org/wiki/List_of_unsolved_problems_in_computer_science) | [2부 전산학과 계산 이론](../part2/01-complexity-theory.md)과 겹치는 더 폭넓은 목록 |
| [위키백과 — List of unsolved problems in neuroscience](https://en.wikipedia.org/wiki/List_of_unsolved_problems_in_neuroscience) | 의식, 결합 문제(binding problem) 등 [5부 신경과학과 심리학](../part5/01-consciousness-and-brain.md)과 겹치는 목록 |

## AI가 낸 결과의 1차 출처

이 아카이브의 [8부 2절](../part8/02-2026-second-half.md)에서 다루는 2026년 사례들의 1차 출처다. 보도가 아니라 발표 주체가 직접 공개한 자료를 우선했다.

| 주체 | 링크 | 내용 |
|---|---|---|
| OpenAI | [github.com/openai/math](https://github.com/openai/math) | 2026년 10월 6일 공개한 대량 수학 원고 저장소. [8부 8.9](../part8/02-2026-second-half.md) |
| OpenAI | [openai.com/index/ten-advances-in-mathematics](https://openai.com/index/ten-advances-in-mathematics/) | 2026년 8월 1일 발표한 수학과 이론전산학 결과 10건 소개 글. [8부 8.7](../part8/02-2026-second-half.md) |
| OpenAI | [github.com/openai/ten-proofs](https://github.com/openai/ten-proofs) | 위 10건에 딸린 린(Lean) 증명서 저장소 |
| OpenAI | [github.com/openai/miniF2F](https://github.com/openai/miniF2F) | 올림피아드 수준 공식 수학 증명 벤치마크. 2026년 5월 29일 자로 보관(archive) 처리됐다 |
| 앤트로픽 | [anthropic.com/research/riemann-zeta](https://www.anthropic.com/research/riemann-zeta) | 2026년 8월 10일 발표, 리만 가설 관련 하한 개선. [8부 8.10](../part8/02-2026-second-half.md) |
| 구글 딥마인드 | [github.com/google-deepmind/alphageometry](https://github.com/google-deepmind/alphageometry) | 알파지오메트리 공식 코드. [8부 8.2](../part8/01-early-cases.md) |
| 구글 딥마인드 | [github.com/google-deepmind/alphaproof-nexus-results](https://github.com/google-deepmind/alphaproof-nexus-results) | 알파프루프 관련 증명 결과 보충 자료. [8부 8.3](../part8/01-early-cases.md) |

## 검증하고 감시하는 쪽

AI가 내놓은 수학 결과를 사람이 다시 확인하는 작업을 모아 둔 자리다. 이 아카이브가 "검증 상태"를 적을 때 가장 자주 참고하는 곳이다.

| 사이트 | 내용 |
|---|---|
| [github.com/teorth/erdosproblems — AI contributions 위키](https://github.com/teorth/erdosproblems/wiki/AI-contributions-to-Erd%C5%91s-problems) | 필즈상 수상자 테런스 타오가 직접 운영하며, AI가 에르되시 문제에 기여한 사례를 문제별로 추적한다. 자율적으로 풀었다고 알려졌다가 기존 논문의 재발견으로 정정된 사례도 숨기지 않고 남겨 둔다 |
| [terrytao.wordpress.com — AHM 성명 재게시](https://terrytao.wordpress.com/2026/10/07/ahm-statement-on-openais-october-6-release-of-mathematical-documents/) | 2026년 10월 OpenAI의 대량 공개에 대한 "인간 수학을 위한 협회" 성명과 테런스 타오의 의견 |
| [위키백과 — OpenAI bulk release of mathematical papers](https://en.wikipedia.org/wiki/OpenAI_bulk_release_of_mathematical_papers) | 2026년 10월 사태 전체를 정리한 문서 |
| [위키백과 — List of mathematical discoveries by artificial intelligence](https://en.wikipedia.org/wiki/List_of_mathematical_discoveries_by_artificial_intelligence) | AI가 수학에 기여했다고 보도된 사례를 통째로 모아 둔 목록. 이 아카이브의 8부보다 훨씬 자주 갱신된다 |

## 이 목록을 보는 법

이 부록의 링크 중에서도 "1차 출처"와 "검증하는 쪽"을 같이 읽어야 한다. 발표 쪽 자료만 읽으면 과장된 인상을 받기 쉽고, 비판 쪽 자료만 읽으면 실제 진전까지 깎아내리기 쉽다. [부록 B](b-legend.md)의 상태 기호가 그 사이 어디쯤인지를 요약한 것이다.
