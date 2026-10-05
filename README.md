# Daeseong (Dennis) Yu

### Backend Software Engineer | Go · TypeScript · AWS Serverless · CI/CD

Backend and cloud developer who builds and operates production systems, from C-based device integrations on nationwide highway infrastructure to AWS serverless APIs in TypeScript and Go.

📍 Kitchener, Ontario · Authorized to work in Canada · Open to relocation within Canada and to remote roles

[LinkedIn](https://linkedin.com/in/daeseong-yu) · [Blog](https://daeseong-yu.github.io/) · [Email](mailto:daeseong.ca@gmail.com)

---

## Background

My professional work has been on two kinds of production systems: toll-collection and roadside equipment software on Korean expressways (C on Unix, sockets and serial links), and the AWS serverless backend of a cloud-connected dashcam service (TypeScript, Go, Lambda).

- Made production APIs **8–10× faster** by tracing a latency bottleneck to AWS credential retrieval and adding caching
- Cut log-management costs by **65%+** by standardizing AWS Lambda logging and building Datadog/Grafana dashboards
- Helped migrate legacy PHP and Go APIs from EC2 to **AWS Lambda** without service disruption

Full work history is on [LinkedIn](https://linkedin.com/in/daeseong-yu).

---

## Projects

### [embedded-rust](https://github.com/Daeseong-Yu/embedded-rust) · in progress

A telemetry pipeline built from the microcontroller up: STM32 firmware → edge gateway → Go API on AWS Lambda → PostgreSQL.

**Rust (`no_std`) · Embassy · defmt · STM32F303 · GitHub Actions**

- Async firmware on the Embassy executor with an interrupt-driven button, task-to-task signalling, and UART output
- CI formats, lints, and cross-compiles the firmware on every push
- Gateway, backend, and Terraform-managed infrastructure are planned; the README tracks what is done
- Write-ups on the [blog](https://daeseong-yu.github.io/)

### [cloud-monitoring](https://github.com/Daeseong-Yu/cloud-monitoring)

A monitoring stack that collects AWS CloudWatch metrics into PostgreSQL, so Grafana dashboards never query CloudWatch directly and dashboard views don't drive API costs.

**Go · PostgreSQL · Grafana · Docker Compose · systemd · GitHub Actions**

- Go collector with resource discovery for EC2, Lambda, API Gateway, Amplify, SES, and S3
- Alerting, summary rollups, and retention run as scheduled one-shot jobs
- Backup, restore, and migration scripts, with deployment and rollback through GitHub Actions

### [QDoc](https://github.com/Daeseong-Yu/QDoc) · ConHack 2026

Clinic check-in and queue management: patients check in before they arrive and get notified when their turn is close.

**TypeScript · Next.js · Node.js · Prisma · PostgreSQL · Redis · Docker · AWS (EC2, S3, Systems Manager)**

- Monorepo with web, API, and worker apps that share Zod contracts
- Notifications go through a database-backed outbox, so status changes survive email failures and retries
- GitHub Actions builds the image, uploads it to S3, and deploys through Systems Manager Run Command

### Canadian Immigration Tracker · [Live demo](https://draw-tracker.nomaduub.com)

Tracks Canadian immigration draws, including Express Entry and Ontario programs.

**Go · React · Vite · AWS · Tailwind CSS**

- Designed the backend API and data model for structured draw data
- Built a responsive interface for exploring historical draws and trends

---

## Skills

| | |
|---|---|
| **Languages** | Go, TypeScript, JavaScript, C, SQL, PHP, Rust (embedded, `no_std`) |
| **Backend & APIs** | Node.js, Express.js, NestJS, Gin, REST APIs, JWT authentication, Stripe |
| **Cloud & DevOps** | AWS (Lambda, API Gateway, S3, CloudFront, SQS, CloudWatch), Serverless Framework, AWS SAM, Docker, GitHub Actions |
| **Databases** | PostgreSQL, MySQL, Oracle, MongoDB |
| **Systems & Observability** | Linux/Unix, Datadog, Grafana, TCP/IP sockets, serial communication |

