<div align="center">

# 따랑해

### 믿을 수 있는 사람이 소개해주는, 새로운 소개팅 문화

<br/>

[![Service](https://img.shields.io/badge/Service-mileojwo.com-FF6B8A?style=flat-square)](https://mileojwo.com)
[![Location](https://img.shields.io/badge/Location-South_Korea-blue?style=flat-square)](#)
[![GitHub Org](https://img.shields.io/badge/GitHub-mileojwo-181717?style=flat-square&logo=github)](https://github.com/mileojwo)

</div>

---

<br/>

## Team

<table align="center">
  <tr>
    <td align="center">
      <a href="https://github.com/lmalma2004">
        <img src="./assets/junmo-profile.jpg" width="250px;" style="border-radius: 50%;" alt="준모"/>
        <br/><br/>
        <sub><b>준모</b></sub>
        <br/>
        <sub>CEO</sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/solone313">
        <img src="./assets/hojin-profile.jpg" width="250px;" style="border-radius: 50%;" alt="호진"/>
        <br/><br/>
        <sub><b>호진</b></sub>
        <br/>
        <sub>CTO</sub>
      </a>
    </td>
  </tr>
</table>

<br/>

## About

**따랑해**는 알고리즘이 아닌, **내가 믿는 사람이 직접 소개해주는** 소개팅 서비스입니다.

기존 소개팅 앱의 차가운 알고리즘 대신, 친구가 직접 내 소중한 사람을 소개해주는 따뜻한 경험을 만듭니다.

> *"불완전하지만 진심 어린 추천이, 완벽하지만 차가운 알고리즘을 이긴다."*

<br/>

### How It Works

```
🧑 따랑지기 (소개해주는 사람)
    ↓  내 친구를 등록하고
💕 따랑이 (소개받는 사람)
    ↓  그룹 안에서
🏠 따랑방 (소개팅 그룹)
    ↓  서로의 친구를 소개하면
🔔 따르릉! → 매칭 성공!
```

1. **따랑지기**가 주변의 소중한 친구(**따랑이**)를 등록합니다
2. **따랑방**에 참여해 다른 따랑지기의 따랑이를 확인합니다
3. 마음에 드는 따랑이에게 **따르릉**(매칭 요청)을 보냅니다
4. 상대 따랑지기가 수락하면 **매칭 성공**!

## Tech Stack

<div align="center">

**Backend**

![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-244C5A?style=for-the-badge&logo=google&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React_19-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)

**Mobile**

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?style=for-the-badge&logo=swift&logoColor=white)

**Infra**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

</div>

<br/>

## Architecture

```
┌─────────────┐  ┌─────────────┐
│   Android    │  │     iOS     │
│  (Kotlin)    │  │   (Swift)   │
└──────┬───────┘  └──────┬──────┘
       │    WebView       │
       └────────┬─────────┘
                │
       ┌────────▼────────┐
       │   React SPA     │
       │  (gRPC-Web)     │
       └────────┬────────┘
                │
       ┌────────▼────────┐
       │  Envoy Proxy    │
       └────────┬────────┘
                │
       ┌────────▼────────┐
       │   Go gRPC API   │
       └───┬─────────┬───┘
           │         │
    ┌──────▼──┐  ┌───▼─────┐
    │PostgreSQL│  │  Redis  │
    └─────────┘  └─────────┘
```

<br/>

## Repositories

| Repository | Description |
|:-----------|:------------|
| [**issueisseo**](https://github.com/mileojwo/issueisseo) | 프로젝트 총괄 (기획, 문서, 설계) |
| [issueisseo-mono](https://github.com/mileojwo/issueisseo-mono) | Go 백엔드 + Proto 정의 |
| [issueisseo-web](https://github.com/mileojwo/issueisseo-web) | React 웹 클라이언트 (Nx 모노레포) |
| [issueisseo-android](https://github.com/mileojwo/issueisseo-android) | Android 앱 (Kotlin WebView) |
| [issueisseo-ios](https://github.com/mileojwo/issueisseo-ios) | iOS 앱 (Swift WKWebView) |

<br/>

## How We Work

> 2인 팀의 협업 규칙. 지속적으로 개선한다 (`#how-to-work` 채널).

### 역할 분담

| 역할 | 담당 | 범위 |
|------|------|------|
| 클라이언트 | 준모 | iOS, Android, Web (프론트엔드) |
| 서버 | 호진 | Go 백엔드, DB, 인프라 |
| 공통 | 자유롭게 | 아이디어, 기획, 디자인 |

### 커뮤니케이션 — 디스코드

| 채널 | 역할 | 사용법 |
|------|------|--------|
| `#ideation` | 아이디어 발산 & 논의 | 자유롭게 던지기. 결론 없어도 OK |
| `#planning` | 확정된 아이디어의 디테일 기획 | 결정사항은 스레드로 정리 |
| `#tech` | 기술(개발) 논의 | API 스펙, 아키텍처, 트러블슈팅 |
| `#bug-report` | 버그 제보 & 추적 | 재현 조건 + 스크린샷 첨부 |
| `#how-to-work` | 일하는 방식 논의 & 개선 | 회고, 프로세스 변경 제안 |

### GitHub 작업 방식

**런칭 전 (현재)**
- **master 직접 push 허용** — 속도 우선
- 작업 전 `git pull` 필수 (충돌 방지)
- 큰 작업은 디스코드에 사전 공유
- DB 초기화 & 마이그레이션 자유롭게 진행
- push 시 CI는 계속 실행 (빌드 깨짐 감지)
- **Proto/IDL 변경 시 `#tech`에서 사전 합의** 필요. 단, 클라이언트도 같이 수정하면 합의 스킵 가능

**런칭 후**
- **PR + 리뷰 필수**로 전환
- DB: staging은 자유, production은 **마이그레이션만 허용, 초기화 금지** (유저 데이터 보호)
- 배포: staging 검증 → production 수동 배포 (workflow_dispatch)

### 기획 문서 워크플로우

기획 문서는 `docs/feature-specs/`에 마크다운으로 작성하여 Git으로 관리한다.

```
1. 기획자(제안자)가 docs/feature-specs/ 에 기획 문서를 작성하여 push
2. #planning 채널에 기획 문서를 공유하고 리뷰 진행
3. 피드백을 문서에 반영하여 업데이트
4. 기획 확정 후 각자 개발 진행
```

- 파일명: `{기능명}.md` (예: `compatibility-service.md`)
- 누구나 제안 가능 (공통 업무)
- 리뷰 시 기술적 실현 가능성, 우선순위, 스펙 누락 여부 확인
- 확정된 문서는 개발 중에도 필요 시 업데이트 (변경사항 `#planning`에 공유)

### IDL(Proto) 협업 프로세스

서버-클라이언트 분리 개발의 핵심 접점:

```
1. 기획 확정 (#planning)
2. API 스펙 논의 (#tech) — 필요한 RPC, 요청/응답 필드 정의
3. Proto IDL 작성 & 합의 — 서버 개발자가 초안, 클라이언트 리뷰 (또는 반대)
4. Proto 확정 후 각자 병렬 구현
   - 서버: Go gRPC 구현 (handler → service → repository)
   - 클라이언트: IDL 동기화 → data-access → UI 구현
5. 통합 테스트 (staging 환경)
```

### 태스크 관리 — GitHub Issues

- 레포별 이슈 생성, 라벨로 분류: `feat`, `bug`, `chore`
- 런칭 후 PR과 이슈 연동 (`closes #123`)

<br/>

---

<div align="center">

*Built with love in South Korea* 💕

</div>
