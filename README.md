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
| `computer_science/` | 소프트웨어 아키텍처, 네트워크·인프라, 관측성, 병렬 처리 성능 모델 |
| `hardware/` | 보드·카메라 등 하드웨어 선택과 구성(CCTV), 제어의 기초(PID) |
| `system_engineering/` | 시스템 엔지니어링 운영: 장애 등급, 시스템 모니터링 |
| `index.html` | GitHub Pages 목차 페이지 (루트에 유지) |
| 루트의 `.md` | HTML이 아닌 기획서 |

새 HTML은 주제에 맞는 폴더에 넣습니다. 폴더 안의 HTML끼리는 같은 폴더의 상대 경로로 서로 링크합니다.

## 저장소의 성격

- 기술 참고 자료, 학습 가이드와 기획 문서를 모아 두는 저장소입니다. 문서에는 구조도, 비교표, 명령어·설정·의사 코드 예제가 포함됩니다.
- 현재 자료는 한국어로 작성된 **HTML 가이드 21개와 Markdown 기획서 1개**입니다. 이 README는 전체 자료의 목차와 이용 안내를 제공합니다.
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
| [system_engineering/system-engineering-incident-priority.html](./system_engineering/system-engineering-incident-priority.html) | P0–P4 장애 등급과 모니터링 | 사용자 영향에서 출발해 P0–P4 등급을 정하는 방법과 알림 설계, 대응·에스컬레이션, SLO와의 연결을 System Engineer 입문자용으로 정리한 교육용 안내서 |
| [linux-command-game-experience-plan.ko.md](./linux-command-game-experience-plan.ko.md) | 리눅스 명령어 학습 게임 기획 | 기록 정거장 복구를 통해 파일·경로·명령 선택과 결과 확인을 배우는 게임의 경험 기획서 |

## 자료별 설명

### Pi 코딩 에이전트 가이드

`ai/Pi-코딩-에이전트-가이드.html`

Pi를 설치하고 모델을 연결해 실제 작업을 시키기까지의 흐름을 다룹니다.

- 설치와 첫 실행: Windows 환경 준비, 공식 npm 패키지 설치, 작업 폴더에서 시작, 인증과 모델 선택
- 작업 흐름: 읽기 → 수정 → 실행 → 검토를 이어가는 방식, 작업 중 방향 전환, 세션 이어하기
- 입력창 기능 탐색과, 목표·범위·조건·검증을 함께 전달하는 요청 방법
- 필요한 만큼만 기능을 더하는 확장 방식과 자동화 연동
- 주의점: 터미널과 도구가 쓰는 셸의 구분, 작업 폴더가 권한 경계가 아니라는 점, 변경 복구·검토, 신뢰와 공유의 구분
- 설치 환경과 최신 동작은 원문 확인 안내

### 오프라인 STT 선택 가이드

`ai/offline-stt-guide.html`

인터넷 없이 기기 안에서 동작하는 음성 인식을 고르기 위한 기술 선택 노트입니다. 한국어·영어 짧은 명령 인식을 전제로 다음 두 후보를 먼저 비교합니다.

- **Vosk**: 한국어/영어 소형 모델
- **SenseVoice INT8**: sherpa-onnx 실행 엔진 기반

주요 내용: 실행 엔진과 모델을 함께 고르는 기준, 언어 모델 하나를 유지하고 한 번 로드해 발화마다 재사용하는 방법, STT 결과를 허용된 명령으로 연결하는 방식, 파일 크기·RAM·응답 속도 비교(RTF는 전체 응답 시간이 아니라는 점 포함), 같은 명령 녹음으로 두 후보를 비교하는 절차, 수치와 제약의 출처.

### 오프라인 TTS 선택 가이드

`ai/offline-tts-guide.html`

네트워크 없이 작은 보드에서 음성을 출력하기 위한 기술 선택 노트입니다.

- **미리 생성한 음성**: TTS로 만든 파일을 기기에 저장해 재생
- **eSpeak NG**: 한국어·영어 지원 규칙 기반 합성, 최소 자원용
- **MeloTTS**: 자연스러운 가변 발화용 비교 검증 대상 (대안: Supertonic 3 INT8)

주요 내용: 한국어 지원과 배포 조건(라이선스) 선별, 반복 문구는 캐시하고 새 문장은 모델로 생성하는 전략, 숫자·단위·한영 혼합·약어가 뜻대로 읽히는지 확인하는 방법, 첫 소리까지의 시간과 지속 속도를 분리해 측정하는 방법, 언어·라이선스·배포 경로의 출처.

### 로컬 AI 모델 선택 가이드

`ai/local-ai-guide.html`

