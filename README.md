## 장민석 · Minseok Jang

**NHN AD** 백엔드 개발자. 광고 운영 플랫폼의 LLM 에이전트와 데이터 배치를 만듭니다.

[![Blog](https://img.shields.io/badge/Blog-colamong.github.io-222222?style=flat-square&logo=astro&logoColor=white)](https://colamong.github.io)
[![Gmail](https://img.shields.io/badge/mjang.dev@gmail.com-d14836?style=flat-square&logo=Gmail&logoColor=white)](mailto:mjang.dev@gmail.com)

---

### 지금 하는 일

- **LLM 에이전트 백엔드** — AWS Bedrock 기반 채팅 에이전트의 툴 호출·응답 경로를 Kotlin/Spring 과 Python 으로 구현하고 운영합니다.
- **광고 데이터 배치** — 매체 연동과 트래킹 수집을 Spring Batch · AWS Lambda 로 돌리고, S3 + Athena 에 쌓아 조회합니다.
- **분산 추적** — API → 에이전트 → 배치로 이어지는 한 요청을 traceId 로 잇는 일. 이 관심이 아래 OpenTelemetry 기여로 이어졌습니다.

### 오픈소스 기여

머지된 PR 17건.

| 저장소 | 머지 | 무엇을 고쳤나 |
|---|:---:|---|
| [opentelemetry-java-instrumentation](https://github.com/open-telemetry/opentelemetry-java-instrumentation) ⭐2.6k | 1 | `otel.spring-starter.debug` 플래그가 켜지지 않던 문제. `LoggingExporterAutoConfiguration` 이 두 등록 파일 모두에서 빠져 Spring Boot 가 발견하지 못했습니다. 기존 테스트는 `AutoConfigurations.of(...)` 로 클래스를 직접 등록해 탐색 경로를 건너뛰었기에 전부 통과하고 있었고, 실제 부팅을 태우는 테스트를 함께 추가했습니다 |
| [egovframe-common-components](https://github.com/eGovFramework/egovframe-common-components) ⭐78 | 11 | 전자정부 표준프레임워크 공통 컴포넌트. 작성자·관리자 권한 검증 누락, 로그인 세션과 중복 제출 토큰의 동시성, 검증 실패 시 화면 상태 복원 |
| [egovframe-docs](https://github.com/eGovFramework/egovframe-docs) | 5 | 표준프레임워크 포털 가이드 문서의 본문 보강과 설정·URL 현행화 |

대표 PR — [otel#19725](https://github.com/open-telemetry/opentelemetry-java-instrumentation/pull/19725) · [egov#1091 중복 로그인 세션 바인딩 동시성 보완](https://github.com/eGovFramework/egovframe-common-components/pull/1091) · [egov#1081 사용자 목록 조회 시 관리자 검증 추가](https://github.com/eGovFramework/egovframe-common-components/pull/1081)

### 기술 스택

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=Kotlin&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=OpenJDK&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=Spring&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=Python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=PostgreSQL&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=Redis&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=flat-square&logo=OpenTelemetry&logoColor=white)

### 쓴 글

- [에이전트에서는 docstring이 코드다](https://colamong.github.io/posts/docstring-is-code/) — 툴 설명은 주석이 아니라 인터페이스입니다
- [docstring 작성 가이드](https://colamong.github.io/posts/docstring-writing-guide/) — 3~4문장부터 시작합니다

더 많은 글은 [colamong.github.io](https://colamong.github.io) 에 있습니다.
