# ABCD Corporation — Software Services Website

## Project Overview
Marketing website for **ABCD Corporation**, a software services company. The site introduces the company, showcases services, displays case studies/portfolio, and drives lead generation through contact forms.

## Goals
- Present ABCD Corporation as a credible, modern software services partner
- Clearly communicate service offerings and differentiators
- Capture qualified leads via contact / "Request a Quote" forms
- Be fast, accessible (WCAG 2.1 AA), and SEO-friendly

## Target Audience
- CTOs, engineering managers, and product leaders evaluating software vendors
- Startups looking for outsourced engineering / MVP development
- Enterprises needing modernization, integrations, or staff augmentation

## Site Structure
| Page | Purpose |
| --- | --- |
| `/` Home | Hero, value proposition, services teaser, social proof, CTA |
| `/services` | Detailed list of service offerings |
| `/services/[slug]` | Individual service detail pages |
| `/industries` | Industries served (FinTech, Healthcare, Retail, etc.) |
| `/case-studies` | Portfolio / client success stories |
| `/case-studies/[slug]` | Individual case study pages |
| `/about` | Company story, leadership, values |
| `/careers` | Open roles, culture |
| `/blog` | Thought leadership articles |
| `/contact` | Contact form, office locations |

## Services to Showcase
- Custom Software Development
- Web & Mobile App Development
- Cloud Engineering (AWS, Azure, GCP)
- DevOps & SRE
- Data Engineering & Analytics
- AI/ML Solutions
- UI/UX Design
- QA & Test Automation
- IT Staff Augmentation

## Tech Stack (suggested — confirm with user before scaffolding)
- **Framework:** Next.js (App Router) + TypeScript
- **Styling:** Tailwind CSS
- **Components:** shadcn/ui or Radix primitives
- **Content:** MDX for blog/case studies, or a headless CMS (Sanity / Contentful) if non-dev editing is required
- **Forms:** React Hook Form + Zod validation; submissions via API route → email service (Resend / SendGrid)
- **Analytics:** Google Analytics 4 + Vercel Analytics
- **Hosting:** Vercel
- **SEO:** Next.js metadata API, sitemap.xml, robots.txt, structured data (JSON-LD)

## Design Direction
- Clean, professional, enterprise-friendly aesthetic
- Primary palette: TBD (placeholder: deep blue + accent teal/orange)
- Typography: Modern sans-serif (Inter, Geist, or similar)
- Imagery: Real team/work photos preferred over generic stock
- Generous whitespace, clear visual hierarchy

## Non-Functional Requirements
- **Performance:** Lighthouse score > 90 on all categories
- **Accessibility:** WCAG 2.1 AA compliance, semantic HTML, keyboard navigation
- **SEO:** Per-page meta tags, OpenGraph, JSON-LD for Organization / Service / Article
- **Responsive:** Mobile-first, tested at 360px, 768px, 1024px, 1440px
- **Privacy:** Cookie consent banner, privacy policy, GDPR-friendly forms

## Development Conventions
- Use TypeScript strict mode
- Prefer Server Components; use Client Components only when interactivity is required
- Co-locate component styles, tests, and stories
- Conventional Commits for commit messages
- Lint + format on pre-commit (ESLint + Prettier)

## Out of Scope (for v1)
- User authentication / customer portal
- E-commerce / payment processing
- Multilingual / i18n (English only at launch)

## Open Questions
- Final brand colors, logo, and typography?
- CMS required, or is MDX-in-repo sufficient?
- Preferred lead-capture destination (email, CRM webhook, HubSpot, Salesforce)?
- Hosting/domain already provisioned?
