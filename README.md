# FestPass — Docker & Container Security Assessment

## Student Details

| Field                     | Value                                           |
| ------------------------- | ----------------------------------------------- |
| **Name**                  | Anuj Gope                                       |
| **Registration Number**   | 202401100200068                                  |
| **PORT**                  | 8068                                             |
| **Docker Hub Username**   | anujgope                                         |
| **Docker Hub Repository** | https://hub.docker.com/r/anujgope/fest-backend   |

## AI Tools Used

| Tool       | Used For                                                        |
| ---------- | --------------------------------------------------------------- |
| Antigravity (Claude / Gemini) | Writing Dockerfile, compose.yaml, fixing vulnerabilities, README |

## Docker Hub Image Digest (1.0.0)

```
sha256:PASTE_DIGEST_HERE
```

## Vulnerability Scan — Before & After (Stage 3.3)

| Metric              | `fest-backend:0.1` (before) | `fest-backend:0.2` (after) |
| -------------------- | --------------------------- | -------------------------- |
| **Base image**       | `python:3.9`                | `python:3.12-slim`         |
| **Image size**       | 1.11GB                      | 140MB                      |
| **CRITICAL**         | 234                         | 0                          |
| **HIGH**             | 2249                        | 44                         |
| **MEDIUM**           | 7530                        | 67                         |
| **LOW**              | 3210                        | 63                         |
| **Non-root user?**   | No                          | Yes                        |

## Steps Not Completed

*(All steps completed)*
