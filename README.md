
# Budget Approval System (Grails 5.x/6.x)

## Features
- Submit, approve, and reject budget requests
- Role-based logic (MANAGER)
- Audit logging for all changes
- RESTful JSON API

## Endpoints
- `POST /api/budget-request`
- `PUT /api/budget-request/{id}/approve`
- `PUT /api/budget-request/{id}/reject`
- `GET /api/budget-request/pending`
- `GET /api/audit-logs?entityType=BudgetRequest`

## Validation
- Max 10% of yearly allocation
- Positive requested amount
- No duplicate purpose in 7 days

## Run
```bash
./gradlew bootRun
```

