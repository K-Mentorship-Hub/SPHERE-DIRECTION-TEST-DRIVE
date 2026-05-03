# Quest 3 — Cybersecurity & Infrastructure

**Sphere:** T | **Time:** 2-4 hours | **Difficulty:** Beginner-friendly

---

## Scenario

You're the first security-conscious person at a 10-person startup. Nobody has thought about security — passwords are shared, servers are open, and the CEO thinks "we're too small to be a target." Your job: audit what you can and create a security improvement plan.

---

## Theory Bite

Cybersecurity and infrastructure are about **protecting systems and keeping them running**. The mindset:

1. **Think like an attacker** — what would you break into?
2. **Think like an operator** — what keeps things alive when things go wrong?
3. **Think like an architect** — how do you design systems that are resilient by default?

Daily reality: it's less "hacking in movies" and more "reading logs, writing policies, patching systems, and convincing people to take risks seriously."

Key areas: network security, access control, incident response, infrastructure automation (DevOps/SRE), compliance

---

## Hands-On Task

### Part 1: Password Audit (30 min)

Check the passwords you personally use (don't share them!). Rate each one:
- Length (under 8 chars = weak)
- Complexity (mix of upper/lower/numbers/symbols?)
- Reuse (do you use it in multiple places?)

Calculate your personal "password hygiene score":
- 5+ unique, strong passwords = Good
- 3-4 = Needs improvement
- 1-2 reused everywhere = Critical

### Part 2: Threat Model a Small Company (45 min)

Pick a real or imaginary small company. Create a threat model document:

| Asset | Threat | Likelihood | Impact | Mitigation |
|-------|--------|------------|--------|------------|
| Customer database | SQL injection | Medium | High | Parameterized queries |
| Employee laptops | Physical theft | Low | High | Full-disk encryption |
| ... | ... | ... | ... | ... |

List at least 5 assets and their threats.

### Part 3: Security Checklist (45 min)

Create a "Startup Security Starter Checklist" with 3 priority levels:

**Critical (do today):**
- Enable 2FA on all accounts
- Use a password manager
- Close unused cloud ports

**Important (do this week):**
- Set up automated backups
- Review who has admin access
- Enable audit logging

**Nice to have (do this month):**
- Create an incident response plan
- Set up a VPN for remote access
- Schedule monthly security reviews

### Part 4: Infrastructure Diagram (30 min)

Draw a simple infrastructure diagram for a web application:
- Users → Load Balancer → Web Servers → Database
- Show where security controls go (firewall, WAF, encryption)

Use any tool: paper, draw.io, Excalidraw, or ASCII art.

<details>
<summary>Stuck? Click here for ASCII diagram example</summary>

```
                    ┌─────────────┐
                    │   Firewall   │
                    └──────┬──────┘
                           │
                    ┌──────▼──────┐
                    │  Load Bal.  │
                    └──────┬──────┘
                      ┌────┴────┐
               ┌──────▼──┐  ┌───▼──────┐
               │ Web Srv1 │  │ Web Srv2 │
               └──────┬──┘  └───┬──────┘
                      └────┬────┘
                    ┌──────▼──────┐
                    │   Database   │
                    │  (encrypted) │
                    └─────────────┘
```

</details>

---

## Reflection Questions

- Did you enjoy thinking about what could go wrong?
- Was the threat modeling analytical or anxiety-inducing?
- Do you prefer the "protect" side (security) or the "build and run" side (infrastructure)?
- Could you see yourself convincing non-technical people to care about security?

---

## Verdict

| If this describes you | Flag |
|-----------------------|------|
| You started threat-modeling things beyond the task | Green |
| You enjoyed the checklist and policy writing | Green |
| You found it interesting but too abstract | Yellow |
| You wanted to build things, not protect them | Yellow (maybe Quest 2 instead) |
| Thinking about threats made you anxious, not engaged | Red |
