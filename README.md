<div align="center">

<!-- Dynamic Typing Header -->
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=32&duration=2800&pause=1200&color=58A6FF&center=true&vCenter=true&width=600&lines=Hey+there!+I'm+Rasel+Shah+%F0%9F%91%8B;Software+Engineer;Full+Stack+Engineer;Open+to+Collaborate+%F0%9F%A4%9D" alt="Typing SVG" />

<br/>
<br/>


<img src="./boot.svg" alt="rasel@production — Software Engineer, service running, 4+ years uptime" width="100%"/>

<br/><br/>

<img src="https://img.shields.io/badge/version-4.2.0-58a6ff?style=flat-square&labelColor=0d1117" alt="version"/>
<img src="https://img.shields.io/badge/build-passing-3fb950?style=flat-square&labelColor=0d1117" alt="build passing"/>
<img src="https://img.shields.io/badge/uptime-4%2B_years-3fb950?style=flat-square&labelColor=0d1117" alt="uptime 4+ years"/>
<img src="https://img.shields.io/badge/region-Dhaka_·_UTC%2B6-8b949e?style=flat-square&labelColor=0d1117" alt="region Dhaka UTC+6"/>
<a href="https://github.com/Raselshah"><img src="https://komarev.com/ghpvc/?username=Raselshah&label=requests&color=1f6feb&style=flat-square" alt="profile views"/></a>

</div>

<img src="./divider.svg" width="100%"/>

## `GET /about`

```jsonc

{
  "name": "Rasel Shah",
  "role": "Software Engineer",
  "experience": "4+ years",
  "location": "Bangladesh 🇧🇩",
  "specialty": "turning vague requirements into systems that survive traffic",
  "currently": {
    "building": "scalable full-stack applications",
    "learning": ["system design", "microservices", "cloud architecture"],
    "reading":  "logs, mostly"
  },
  "principles": [
    "First, solve the problem. Then, write the code.",
    "Boring technology, interesting problems.",
    "If it isn't measured, it isn't fast."
  ],
  "openTo": ["collaboration", "open source", "hard problems"]
}
```

<img src="./divider.svg" width="100%"/>

## `GET /architecture`

The kind of system I spend my days inside — client to event bus to worker, and back out over a socket.

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#161b22','primaryTextColor':'#c9d1d9','primaryBorderColor':'#30363d','lineColor':'#58a6ff','secondaryColor':'#161b22','tertiaryColor':'#0d1117','fontFamily':'monospace','clusterBkg':'#0d1117','clusterBorder':'#21262d'}}}%%
flowchart LR
    U([Client · Next.js]) -->|REST| GW[API Gateway]
    U <-->|WebSocket| RT[Realtime Layer]
    GW --> AUTH[Auth Service]
    GW --> API[Core API · NestJS]
    API <--> PG[(PostgreSQL · Prisma)]
    API <--> MG[(MongoDB)]
    API --> BUS{{Event Bus}}
    BUS --> WRK[Workers · jobs, mail, reports]
    BUS --> RT
    subgraph CD [ship it]
        DOC[Docker] --- AWS[AWS]
    end
    WRK -.-> CD
