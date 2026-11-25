# 규장각 (kyujanggak)

내가 나중에 다시 찾아볼 기술 자료를 모아 두는 저장소입니다.

이름은 조선 정조가 1776년에 세운 왕실 도서관 규장각(奎章閣)에서 따왔습니다. 규장각이 중요한 서적과 문서를 모아 보관하고 필요할 때 꺼내 보는 곳이었던 것처럼, 이 저장소도 참고할 만한 자료를 한곳에 쌓아 두고 다시 찾아보는 서가 역할을 합니다.

## 웹에서 보기

GitHub Pages로 배포하면 별도 설치 없이 브라우저에서 바로 읽을 수 있습니다.

- 주소: <https://neosdc.github.io/kyujanggak/>
- 루트의 `index.html`이 전체 자료의 목차 페이지입니다. 문서끼리의 상대 링크도 그대로 동작합니다.
- Markdown 기획서는 Pages에서 렌더링되지 않으므로 목차의 링크가 GitHub의 파일 보기로 연결됩니다.
- 새 HTML을 추가하면 `index.html`의 카드 목록에도 항목을 추가해야 합니다.

## 폴더 구조

| 경로 | 내용 |
| --- | --- |
| `ai/` | AI 도구와 모델: 코딩 에이전트, 로컬 AI 모델 선택, 오프라인 음성 인식(STT)·합성(TTS) |
| `computer_science/` | 소프트웨어 아키텍처, 네트워크·인프라, 관측성, 로그 레벨, 병렬 처리 성능 모델 |
| `hardware/` | 보드·카메라 등 하드웨어 선택과 구성(CCTV), 제어의 기초(PID) |
| `system_engineering/` | 시스템 엔지니어링 운영: 장애 등급, 시스템 모니터링 |
| `index.html` | GitHub Pages 목차 페이지 (루트에 유지) |
| 루트의 `.md` | HTML이 아닌 기획서 |

새 HTML은 주제에 맞는 폴더에 넣습니다. 폴더 안의 HTML끼리는 같은 폴더의 상대 경로로 서로 링크합니다.

## 저장소의 성격

- 기술 참고 자료, 학습 가이드와 기획 문서를 모아 두는 저장소입니다. 문서에는 구조도, 비교표, 명령어·설정·의사 코드 예제가 포함됩니다.
- 현재 자료는 한국어로 작성된 **HTML 가이드 22개와 Markdown 기획서 1개**입니다. 이 README는 전체 자료의 목차를 제공합니다.
- HTML의 스타일, 스크립트와 SVG 도식은 각 파일 안에 포함되어 있습니다. 글꼴은 외부 Google Fonts를 사용하며, 일부 문서에는 단계별 도식 재생·검색·복사 같은 상호작용이 있습니다.
- 문서를 열기 위한 빌드나 서버는 필요하지 않습니다. 별도의 빌드 설정, 자동 테스트나 배포 스크립트는 없습니다.

## 자료 목록