Ollama와 ComfyUI, 특수 목적 모델의 실행 환경을 구분하고 내 노트북에서 사용할 모델을 고르기 위한 가이드입니다.

- Ollama의 모델 실행·관리, ComfyUI의 노드 워크플로, Qwen3-TTS의 별도 실행 환경과 연결 흐름
- 코딩·수학·범용 모델의 목적별 비교와 공개 평가 3종 × 벤치마크 15개 점수표, 문서 검색용 임베딩·음성 모델의 역할
- ROG Strix G16, Ryzen 9 8940HX, RAM 64GB·RTX 5070 Laptop VRAM 8GB 구성을 기준으로 로컬 테스트에서 응답을 확인한 모델(Gemma 4 E4B, Llama 3.1 8B, DeepSeek-R1 8B)과 RAM을 나눠 쓰는 확장 후보
- 모델 용도·실행 범위 필터, 벤치마크별 그래프 전환, 실행 명령 복사
- 직접 실행해 응답을 확인한 결과와 개발사·공개 평가 점수를 구분하며, 응답 속도는 실측값이 아님

### CCTV 카메라 선택 노트

`hardware/cctv-camera-guide.html`

ESP32 카메라 보드나 라즈베리파이로 NAS에 녹화하고 실시간으로 볼 수 있는 저가 CCTV를 만들 때의 선택 노트입니다. 다음 두 후보를 비교합니다.

- **ESP32-S3 + 미들서버**: 카메라는 영상만 내보내고 감지·녹화는 기존 PC가 담당 (go2rtc, Frigate, FFmpeg)
- **Raspberry Pi Zero 2 W**: 하드웨어 H.264 인코딩과 동작 → 물체 2단계 감지를 한 보드에서 처리

주요 내용: 사양·카메라·압축 방식 비교표, 두 구성의 구조도, 순환 버퍼 녹화와 상시 녹화 + 이벤트 태깅의 차이, 하루 저장 용량 대략치, Wi-Fi·전원·발열·단일 장애점 등 운영 문제, 상황별 선택 기준과 만드는 순서. 가격과 속도, 용량 수치는 대략치입니다.

### PID 제어를 그림으로 이해하기

`hardware/pid-control.html`

자동차 정속 주행 장치를 예로, 목표와 현재 값의 차이를 보고 조작량을 계속 고치는 피드백 제어를 설명하는 입문 가이드입니다.

- 설정값·측정값·오차와 측정 → 비교 → 조절 → 재측정의 피드백 고리, 샤워 물 온도를 맞추는 비유
- P는 현재 차이, I는 쌓인 차이, D는 변화 속도를 본다는 세 항의 역할과 `조작량 = P + I + D`
- Kp·Ki·Kd를 슬라이더로 바꾸며 속도 곡선과 오르막 방해의 영향을 보는 조절 모형(개념 학습용 가상 자동차이며 실제 차량의 응답과 같지 않음)
- 오버슈트·진동·정착, 출력 한계와 적분 누적 방지, 센서 잡음, 지연 같은 실제 적용 시 고려 사항

### Monolith + 2-Tier + MVC

`computer_science/architecture-guide.html`

직원 PC의 주문·재고 관리 프로그램이 별도 DB 서버와 직접 통신하는 예시로, 배포 단위·실행 계층·내부 책임을 구분합니다.

- Monolith는 화면과 업무 기능을 묶은 배포 단위, 2-Tier는 클라이언트와 DB의 실행 경계, MVC는 클라이언트 내부의 역할을 뜻합니다.
- Layer와 Tier, Model과 DB의 차이, 주문 조회부터 화면 갱신까지의 흐름을 설명합니다.
- 여러 PC의 설치본·버전 호환성, DB 권한·연결·트랜잭션·동시성 등 운영할 항목을 다룹니다.

### Monolith + 3-Tier · SPA + API

`computer_science/monolith-3-tier-spa-api.html`

브라우저 SPA → API 백엔드 → DB로 표현·업무·데이터의 실행 책임을 나눈 주문·재고 서비스 예시입니다. 여기서 Monolith는 여러 업무 기능을 함께 배포하는 API 백엔드를 가리킵니다.

- SPA의 정적 파일 로딩·화면 전환과 API의 인증·권한·업무 처리를 구분합니다.
- 주문 생성의 HTTP·JSON 요청과 DB 트랜잭션, 응답 유실과 중복 요청 처리를 설명합니다.
- SPA와 API의 별도 배포, 구버전 호환성, API 복제·확장, CORS·인증과 사용자 경험을 다룹니다.

### Modular Monolith

`computer_science/modular-monolith.html`

