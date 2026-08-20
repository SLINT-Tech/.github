# Governance

How SLINT Tech is organized, and how that maps onto this GitHub organization.

SLINT Tech is the operating name of **Selfless Leadership & Innovation for a New Tomorrow LBG**,
a company limited by guarantee incorporated in the Republic of Ghana under the Companies Act,
2019 (Act 992), Reg. No. CG014410225. Our full **Constitution** is the authoritative document;
this page is a plain summary of the parts that affect work done here.

## The Board

The Board sets strategy, approves major financial and operational decisions, and reviews
organizational performance annually. It is organized into eight offices:

| Office | Remit |
| --- | --- |
| **Leadership** | Strategy, direction, public representation |
| **Operations** | Day-to-day operations and human resources |
| **Programs & Curriculum** | Learning paths, career cells, curriculum |
| **Community Outreach & Membership** | Recruitment of members, community engagement |
| **Finance & Administration** | Budget, records, secretariat |
| **Communications & Media** | Comms, marketing, media, design |
| **Mentorship & Member Development** | Mentor programs, member growth |
| **Recruitment** | Employer partnerships, job placement |

### Decision-making

- **Quorum** — two-thirds of Board members present.
- **General decisions** — majority vote.
- **Constitutional amendments** — unanimous Board consent, plus the Founder's final consent.
- **Removing a leader** — a two-thirds majority vote.

The Founder holds reserved powers under Article IV of the Constitution, including authority over
the mission and values, appointment and removal of Board members, a veto over constitutional
amendments and structural changes, and the role of final arbiter in unresolved disputes.

## Career Cells

Technical work happens in **career cells**. Each cell covers one career path, is led by a **Cell
Leader**, and runs weekly lessons, projects, and showcases. Cell Leaders report progress to the
Office of Programs and Curriculum.

`Software Engineering` · `Frontend Development` · `Backend Development` · `Cybersecurity`
`Cloud Computing` · `Data Analysis` · `Data Science` · `AI & Machine Learning`

## How This Maps to GitHub

The Board governs the whole organization, but most of it never touches a repository — Finance,
Recruitment, and HR do their work in email, documents, and meetings. So GitHub teams mirror the
**career cells**, where the code actually lives, rather than the board offices.

```
@SLINT-Tech/cells                      parent team — every career cell
  ├── @SLINT-Tech/software-engineering   architecture, testing, delivery
  ├── @SLINT-Tech/frontend               HTML, CSS, JavaScript, TypeScript, React
  ├── @SLINT-Tech/backend                APIs, databases, server-side systems
  ├── @SLINT-Tech/cybersecurity          secure coding, app and network security
  ├── @SLINT-Tech/cloud                  cloud platforms, containers, CI/CD
  ├── @SLINT-Tech/data-analysis          SQL, dashboards, business intelligence
  ├── @SLINT-Tech/data-science           statistics, Python, applied data science
  └── @SLINT-Tech/ai-and-ml              machine learning, deep learning, applied AI

@SLINT-Tech/cell-leaders               every Cell Leader — announcements, cross-cell coordination
@SLINT-Tech/maintainers                cross-cutting reviewers with write access
```

Mention a team to pull the right people into a review: `@SLINT-Tech/backend`.

### Repository roles

| Role | Who | Can |
| --- | --- | --- |
| **Owner** | Founder & Executive Director, Co-Founder & Deputy Director | Everything, including organization settings and billing |
| **Maintainer** | `@SLINT-Tech/maintainers`, and Cell Leaders on their own cell's repositories | Merge pull requests, manage issues, cut releases |
| **Member** | All verified members, through their cell team | Read all repositories, open issues and pull requests |
| **Outside collaborator** | Invited partners and volunteers | Access to specific repositories only |

New members default to **read**. Write access is granted through a cell team, never to an
individual — that way access follows the person's role and is removed when the role changes.

Current grants:

| Team | Repository | Permission |
| --- | --- | --- |
| `@SLINT-Tech/maintainers` | `slinttech.org` | write |
| `@SLINT-Tech/maintainers` | `.github` | admin |
| `@SLINT-Tech/frontend` | `slinttech.org` | write |
| `@SLINT-Tech/cells` | `slinttech.org` | read |
| `@SLINT-Tech/cells` | `.github` | read |

### Who approves what

| Change | Approver |
| --- | --- |
| Code in a cell's project repository | A maintainer of that cell |
| Curriculum or learning-path content | The Cell Leader, with the Office of Programs & Curriculum |
| Anything in `.github` (organization-wide defaults) | `@SLINT-Tech/maintainers` or an owner |
| Public-facing website content | Office of Communications & Media, via an owner |
| Creating, archiving, or deleting a repository | An organization owner |
| Adding a new organization owner | Founder & Executive Director |

Offices that do not appear here still direct the work — they simply do it off GitHub, and an
owner carries the decision into the repository.

## Becoming a Leader

Under Article III of the Constitution, leadership candidates must have been active members for at
least six (6) months, demonstrate alignment with our mission and values, and hold skills relevant
to the role. Nominations — including self-nominations — are submitted through the official
website, shortlisted by the Board, and decided by interview and majority Board vote. Appointees
sign a Leadership Agreement.

## Amending This Document

Open a pull request against this repository and request review from
[@SLINT-Tech/leadership](https://github.com/orgs/SLINT-Tech/teams/leadership). Changes that alter
governance in substance — not just wording — require Board approval, and this page can never
contradict the Constitution.

*Questions about governance: [administration@slinttech.org](mailto:administration@slinttech.org)*
