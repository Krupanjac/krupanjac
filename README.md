# `~/krupanjac`

```bash
$ ./whoami.sh
> Initializing backend services...
> Loading profile... 100%
```

### 📡 System Architecture

```mermaid
graph LR
    Client(User) -- HTTPS --> LB{Load Balancer}
    LB -- /GET profile --> API[krupanjac-api]
    API -- Query --> DB[(Skills DB)]
    DB -- Result --> API
    API -- JSON --> Client
    style API fill:#1f2020,stroke:#fff,stroke-width:2px,color:#fff
    style DB fill:#1f2020,stroke:#fff,stroke-width:2px,color:#fff
    style LB fill:#1f2020,stroke:#fff,stroke-width:2px,color:#fff
    style Client fill:#1f2020,stroke:#fff,stroke-width:2px,color:#fff
```

### 💾 HTTP Response

```http
HTTP/1.1 200 OK
Content-Type: application/json
X-Powered-By: Coffee
Date: Mon, 01 Jan 2026 12:00:00 GMT
```

```json
{
  "data": {
    "id": "krupanjac",
    "type": "Backend Engineer",
    "attributes": {
      "intelligence": "Artificial & Natural",
      "languages": ["Python", "Go", "Rust", "SQL"],
      "infrastructure": ["Docker", "Kubernetes", "AWS", "Linux"],
      "database": ["PostgreSQL", "Redis", "MongoDB"],
      "status": "Building scalable systems",
      "location": "127.0.0.1"
    },
    "links": {
      "github": "https://github.com/krupanjac",
      "linkedin": "https://linkedin.com/in/krupanjac"
    }
  }
}
```

### 🛠️ `sudo apt-get install skills`

![Python](https://img.shields.io/badge/python-3670A0?style=flat-square&logo=python&logoColor=ffdd54)
![Go](https://img.shields.io/badge/go-%2300ADD8.svg?style=flat-square&logo=go&logoColor=white)
![Rust](https://img.shields.io/badge/rust-%23000000.svg?style=flat-square&logo=rust&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=flat-square&logo=docker&logoColor=white)
![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=flat-square&logo=postgresql&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

### 📝 `tail -f /var/log/dev.log`

```diff
+ 🔭 I’m currently working on High availability distributed systems
+ 🌱 I’m currently learning eBPF and Kernel tuning
+ 👯 I’m looking to collaborate on Open Source Backend Tooling
! ⚡ Fun fact: I dream in JSON.
```

<details>
<summary><b>🛑 sudo systemctl status motivation</b></summary>

```ini
● motivation.service - Daily Coding Drive
   Loaded: loaded (/lib/systemd/system/motivation.service; enabled; vendor preset: enabled)
   Active: active (running) since Mon 2026-01-01 08:00:00 UTC; 4h 20min ago
 Main PID: 1337 (brain)
    Tasks: 42 (limit: 4915)
   Memory: 99.9%
   CGroup: /system.slice/motivation.service
           └─1337 /usr/bin/brain --focus=backend --coffee=true
```
</details>

---
```console
krupanjac@github:~$ exit
logout
Connection to localhost closed.
```
