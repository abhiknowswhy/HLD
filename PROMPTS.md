# HLD Interview Solution Prompts

## Prompt 1: Create HLD Interview Solution

For a **1-hour system design interview**, create a comprehensive HLD document following the structure of `Craigslist_Core_Architecture.md`:

1. **Question Clarifications** - Define scope and similar questions
2. **Functional Requirements** - Requirements-to-infrastructure mapping (table format)
3. **Non-Functional Requirements** - Scale, Availability, Performance, Security, Consistency
4. **Capacity Planning & Estimates** - DAU, Storage, RPS, QPS with calculations
5. **Data Model & Schema** - ERD or schema description with indexing strategy
6. **High-Level Architecture** - Diagram reference and service responsibilities
7. **Infrastructure Sizing & Configuration** - Detailed sizing table for each component
8. **Data Flow Paths** - Write, Read, Search, Notifications flows
9. **Storage Strategy** - Primary storage, caching, CDN with TTLs and sizing
10. **Replication & BCDR** - Multi-region strategy with RTO/RPO justification
11. **Security** - Encryption (transit & at-rest), rate limiting, compliance
12. **Technology Choices** - Justify each choice and explain trade-offs
13. **Operational Excellence** - Graceful degradation, S2S communication, monitoring
14. **Additional Discussion Points** - Data retention, rate limiting, compliance, future features

**Output**: Markdown document structured like the Craigslist design (use as template)

---

## Prompt 2: Evaluate HLD Interview Solution

For a **1-hour system design interview**, evaluate the HLD document following the framework in `EVALUATION_AND_IMPROVEMENTS.md`:

**Rating Dimensions (0-10 each):**
- Scalability: Handles estimated load with justified architecture decisions
- Availability & BCDR: Multi-region strategy, failover, RTO/RPO targets
- Security: Encryption (transit/at-rest), rate limiting, compliance
- Performance: Caching, database optimization, search, latency targets
- Data Consistency: Replication strategy, conflict resolution approach
- Cost Optimization: Resource allocation, tiered storage, pricing awareness
- Technology Choices: Each justified with trade-off reasoning
- Operational Excellence: Monitoring, graceful degradation, S2S communication
- Database Design: Schema clarity, indexing, RDBMS vs NoSQL justification
- Complexity Management: Interview-appropriate depth and digestibility

**Output Structure:**
1. Overall rating (X/10) with context
2. Scoring breakdown table (all 10 dimensions)
3. Strengths section - what's working well with specifics
4. Gaps section - organized by priority (Critical → Low)
5. Interview readiness assessment - is it ready to present?
6. Talking points - likely interviewer questions with prepared answers
7. Recommendations - focus areas before interview

**Evaluation Context:**
- 1-hour interview scope, not production system
- Recognize context-appropriate decisions (e.g., no sharding at 5M records)
- Look for reasoning and trade-off awareness, not perfection
- Target rating: 8.5+/10 for interview readiness

---

## Workflow

1. **Create**: Use Prompt 1 on the system design question
2. **Evaluate**: Use Prompt 2 on the generated HLD document
3. **Reference**: Compare structure to `Craigslist_Core_Architecture.md` and `EVALUATION_AND_IMPROVEMENTS.md`
4. **Target**: Aim for 8.5+/10 rating for interview readiness

## Example Systems

YouTube, Uber, Netflix, Twitter, WhatsApp, Instagram, Amazon, Airbnb, Google Maps, Twitch, Discord, Slack, Dropbox, Google Docs, TikTok
