# Departmental Access Control Design

## Business requirements from the assignment

- Three departments: Sales, HR, Testing.
- Four users and one manager per department (15 total accounts).
- Each department has its own shared data folder.
- Users can create and edit department files but should not be able to delete them.
- Managers can create, edit, and delete files within their department.
- Access is granted via security groups, not individual-user ACEs.

## Group model

The course materials use `GG_` for global groups (people/roles) and `DLG_` for domain-local groups (resource permissions). Examples visible in the student screenshots include:

| Group | Intended use |
|---|---|
| `GG_Sales_Users` | Sales employees |
| `GG_Sales_Managers` | Sales managers |
| `DLG_Sales_Write` | Sales resource write permission |
| `DLG_Sales_Modify` | Sales resource modify permission |

**Design pattern:** Accounts → Global groups → Domain-local groups → Resource permissions (AGDLP).

**Technical caution:** Windows NTFS “Write” and “Modify” are not interchangeable, and restricting deletion while permitting other write operations requires carefully checking advanced permissions, inheritance, and `DELETE` / `DELETE_CHILD` rights. Screenshots alone cannot prove this requirement was achieved. No effective-access tests are available.

The HR and Testing equivalents are **assignment design expectations**, not independently verified completed configurations.
