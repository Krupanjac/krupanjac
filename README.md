# `class Krupanjac extends SoftwareEngineer`

```typescript
/**
 * Arsen Đurđev (Krupanjac)
 * Fullstack Systems Architect & Performance Engineer
 */
interface EngineerProfile {
    core: {
        languages: ["TypeScript", "C++", "Python", "Go"];
        backend: ["Node.js", "Microservices", "gRPC", "PostgreSQL"];
        systems: ["OpenGL", "Memory Optimization", "Multi-threading"];
        frontend: ["React", "Next.js", "WebGL"];
    };
    focus: "Building scalable, high-performance distributed systems";
    status: "Compiling...";
}

const me: EngineerProfile = {
    // ...initializing dependencies
};
```

### 📡 System Architecture

```mermaid
graph TD
    User((Client)) -->|HTTPS/WSS| LB{Load Balancer}
    LB -->|Routing| Gateway[API Gateway]
    
    subgraph Services [Backend Cluster]
        Gateway -->|gRPC| Auth[Auth Service]
        Gateway -->|REST| Core[Core API]
        Gateway -->|Socket| Realtime[Realtime Svc]
        
        Core -->|Write| PrimaryDB[(PostgreSQL)]
        Core -->|Read| ReadReplica[(PostgreSQL - Read)]
        Realtime -->|Pub/Sub| Redis[(Redis Cache)]
    end
    
    subgraph Native [High Performance]
        Engine[C++ Voxel Engine] <-->|FFI| Core
        GPU[OpenGL/Vulkan] <--> Engine
    end

    style Services fill:#1e1e1e,stroke:#333,stroke-width:2px,color:#fff
    style Native fill:#1e1e1e,stroke:#d07a16,stroke-width:2px,color:#fff
    style Gateway fill:#2d699e,stroke:#fff,stroke-width:0px,color:#fff
```

### 🛠️ Technology Stack

| Domain | Technologies |
|:--- |:--- |
| **Backend & Cloud** | ![NodeJS](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=node.js&logoColor=white) ![Go](https://img.shields.io/badge/-Go-00ADD8?style=flat-square&logo=go&logoColor=white) ![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Postgres](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/-Redis-DC382D?style=flat-square&logo=redis&logoColor=white) |
| **Systems & Native** | ![C++](https://img.shields.io/badge/-C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white) ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) ![OpenGL](https://img.shields.io/badge/-OpenGL-FFFFFF?style=flat-square&logo=opengl) ![Bash](https://img.shields.io/badge/-Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white) |
| **Frontend & Web** | ![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black) ![HTML5](https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) ![SASS](https://img.shields.io/badge/-SASS-CC6699?style=flat-square&logo=sass&logoColor=white) |

### 📊 Repository Analytics

<div align="left">
  <img src="https://github-readme-stats.vercel.app/api?username=Krupanjac&show_icons=true&theme=transparent&hide_border=true&title_color=3178C6&text_color=8b949e&icon_color=3178C6&count_private=true&include_all_commits=true" height="150" alt="stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Krupanjac&layout=compact&theme=transparent&hide_border=true&title_color=3178C6&text_color=8b949e&icon_color=3178C6&hide=css,html,shell" height="150" alt="languages" />
</div>

### 💾 Selected Works

```json
[
  {
    "project": "minecraft-cpp",
    "type": "Game Engine",
    "stack": ["C++", "OpenGL", "GLSL"],
    "description": "High-performance voxel rendering engine with custom memory allocators."
  },
  {
    "project": "gyst-ecosystem",
    "type": "Fullstack Platform",
    "stack": ["Node.js", "TypeScript", "Swift"],
    "description": "Distributed backend systems for mobile application synchronization."
  }
]
```

<!-- Footer -->
<div align="right">
  <code>echo "contact: linked/in/krupanjac" >> /dev/null</code>
</div>