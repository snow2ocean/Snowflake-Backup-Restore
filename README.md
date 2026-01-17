# Snowflake-Backup-Restore
With Snowflake Backups, keep critical data in Snowflake for up to 10 years in an immutable format designed to support demanding regulatory and security requirements — and still benefit from the ease of use of the Snowflake AI Data Cloud.

1. Clone and Setup git clone https://github.com/snow2ocean/Snowflake-Backup-Restore.git
2. cd Snowflake-Backup-Restore

Follow the Quickstart Guide 👉 Complete Step-by-Step Instructions
The quickstart guide walks you through:

- Create role and assign to user
- Create database, schema, warehouse
- Privilege grants
- Create backup policies
  - Hourly backups, expire after 90 days
  - Daily backups with retention lock (Business Critical Edition)
  - Daily backups without retention lock
  - Twice-weekly backups using cron (Tue & Fri 23:00 UTC)
- Create backup sets and apply policies
  - Table-level backup set
  - Schema-level backup set
  - Database-level backup set
- Manage backup sets (apply/suspend/resume)
  - Apply/replace policy (use FORCE to replace existing policy)
  - Suspend & resume backups on a set
  - drop a backup set
- Inspect backup sets
- Restore from backups
  - Find backup IDs
  - Restore
      - Restore table
      - Restore schema
      - Restore database

SQL Scripts All SQL scripts are referenced in the quickstart guide:

1.snowflake_backup_setup.sql - Create role, database, warehouse, backup policy 
2.snowflake_restore.sql - inspect backup set and restore
