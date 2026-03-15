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

<br/>

## Team

<table align="center">
  <tr>
    <td align="center">
      <a href="https://github.com/lmalma2004">
        <img src="./assets/junmo-profile.jpg" width="150px;" style="border-radius: 50%;" alt="준모"/>
        <br/>
        <sub><b>준모</b></sub>
        <br/>
        <sub>CEO</sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/solone313">
        <img src="./assets/hojin-profile.jpg" width="150px;" style="border-radius: 50%;" alt="호진"/>
        <br/>
        <sub><b>호진</b></sub>
        <br/>
        <sub>CTO</sub>
      </a>
    </td>
  </tr>
</table>

<br/>

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

---

<div align="center">

*Built with love in South Korea* 💕

</div>
