# Knowledge Injector — 뉴럴 지식 주입 단말기

> 카파시의 도서관 꿈을 뒤집은 단일 HTML 앱. *"이 모든 책을 다 배울 순 없다 → 그러면 그걸 배울 무언가를 만들자, 그리고 그걸 내 머리에 주입하자."*

아무 지식 자료(텍스트·**PDF·PPTX·DOCX·TXT**)를 던지거나 **자연어로 주제를 물어보면**, AI가 대신 소화해 원자 단위 지식 카드로 분해하고, 인간 뇌가 가장 잘 흡수하는 과학적 방식(**FSRS-5 간격반복 + 능동인출**)으로 자동 주입합니다. 채점할수록 가운데 뇌 격자가 차오릅니다.

## 기능
- **파일 업로드** — PDF / PPTX / DOCX / TXT·MD 텍스트 자동 추출 (전부 client-side)
- **모델 선택** — Claude Haiku 4.5(빠름) · Sonnet 4.6(균형) · Opus 4.8(최고)
- **노력 단계** — Quick / Standard / Deep / **ULTRACODE**(멀티패스 + 최대 추론)
- **자연어 토픽 모드** — 파일 없이 주제만으로 카드 생성 (Claude API 키 필요)
- **FSRS-5 스케줄러** — Anki 탑재 최신 알고리즘, 로드마다 6개 레퍼런스값 자가검증
- **오프라인 코어** — 추출·FSRS·복습은 서버/네트워크 없이 동작 (덱은 localStorage 저장)

100% 클라이언트 사이드. Claude 생성/토픽과 PDF 등 라이브러리 첫 로드만 네트워크 사용.

검증: FSRS·소화엔진 Node 27/27, 헤드리스 Edge FSRS selftest 15/15, 엔드투엔드 + 모델별 API 규약(400 함정) 검사 전수 PASS.

— Built with Claude Code (DreamsComeTrue)