업무별 모듈의 책임과 데이터 소유권을 분명히 하면서 애플리케이션은 하나로 배포하는 구조입니다.

- 공개 인터페이스와 내부 구현, 모듈 간 의존 방향과 순환 참조 방지를 설명합니다.
- 공유 DB에서도 데이터의 소유자를 구분하는 방법, 모듈 간 조회와 트랜잭션 참여 계약을 다룹니다.
- 내부 이벤트·Outbox의 적용 조건, 경계를 유지하는 코드 접근 제한과 의존성 검증, 배포·자원 공유의 비용을 정리합니다.

### Microservices

`computer_science/microservices.html`

주문·재고·결제 서비스를 예로, 업무 경계에 맞춘 독립 실행·배포와 데이터 소유권을 설명합니다.

- 동기 API와 비동기 이벤트, 계약 호환성과 서비스별 저장소 접근 원칙을 비교합니다.
- 여러 로컬 트랜잭션으로 이어지는 주문 처리, Saga와 보상, Outbox와 멱등성을 다룹니다.
- 타임아웃의 결과 불명 상태, 재시도·상태 대사·장애 전파 제어와 서비스별 관측·운영 책임을 정리합니다.

### Micro-frontends

`computer_science/micro-frontends.html`

업무별 프런트엔드의 변경·배포 책임을 나누고 하나의 제품으로 조합하는 구조입니다. 주요 예시는 Shell이 경로에 따라 업무 앱을 로드하는 브라우저 런타임 조합입니다.

- 경로·페이지, 브라우저, 서버·엣지, iframe, 빌드 시 조합 방식을 비교합니다.
- 앱 로딩·종료, 라우팅·이벤트·상태·인증 연계와 구버전 자원의 호환성을 다룹니다.
- 같은 페이지에서 공유하는 CSS·라이브러리·실행 환경의 영향과 제품 전체의 성능·접근성·검증·관측을 설명합니다.

### 이벤트 기반 아키텍처(EDA)

`computer_science/event-driven-architecture.html`

주문 확정이라는 사실에 배송·알림·분석이 반응하는 예시로 이벤트 기반 협력을 설명합니다. 모놀리스 내부에도 적용할 수 있으며, 주요 예시는 브로커를 사용하는 비동기 분산 구성입니다.

- Command·Event·Query, 독립 구독과 같은 구독 안의 작업 분담을 구분합니다.
- 브로커 수락과 업무 완료의 차이, Transactional Outbox, 멱등 소비자, 재시도·DLQ·순서·재처리를 다룹니다.
- 이벤트 계약·버전, 최종적 일관성, Choreography·Orchestration·Saga와 Event Sourcing·CQRS의 관계를 정리합니다.

### Hexagonal Architecture

`computer_science/hexagonal-architecture.html`

Ports & Adapters 구조로 애플리케이션의 업무 핵심과 외부 기술의 경계를 설명합니다.

- 입력·출력 Port와 Driving·Driven Adapter, 실행 흐름과 소스 코드 의존성의 차이를 다룹니다.
- 의존성 역전(DIP)과 의존성 주입(DI), 주문 생성 유스케이스와 외부 구현의 조립을 설명합니다.
- DB 없이 핵심을 검증하는 방법과 실제 Adapter의 통합 검증, 자료형·오류·트랜잭션 경계의 설계 비용을 정리합니다.

### Onion Architecture

`computer_science/onion-architecture.html`

도메인 모델을 중심에 두고 UI·인프라 등 바깥 코드가 안쪽 정책에 의존하도록 구성하는 구조입니다.

- Domain Model·Domain Services·Application Services·Infrastructure의 책임을 주문 생성·취소로 설명합니다.
- 안쪽이 소유하는 Repository 계약과 바깥 구현, DB Row·업무 모델·표현 데이터의 경계를 다룹니다.
- 계층별 검증과 적용 판단, Hexagonal·Clean 및 배포·협력 방식과의 관계를 정리합니다.

### Clean Architecture

`computer_science/clean-architecture.html`

소스 코드 의존성이 안쪽 정책을 향해야 한다는 Dependency Rule을 중심으로 업무 규칙과 유스케이스를 보호하는 구조입니다.

- Entities·Use Cases·Interface Adapters·Frameworks & Drivers의 책임을 구분합니다.
- Input·Output Boundary, Persistence Gateway와 Presenter를 사용하는 주문 생성 흐름을 설명합니다.
- 요청·응답·영속성·화면 모델의 차이, 외부 조립 지점(Composition Root), 경계별 검증과 적용 판단을 다룹니다.

### CQRS