```

<img src="./divider.svg" width="100%"/>

## `GET /endpoints`

| Method | Endpoint | Returns | Status |
| :--- | :--- | :--- | :--- |
| `GET` | `/skills/frontend` | React · Next.js · TypeScript · Redux · Tailwind | `200 OK` |
| `GET` | `/skills/backend` | Node.js · Express · NestJS · REST · WebSockets | `200 OK` |
| `GET` | `/skills/data` | PostgreSQL · MongoDB · Prisma | `200 OK` |
| `GET` | `/skills/infra` | Docker · AWS · Git · CI | `200 OK` |
| `GET` | `/learning` | system design · microservices · event-driven architecture | `206 Partial Content` |
| `POST` | `/collaborate` | open source, side projects, ideas worth building | `202 Accepted` |
| `POST` | `/hire` | full-time and contract enquiries | `202 Accepted` |
| `DELETE` | `/tech-debt` | refactors, DRY passes, performance work | `204 No Content` |
| `GET` | `/free-time` | — | `503 Service Unavailable` |

<img src="./divider.svg" width="100%"/>

## `GET /dependencies`

```jsonc
{
  "name": "@rasel/full-stack-engineer",
  "version": "4.2.0",
  "main": "problem-solving.ts",
  "engines": { "curiosity": ">=1.0.0", "coffee": "^2 cups/day" },
  "dependencies": {
    "typescript": "^5.x",
    "react": "^19.x",
    "next": "^15.x",
    "nestjs": "^11.x",
    "express": "^4.x",
    "prisma": "^6.x",
    "postgresql": "*",
    "mongodb": "*"
  },
  "devDependencies": {
    "docker": "*",
    "aws": "*",
    "git": "*",
    "python": "^3.x"
  },
  "scripts": {
    "start": "first, solve the problem",
    "build": "then, write the code",
    "test":  "then, prove it under load"
  }
}
```

<div align="center">
  <br/>
  <img src="https://skillicons.dev/icons?i=ts,js,react,nextjs,redux,tailwind,nodejs,express,nestjs,python&theme=dark" alt="languages and frameworks"/>
  <br/><br/>
  <img src="https://skillicons.dev/icons?i=postgres,mongodb,prisma,docker,aws,git,github,vscode&theme=dark" alt="data and infrastructure"/>
</div>

<img src="./divider.svg" width="100%"/>

## `GET /metrics`

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=Raselshah&show_icons=true&hide_border=true&include_all_commits=true&count_private=true&bg_color=0d1117&title_color=58a6ff&icon_color=1f6feb&text_color=8b949e" alt="GitHub stats"/>
<img height="170" src="https://streak-stats.demolab.com?user=Raselshah&hide_border=true&background=0d1117&stroke=21262d&ring=58a6ff&fire=e3b341&currStreakLabel=58a6ff&sideLabels=8b949e&dates=8b949e&currStreakNum=c9d1d9&sideNums=c9d1d9" alt="contribution streak"/>

<br/><br/>

<img height="150" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Raselshah&layout=compact&langs_count=8&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=8b949e" alt="most used languages"/>

</div>

### `tail -f /var/log/commits`

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Raselshah&hide_border=true&bg_color=0d1117&color=58a6ff&line=1f6feb&point=c9d1d9&area=true&area_color=1f6feb&custom_title=commit%20throughput%20·%20last%2031%20days" width="100%" alt="commit activity graph"/>
</div>

<img src="./divider.svg" width="100%"/>

## `GET /changelog`

> **`v4.2.0`** — *current*
> Deep in system design. Splitting monoliths, designing event-driven flows, and getting serious about observability.

> **`v4.0.0`** — production scale
> Shipped full-stack products end to end: REST APIs, WebSocket realtime layers, Postgres schema design with Prisma, containerised deploys on AWS.

> **`v2.0.0`** — the backend turn
> Moved from UI work into Node, Express and NestJS. Learned that most frontend problems are actually API design problems.

> **`v1.0.0`** — first commit
> React, curiosity, and far too much `console.log`.

<img src="./divider.svg" width="100%"/>

## `GET /sla`

| Metric | Target |
| :--- | :--- |
| First response | under 24 hours |
| Peak hours | 10:00 – 02:00 (UTC+6) |
| Preferred protocol | LinkedIn · email |
| Rate limit | 2 side projects concurrent |
| Accepts | code review, pair debugging, architecture arguments |
| Rejects | "make it like Facebook, budget is $50" |

<img src="./divider.svg" width="100%"/>

## `POST /subscribe`


<div align="left">

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Raselshah)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/md-rasel-shah-b085a6228/)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/MdRaselShah5)
[![Facebook](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/mdrasel.shah.92505/)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=firefox-browser&logoColor=white)](https://raselshah.vercel.app/)

</div>

---

## 💡 Dev Philosophy

<div align="center">

> *"First, solve the problem. Then, write the code."*
>
> — clean code · scalable systems · continuous learning

</div>


<br/>

<div align="center">
  <img src="./footer.svg" width="100%"/>
</div>


<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:58A6FF,100:1F6FEB&height=90&section=footer&text=Thanks+for+visiting!&fontSize=16&fontColor=ffffff&fontAlignY=65" />


</div>