| 파일 | 주제 | 한 줄 요약 |
| --- | --- | --- |
| [ai/Pi-코딩-에이전트-가이드.html](./ai/Pi-코딩-에이전트-가이드.html) | Pi 코딩 에이전트 | 터미널에서 파일을 읽고 코드를 수정하고 명령을 실행하는 코딩 에이전트 Pi의 구조부터 첫 실행까지 정리한 사용 가이드 |
| [ai/offline-stt-guide.html](./ai/offline-stt-guide.html) | 오프라인 STT 선택 | 저사양 보드에서 한국어·영어 짧은 명령을 인식하기 위한 음성 인식(STT) 모델 비교 노트 |
| [ai/offline-tts-guide.html](./ai/offline-tts-guide.html) | 오프라인 TTS 선택 | 작은 보드에서 네트워크 없이 한국어·영어 음성을 출력하기 위한 음성 합성(TTS) 모델 선택 노트 |
| [ai/local-ai-guide.html](./ai/local-ai-guide.html) | 로컬 AI 모델 선택 | Ollama·ComfyUI·Qwen3-TTS의 역할, 로컬 테스트에서 응답을 확인한 모델과 확장 후보, 공개 평가 3종·벤치마크 15개 점수 비교를 RAM 64GB·RTX 5070 Laptop 8GB 노트북 기준으로 정리한 가이드 |
| [hardware/cctv-camera-guide.html](./hardware/cctv-camera-guide.html) | CCTV 카메라 선택 | ESP32-S3와 라즈베리파이 Zero 2 W를 후보로, NAS 녹화·실시간 시청·동작/물체 감지가 되는 저가 CCTV를 구성하는 방법을 비교한 노트 |
| [hardware/pid-control.html](./hardware/pid-control.html) | PID 제어 | 목표와 현재의 차이를 보고 조작을 고치는 PID 제어에서 P·I·D의 역할을 자동차 정속 주행 비유와 계수 조절 모형으로 설명한 입문 가이드 |
| [computer_science/architecture-guide.html](./computer_science/architecture-guide.html) | Monolith + 2-Tier + MVC | 화면과 업무 기능을 담은 하나의 클라이언트 프로그램이 별도 DB 서버에 직접 연결하는 구성을 설명한 학습 가이드 |
| [computer_science/monolith-3-tier-spa-api.html](./computer_science/monolith-3-tier-spa-api.html) | Monolith + 3-Tier · SPA + API | 브라우저 SPA, 모놀리식 API 백엔드, DB의 책임과 요청 흐름을 설명한 학습 가이드 |
| [computer_science/modular-monolith.html](./computer_science/modular-monolith.html) | Modular Monolith | 업무 모듈의 공개 계약·데이터 소유권·의존성 경계를 유지하면서 하나의 애플리케이션으로 배포하는 구조 |
| [computer_science/microservices.html](./computer_science/microservices.html) | Microservices | 독립 배포하는 업무 서비스의 계약, 데이터 소유권, 분산 트랜잭션과 장애 대응을 설명한 가이드 |
| [computer_science/micro-frontends.html](./computer_science/micro-frontends.html) | Micro-frontends | 업무별 프런트엔드를 Shell과 조합하고 팀별 배포·라우팅·상태·스타일의 경계를 관리하는 방법 |
| [computer_science/event-driven-architecture.html](./computer_science/event-driven-architecture.html) | 이벤트 기반 아키텍처(EDA) | 이벤트 발행·구독, Outbox, 중복·순서·실패 처리와 업무 완료 기준을 설명한 가이드 |
| [computer_science/hexagonal-architecture.html](./computer_science/hexagonal-architecture.html) | Hexagonal Architecture | Port와 Adapter로 업무 핵심을 UI·DB·메시지 등 외부 기술과 연결하는 구조 |
| [computer_science/onion-architecture.html](./computer_science/onion-architecture.html) | Onion Architecture | 도메인 모델을 중심에 두고 바깥 기술이 안쪽 정책에 의존하도록 설계하는 구조 |
| [computer_science/clean-architecture.html](./computer_science/clean-architecture.html) | Clean Architecture | Dependency Rule과 Use Case 경계로 핵심 업무 규칙을 외부 기술에서 보호하는 구조 |
| [computer_science/cqrs.html](./computer_science/cqrs.html) | CQRS | 명령과 조회의 모델·책임을 분리하고 읽기 모델의 갱신·지연·복구를 설계하는 패턴 |
| [computer_science/reverse-tunnel.html](./computer_science/reverse-tunnel.html) | SSH 역방향 터널 | 내부 웹 서비스를 클라우드 VM의 Nginx와 SSH 역방향 터널로 공개하는 구성·보안·운영 노트 |
| [computer_science/cloud-internal-vpn.html](./computer_science/cloud-internal-vpn.html) | 클라우드 ↔ 내부망 VPN | WireGuard로 클라우드 VM과 내부망을 연결하고 Nginx가 내부 웹에 접근하도록 하는 구성 노트 |
| [computer_science/opentelemetry-jaeger.html](./computer_science/opentelemetry-jaeger.html) | OpenTelemetry + Jaeger | 계측·문맥 전파·OTLP 수집과 Jaeger의 Trace 저장·조회, 샘플링·운영을 설명한 가이드 |
| [computer_science/amdahl-and-gustafson-laws.html](./computer_science/amdahl-and-gustafson-laws.html) | 암달·구스타프손의 법칙 | 작업량을 고정하는 암달의 법칙과 실행 시간을 고정하는 구스타프손의 법칙을 식 유도, 100분 기준 예시, 계산 모형으로 비교한 학습 가이드 |
| [computer_science/software-log-levels.html](./computer_science/software-log-levels.html) | 소프트웨어 로그 레벨 | TRACE부터 FATAL까지 로그 레벨의 의미와 출력 설정, 로그 작성·수집·조회, 운영 정책과의 연결을 개발자·System Engineer·SRE용으로 설명한 안내서 |
| [system_engineering/system-engineering-incident-priority.html](./system_engineering/system-engineering-incident-priority.html) | P0–P4 장애 등급과 모니터링 | 사용자 영향에서 출발해 P0–P4 등급을 정하는 방법과 알림 설계, 대응·에스컬레이션, SLO와의 연결을 System Engineer 입문자용으로 정리한 교육용 안내서 |
| [linux-command-game-experience-plan.ko.md](./linux-command-game-experience-plan.ko.md) | 리눅스 명령어 학습 게임 기획 | 기록 정거장 복구를 통해 파일·경로·명령 선택과 결과 확인을 배우는 게임의 경험 기획서 |

## 참고

- 모델 크기·성능·라이선스, 도구 버전과 설정은 작성 시점 기준이며 변할 수 있습니다. 문서에 기재된 작성 기준과 출처·참고 링크를 확인하세요.
- STT·TTS 가이드는 공식 자료를 정리한 선택 노트이며 실제 보드의 실측 결과는 포함하지 않습니다. CCTV의 가격·속도·용량도 대략치입니다.
- 구조도와 명령어·설정·의사 코드 예제의 생략 사항과 검증 범위는 각 문서의 안내를 따릅니다. 실제 적용 시에는 사용하는 버전과 환경에서 확인하세요.
- 새 자료를 추가하거나 내용을 바꿀 때는 위 표와 `index.html`의 목차 카드도 함께 갱신합니다.
