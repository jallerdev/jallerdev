## Luis G. Jaller

**Platform / Cloud Engineer** · Cartagena, Colombia

I build and operate production infrastructure on AWS, defined as code. Three and a half
years across cloud platform work, backend services, and the pipelines that ship them.

Currently full stack engineer at **[InvitiApp](https://invitiapp.com)** — Next.js on AWS
Lambda, S3 and CloudFront.

---

### What I actually do

**Infrastructure as code.** Built a Terraform codebase from zero: 8 modules — `vpc`,
`rds`, `ecs`, `ecr`, `alb`, `ec2`, `secretmanager`, `frontend` — declaring **45 AWS
resource types** across three environments, driven by per-environment `tfvars`.

**CI/CD.** **5 GitHub Actions pipelines** covering infrastructure plan/apply, API and
frontend, with deploy-time secrets read from AWS Secrets Manager and scoped per
environment. Also Jenkins and Octopus Deploy.

**Cost decisions with the invoice open.** Chose ECS on Fargate over EKS after breaking
the bill down component by component: the control plane alone cost more than the rest of
the project's infrastructure.

**Observability as code.** New Relic alert policies declared in Terraform and routed to a
Teams channel. CloudWatch for logs and metrics. IAM roles scoped per service and per
environment.

---

### Stack

| | |
|---|---|
| **AWS** | EC2 · ECS/Fargate · Lambda · Step Functions · API Gateway · S3 · VPC · RDS · DynamoDB · SQS · EventBridge · CloudWatch · IAM · Secrets Manager |
| **IaC & delivery** | Terraform · Docker · Kubernetes · Helm · GitHub Actions · Jenkins · Octopus Deploy · Nginx · Linux |
| **Backend** | TypeScript · Node.js · NestJS · Hono · PostgreSQL (Drizzle, Row Level Security) · Redis |
| **Frontend** | Next.js 15 · React 19 · Tailwind CSS |

---

### Built on my own

**[Hummik](https://hummik.com)** — WhatsApp scheduling for businesses in Colombia. pnpm
monorepo, ports and adapters with an I/O-free core. Real multi-tenancy: tenant resolved
from a verified JWT claim plus Postgres Row Level Security. Serverless on AWS with SST v3
— Hono on Lambda, SQS with dead-letter queues, crons. **841 tests**, most of them over
pure logic.

**[HalcónOS](https://halcon.jvagencia.com)** — CRM with lead discovery over the Google
Places API. Next.js 15, tRPC, Drizzle, multi-tenant with organization-scoped RBAC
enforced at the tRPC layer. Separate Python + Playwright scraping service.

---

### Reach me

**[Portfolio](https://jaller-dev.vercel.app)** · **[LinkedIn](https://linkedin.com/in/jallerdev)** · jallerangel06@gmail.com
