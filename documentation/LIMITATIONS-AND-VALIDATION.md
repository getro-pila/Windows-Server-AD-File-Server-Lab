# Limitations and Future Validation

## Historical evidence

- This project was completed as NOS 130 coursework in Spring 2025.
- The original Hyper-V virtual machines are no longer available.
- Screenshots were extracted from the retained student worksheet; some fields in that worksheet are blank.
- The diagram is a reconstruction of the assigned architecture.
- No live operational or security verification is possible from these files alone.

## Suggested validation if rebuilt

1. Confirm each VM's OS version, network adapter, addressing, and DNS settings.
2. Validate domain controller services and forward/reverse DNS resolution.
3. Verify workstation domain membership and standard-user login.
4. Export sanitized OU, user, and security group membership inventory.
5. Test Sales/HR/Testing access with user and manager test accounts, including attempts to delete and cross-access department files.
6. Validate share permissions and NTFS effective access separately.
7. Record disk/volume health and perform controlled failure/recovery tests in an isolated lab.

These are **future test recommendations**, not historical results.