`computer_science/cqrs.html`

상태를 변경하는 명령 모델과 정보를 읽는 조회 모델을 목적에 맞게 분리하는 패턴입니다. 같은 프로세스·같은 DB에서도 적용할 수 있습니다.

- CQS와 CQRS의 차이, 쓰기 모델의 업무 규칙과 전용 조회·읽기 모델의 책임을 설명합니다.
- 저장소 분리의 선택지, 비동기 Projection의 갱신 지연과 명령 성공 직후의 화면 처리를 다룹니다.
- 중복·동시성·순서·조회 권한·재구축 정책을 정리하고, CQRS·EDA·Event Sourcing을 구분합니다.

### SSH 역방향 터널

`computer_science/reverse-tunnel.html`

내부 서버가 클라우드 VM으로 SSH 연결을 먼저 맺고, VM의 Nginx가 HTTPS 요청을 터널을 통해 내부 웹 서비스에 전달하는 구성입니다.

- 연결 경로 확인부터 전용 계정·키, `ssh -R`, Nginx·TLS, DNS 전환까지의 순서를 설명합니다.
- VM의 터널 포트를 `127.0.0.1`에 한정하고 `PermitListen`·`GatewayPorts`·방화벽으로 제한하는 방법을 다룹니다.
- 프록시 헤더·내부 HTTP 구간·키 유출의 위험, 연결 단절·자동 재접속·인증서·WebSocket·업로드 검증을 정리합니다.

### 클라우드 ↔ 내부망 VPN

`computer_science/cloud-internal-vpn.html`

WireGuard로 클라우드 VM과 내부망 게이트웨이 사이에 암호화된 IP 경로를 만들고, VM의 Nginx가 내부 웹 서버에 접근하는 예시입니다.

- 단일 포트 전달인 SSH 역방향 터널과 VPN 라우팅의 차이, 요청·응답 경로와 IP 포워딩·SNAT을 설명합니다.
- 피어·주소·`AllowedIPs`·NAT keepalive 설정과, 별도 방화벽으로 내부 접근을 필요한 주소·포트에 제한하는 방법을 다룹니다.
- 키·VM 침해, UDP·MTU·반환 경로·단일 장애점과 실제 외부 웹 요청의 검증 순서를 정리합니다.

### OpenTelemetry + Jaeger

`computer_science/opentelemetry-jaeger.html`

OpenTelemetry의 계측·수집·전송과 Jaeger v2의 Trace 저장·조회 역할을 연결해 설명하는 관측 가이드입니다.

- Metric·Log·Trace, Trace·Span·Resource와 W3C Trace Context의 문맥 전파를 구분합니다.
- OTLP, 선택적인 별도 Collector의 파이프라인, Jaeger 수집·저장·Query·UI 경로와 타임라인 읽기를 설명합니다.
- EDA의 비동기 추적과 Span Link, 샘플링·누락·보관·민감 정보·비용 및 도입·문제 해결 순서를 다룹니다. 실행 가능한 배포 설정은 포함하지 않습니다.

### 암달과 구스타프손의 법칙

`computer_science/amdahl-and-gustafson-laws.html`

병렬 처리의 효과를 서로 다른 조건에서 계산하는 두 법칙을 비교하는 학습 가이드입니다. 차이는 무엇을 고정하는가에 있습니다.

- 암달의 법칙은 작업량을 고정하고, 순차 부분이 시간 단축의 상한(`1/s`)을 정한다는 점을 식 유도와 함께 설명합니다.
- 구스타프손의 법칙은 실행 시간을 고정하고, 같은 시간에 처리할 작업량을 키우는 경우를 설명하며 ‘9.1배’가 뜻하지 않는 것을 짚습니다.
- 100분짜리 기준 작업에서 두 실험(작업량 고정, 실행 시간 고정)을 비교하고, 같은 작업으로 맞추면 두 식이 같은 답을 낸다는 점을 보입니다.
- 순차 비율과 코어 수를 바꿔 보는 계산 모형, 작업 분배·동기화, 메모리·입출력, 확장 가능한 작업량 같은 현실의 제약을 다룹니다.
- 암달의 법칙이 병렬 처리 밖의 최적화에도 적용된다는 점(이미지 처리 예), 속도 향상률·코어 효율·처리량의 구분, 강한 확장과 약한 확장, 순차 시간이 고정된 값이 아니라는 점을 정리합니다.

### P0–P4 장애 등급과 시스템 모니터링 안내서

`system_engineering/system-engineering-incident-priority.html`

