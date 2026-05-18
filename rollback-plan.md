# Rollback Plan

### If production deployment fails:

1. Switch traffic back to Blue environment
2. Restore database from latest backup
3. Redeploy previous stable version using Git tag `v0.9.0`
4. Notify stakeholders
5. Investigate root cause
