# Tenant Backup page graphics

For `https://www.arjdistribution.se/en/m365-configuration-backup` (EtherInsights Tenant Backup).

Delivered by Ryan Mangan (EfficientEther) 16 Nov 2026. Draft confirmed go-ahead 16 Nov 2026. All seven are 2x resolution — display at 760 px wide (height auto) inside ARJ's content column.

| File | Display | Where on the page |
|---|---|---|
| `01-hero.png` | 1520×760 | Under the intro, before "This is not a content backup" |
| `02-two-backups.png` | 1520×820 | After "A customer … needs both" |
| `03-what-is-captured.png` | 1520×960 | Under "What is protected" |
| `04-restore.png` | 1520×600 | Under "Restore" |
| `05-storage.png` | 1520×640 | Under "Storage and licence" |
| `06-drift.png` | 1520×1120 | Under the drift paragraph |
| `07-link-share.png` | 1200×627 | Open Graph / LinkedIn share card (page metadata) |

## Alt text (for `<img alt="">`)

- **01-hero.png** — EtherInsights Tenant Backup. A Microsoft 365 setting changed. Put it back. EtherInsights Tenant Backup saves your tenant's configuration and restores supported settings to the same tenant. Beside it, the EtherInsights Tenant Drift screen for a sample company: 7 things changed since you saved your copy, 1 restore waiting for approval, Tenant Backup enabled daily with 93 backups kept.
- **02-two-backups.png** — A Microsoft 365 tenant needs two backups. One keeps what people made, the other keeps how the tenant is set up. Content backup, your existing Microsoft 365 backup: files and documents, mail, Teams chats. Configuration backup, EtherInsights Tenant Backup: Microsoft Entra identity and directory; applications and consent; Exchange Online and Microsoft Purview; Microsoft Intune and Microsoft Teams.
- **03-what-is-captured.png** — What a snapshot captures. Saved to storage you own; areas without the right licence show as not applicable. Microsoft Entra: identity and directory settings and relationships. Applications and consent: app registrations and enterprise app consent; secret values are never captured. Exchange Online and Microsoft Purview: settings on existing Exchange objects; some Purview settings are backup only. Microsoft Intune and Microsoft Teams: Intune settings with their targeting; Teams configuration is recorded. Restore support differs by area. Deleted objects are only recreated where the workload supports it safely.
- **04-restore.png** — Restore in four steps, into the same tenant. 1, open the backup: pick the snapshot to restore from. 2, choose the scope: only the settings you select. 3, confirm the plan: review it, then run the restore. 4, check the result: see what was put back. A recovery point is taken before anything is written, and kept for at least 180 days.
- **05-storage.png** — Snapshots stay in storage you own. The customer or the MSP holds the storage contract. Azure Blob Storage, in the storage owner's Azure subscription. Impossible Cloud Object Storage, a separate subscription; ask ARJ about availability. Strict immutable storage is there when a customer wants it.
- **06-drift.png** — Pin a known-good copy. Checked every 6 hours. Tenant Drift shows what changed, who changed it and when, and a result can open a restore with the items already selected. Below, the EtherInsights Tenant Drift screen for a sample company, Example Ltd: 7 things changed since you saved your copy, 1 restore waiting for approval, and a list of changes such as Edge settings, a Teams meeting policy and an Intune assignment filter, with who changed each and when.
- **07-link-share.png** — Back up the Microsoft 365 configuration. EtherInsights Tenant Backup, for resellers and MSPs in the Nordics, through ARJ Distribution.

A Swedish variant is pending. Ryan re-renders once ARJ sends the Swedish on-image copy.