System Engineer 입문자와 서비스 운영 참여자를 위해, 측정값이 아니라 사용자 영향에서 장애 등급을 판단하는 방법을 정리한 교육용 안내서입니다. 등급은 대응 인력·시간·의사소통을 연결하는 조직의 운영 약속이라는 관점으로 설명합니다.

- Severity·Priority·Alert level의 차이, P0–P4 등급별 영향 기준·대표 사례·기본 대응
- 영향(Impact)과 긴급도(Urgency)를 교차하는 판단 방법과, 데이터·보안 위험을 점수와 별도로 검토해야 하는 이유, 가상 사례 비교
- 사용자 결과와 시스템 내부 신호를 함께 관측하는 모니터링, 실행 가능한 알림 설계
- 탐지·확인·선언과 호출·완화·검증·회고의 대응 단계, 담당자와 등급 두 방향의 에스컬레이션, 응답·복구 시간의 구분
- SLI·SLO·오류 예산과 P등급의 연결, 팀 등급 정책에 넣을 항목과 점검 질문
- P0–P4 정의표, 매트릭스, 사례, 응답 시간은 이 문서의 교육용 예시이며 업계 표준이나 특정 기업의 정책이 아님. 참고한 공개 지침(PagerDuty, Google SRE 문서)의 확인일은 2026년 11월 25일

### 리눅스 명령어 학습 게임 경험 기획서

`linux-command-game-experience-plan.ko.md`

가제 **기록 정거장**, 기획 제안 v0.1입니다. 정거장을 복구하는 탐험과 부탁을 통해 리눅스 입문자가 상황을 관찰하고, 명령을 고르고, 결과를 확인하도록 설계한 문서입니다.

- 파일·폴더·현재 경로를 세계의 기록·방·위치에 연결하고, 입력 → 탐색 → 읽기 → 검색 → 정리 → 독립 해결의 성장 여정을 제안합니다.
- 대표 미션, 단계별 힌트, 오류 설명, 게임 차원의 복구 기능, 화면·접근성·회고와 실제 터미널로의 전이를 다룹니다.
- 첫 버전은 약 15분의 도입과 짧은 독립 미션에서 탐색·읽기·복사·이동을 확인하는 범위입니다. 구현된 게임이나 검증된 학습 효과를 보고하는 문서는 아니며, 사용자 관찰로 확인할 가설을 제시합니다.

## 보는 방법

저장소를 클론하거나 파일을 내려받으면 됩니다. HTML은 최신 브라우저에서 직접 열고, Markdown 기획서는 GitHub 또는 Markdown 미리보기를 지원하는 편집기에서 읽습니다. 별도의 패키지 설치, 빌드나 서버 실행은 필요하지 않습니다.

```bash
git clone https://github.com/neosdc/kyujanggak.git
cd kyujanggak
```

예를 들어 Windows PowerShell에서는 다음과 같이 HTML을 기본 브라우저로 엽니다.

```powershell
Start-Process .\ai\offline-stt-guide.html
```

macOS에서는 `open ai/offline-stt-guide.html`, Linux 데스크톱에서는 `xdg-open ai/offline-stt-guide.html`을 사용할 수 있습니다.

Google Fonts와 외부 참고 링크에는 인터넷 연결이 필요합니다. 네트워크가 없어도 HTML 본문과 내장 도식은 읽을 수 있으며, 웹 글꼴을 받지 못하면 시스템 글꼴로 표시됩니다. 아키텍처 문서의 넓은 도식은 작은 화면에서 좌우로 스크롤해 볼 수 있습니다.

일부 HTML은 도식 재생, 텍스트 선택 후 댓글·질문 작성과 답변 복사를 지원합니다. 메모 저장은 브라우저의 `localStorage`를 사용하므로 로컬 파일 접근 정책에 따라 유지되지 않을 수 있습니다. 인쇄용 스타일이 있는 문서는 브라우저의 인쇄 기능으로 PDF로 저장할 수 있습니다.

## 참고

- 모델 크기·성능·라이선스, 도구 버전과 설정은 작성 시점 기준이며 변할 수 있습니다. 문서에 기재된 작성 기준과 출처·참고 링크를 확인하세요.
- STT·TTS 가이드는 공식 자료를 정리한 선택 노트이며 실제 보드의 실측 결과는 포함하지 않습니다. CCTV의 가격·속도·용량도 대략치입니다.
- 구조도와 명령어·설정·의사 코드 예제의 생략 사항과 검증 범위는 각 문서의 안내를 따릅니다. 실제 적용 시에는 사용하는 버전과 환경에서 확인하세요.
- 새 자료를 추가하거나 내용을 바꿀 때는 위 표, "자료별 설명", `index.html`의 목차 카드도 함께 갱신합니다.
