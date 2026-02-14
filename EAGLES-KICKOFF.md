# EAGLES Kickoff — MOHAMMED-REDA

## Assigned Microservice: [5.12] Integration & Onboarding

**Repo**: [rh-optimerp-integration-and-onboarding](https://github.com/ERP-CORE-DEV/rh-optimerp-integration-and-onboarding)
**Issue**: [#1](https://github.com/ERP-CORE-DEV/rh-optimerp-integration-and-onboarding/issues/1)

---

## Phase 1 — Plan (uses 1 planner agent, isolated context)
```
/plan integration-and-onboarding microservice — Controller-Service-Repository, .NET 8, CosmosDB SDK 3.54, React 18 + Ant Design, French HR compliance (DPAE, DSN, contrat de travail, periode d'essai). Reference: rh-optimerp-sourcing-candidate-attraction repo.
```

## Phase 2 — Scaffold (after plan approval)
```
/scaffold integration-and-onboarding
```

## Phase 3 — TDD first feature
```
/tdd employee-onboarding-workflow
```

## Phase 4 — Pre-PR validation
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
- **French HR**: DPAE declarations, DSN reporting, contrat de travail, periode d'essai
- **Tests**: xUnit + FluentAssertions + Moq, minimum 80% coverage
- **Commits**: Conventional commits (feat/fix/refactor/test/docs)
- **Integration dependency**: Watches [5.3] Hiring Process Management

## Reference Repo
Use [rh-optimerp-sourcing-candidate-attraction](https://github.com/ERP-CORE-DEV/rh-optimerp-sourcing-candidate-attraction) as the architecture reference.
