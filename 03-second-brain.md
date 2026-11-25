# Most2baly Second Brain: Week 4

Tag format: `[week] [source] [topic] [priority]`

## 1. Key Decisions Taken

- Move mentor session booking to a new redesigned page instead of patching the old one. `[W4] [standup] [mentor-booking] [priority: medium]`
- Escalate the payment webhook issue to the payment provider instead of fixing it internally. `[W4] [standup] [payments] [priority: high]`
- Launch the new onboarding flow on Thursday after QA approval. `[W4] [standup] [onboarding] [priority: high]`
- Add caching to the cohort dashboard to fix slow load for large cohorts. `[W4] [standup] [dashboard] [priority: medium]`

## 2. Action Items & Owners

| Action | Owner | Due | Status | Tags |
|--------|-------|-----|--------|------|
| Email 40 students who never finished profile setup | Nour | Wed | Planned | `[engagement]` `[priority: medium]` |
| Fix payment webhook timeout (via provider escalation) | Ahmed | Wed | Done (Fri) | `[bug]` `[payments]` `[priority: high]` |
| Prepare onboarding launch announcement post | Hana | Thu | Planned | `[marketing]` `[priority: medium]` |
| Implement cohort dashboard caching | Karim | Fri | Done | `[performance]` `[priority: medium]` |
| Deliver design for mentor booking page | Layla | Next Tue | In progress | `[design]` `[priority: medium]` |
| Fix certificate PDF name order | Unassigned | No date | Open | `[bug]` `[certificates]` `[priority: high]` |
| Build mobile-friendly progress tracker | Unassigned | No date | Open | `[feature]` `[priority: low]` |
| Fix late session reminders | Unassigned | No date | Open | `[bug]` `[mentors]` `[priority: high]` |

## 3. Operational Bottlenecks

- Payment webhook timeouts blocked 3 students from enrolling (reported in 1 source, resolved Friday after provider patch). `[payments] [priority: high]`
- Certificate PDF shows the wrong name order, reported by 12 students, no owner yet. `[certificates] [priority: high]`
- Google login blank screen affected 5 students after the update (hotfix v2.4.1 released Friday). `[login] [priority: high]`
- Session reminders reach mentors after sessions have already started (mentor feedback, no owner). `[mentors] [priority: high]`
- Mentor booking redesign is waiting on design delivery. `[design] [priority: medium]`
- Cohort dashboard was slow for large cohorts before caching. `[performance] [priority: medium]`

## 4. Product & Platform Updates

- v2.4.0: new onboarding flow with checklist released Thursday; students and mentor Youssef reported positive feedback. `[onboarding]`
- v2.4.1 hotfix: fixed Google login blank screen, released Friday. `[login]`
- Internal: cohort dashboard caching added, load time dropped significantly. `[performance]`
- Planned: mentor booking page redesign next week. `[mentor-booking]`
- Requested features: mobile-friendly progress tracker, "missed previous session" view for mentors. `[feature-requests]`

## Questions this knowledge base can answer

1. **What are the top 3 technical bugs reported this week and who is fixing them?**
   Certificate name order (12 reports, unassigned), Google login blank screen (5 reports, fixed in v2.4.1), payment webhook timeout (3 students blocked, Ahmed, fixed after provider patch).
2. **Which blockers have no owner?** Certificate PDF name order, late session reminders, and the mobile progress tracker request.
3. **What did mentors ask for this week?** Earlier session reminders and a view of students who missed the previous session.
