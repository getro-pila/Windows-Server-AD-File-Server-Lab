# Requirement-to-Evidence Matrix

**Interpretation:** “Screenshot present” means a relevant screen was captured, **not** that all functional requirements passed testing.

| Assignment category | Evidence in worksheet | Confidence / gaps |
|---|---|---|
| Hyper-V configuration | VM inventory and virtual switch | Screenshot present; topology connectivity not retested |
| Operating systems | Two Server Manager views and Windows client properties | Screenshots present; exact installation details not independently verified |
| AD DS and DNS | ADUC domain/OU view and DNS forward lookup zone | Screenshots present; no current DNS query or authentication test |
| Sales users and groups | Sales OU, user and group membership views | Multiple screenshots present; effective permissions not tested |
| HR users and groups | HR detail screenshot fields blank | **Not demonstrated** in surviving worksheet |
| Testing users and groups | Testing detail screenshot fields blank | **Not demonstrated** in surviving worksheet |
| Sales folder NTFS/share permissions | Advanced Security and Share dialog screenshots | Screenshots present; no effective-access test |
| HR and Testing folder permissions | Detail fields blank | **Not demonstrated** |
| Mirrored OS drive | Domain controller Disk Management screenshot | Screenshot present; recovery behavior not verified |
| File server RAID-5/storage pool | File server Disk Management screenshot | Screenshot present; resilience and health not verified |

The instructor-provided example screenshot has been excluded from the public portfolio.
