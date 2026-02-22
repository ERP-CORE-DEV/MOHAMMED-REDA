# EAGLES Kickoff - MOHAMMED-REDA

## Assigned Microservice: [5.8] Talent Management and Internal Mobility

**Repo**: [rh-optimerp-talent-management-and-internal-mobility](https://github.com/ERP-CORE-DEV/rh-optimerp-talent-management-and-internal-mobility)
**Syncs with**: HOUDAIFA (5.7 Training and Skill Development)

---

## Phase 1 - Plan (uses 1 planner agent, isolated context)
```
/plan talent-management-and-internal-mobility microservice - Controller-Service-Repository, .NET 8, CosmosDB SDK 3.54, React 18 + Ant Design, French HR compliance (entretien professionnel, bilan de competences, mobilite interne, GPEC, plan de succession). Reference: rh-optimerp-sourcing-candidate-attraction repo.
```

## Phase 2 - Scaffold (after plan approval)
```
/scaffold talent-management-and-internal-mobility
```

## Phase 3 - TDD first feature
```
/tdd talent-pool-management
```

## Phase 4 - Pre-PR validation
```
/code-review
/security-scan
/gdpr-check
```

---

## Key Rules
- **Pattern**: Controller-Service-Repository (NOT CQRS/MediatR)
- **Database**: CosmosDB SDK 3.54 direct (NOT EF Core)
- **GDPR**: AnonymizeXxx() on personal data models + IsAnonymized flag
- **French HR**: Entretien professionnel, bilan de competences, mobilite interne, GPEC, plan de succession
- **Tests**: xUnit + FluentAssertions + Moq, minimum 80% coverage
- **Commits**: Conventional commits (feat/fix/refactor/test/docs)
- **Integration dependencies**: Watches [5.7] Training and Skill Development and [5.11] Reporting and Analytics

## Reference Repo
Use [rh-optimerp-sourcing-candidate-attraction](https://github.com/ERP-CORE-DEV/rh-optimerp-sourcing-candidate-attraction) as the architecture reference.
