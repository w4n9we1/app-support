# Privacy Policy

**Product:** Access Database Viewer: MDB AI (Access DB Manager)  
**Effective Date:** March 10, 2026  
**Last Updated:** March 10, 2026

This Privacy Policy explains how the app processes information when you use Access Database Viewer: MDB AI (the "App"). This policy is written for the current app behavior and codebase as of the date above.

## 1. Core Privacy Principles

- The App is designed for local-first processing on your device.
- Core database workflows (file access, parsing, mirror building, SQL execution, import/export, diagnostics, backup/restore) run locally.
- Raw MDB/ACCDB database files are not uploaded as part of AI requests.
- If you use AI features, limited request context is sent to an external AI provider as described below.

## 2. Information We Process

### 2.1 Information You Provide or Select

- Database files you choose from Files or local storage (`.mdb`, `.accdb`, and import/export files such as `.csv`, `.xlsx`).
- Natural-language questions you enter for AI query or Text-to-SQL features.
- Optional semantic dictionary entries you create (for example, field aliases and business meanings).

### 2.2 Information Processed and Stored Locally on Device

The App stores certain data locally to provide functionality and recovery:

- Security-scoped bookmarks and recent file references (for reopening files).
- Local configuration (for example, AI/text-to-SQL settings and local rate-limit state).
- Local SQLite mirror databases used for query execution.
- Local snapshots/backups created before critical operations.
- Local diagnostics and audit reports (JSON files).
- Local export files you generate.
- Local semantic dictionary data.

These items are stored on-device using iOS app storage locations (such as UserDefaults, app support storage, and temporary directories).

### 2.3 AI-Related Data Transfers (Only When AI Features Are Used)

When you run AI features, the App may send a request to an AI service endpoint (currently OpenRouter API path). The request can include:

- Your natural-language question.
- Sanitized schema context (such as table names, column names, and column types).
- Semantic dictionary context (if applicable in that flow).
- Limited value hints sampled from selected columns (small candidate text values used to improve SQL grounding).

The App does **not** intentionally upload raw MDB/ACCDB file binaries in these AI requests.

## 3. How We Use Information

We use processed information to:

- Open and parse database files you selected.
- Build a local queryable mirror and execute SQL.
- Provide error diagnostics and repair guidance.
- Run import/export and consistency checks.
- Create backup snapshots and restore state when needed.
- Generate SQL with AI when you explicitly use AI features.

## 4. Sharing and Third Parties

- We do not sell your personal information.
- We do not use third-party ad SDKs for personalized advertising in the current app implementation.
- We do not use third-party analytics/crash SDKs in the current app implementation.
- Data is sent to an external AI provider only when AI features are used, and only with the request context described in Section 2.3.
- If you manually export or share files/reports, you control where those files go.

## 5. Data Retention

- Local app data remains on your device until it is overwritten, cleared, or the app is removed.
- Some files are stored in iOS temporary directories and may be removed by the system.
- Backup snapshots and diagnostics remain until cleared by app actions or app removal.

## 6. Security

- The App uses iOS file permission mechanisms (including security-scoped access) for document access.
- The codebase includes secure storage support via iOS Keychain APIs for secrets.
- No system can guarantee absolute security; please protect your device and local files appropriately.

## 7. Your Choices

- You can use core database features locally without enabling cloud sync.
- If you do not want AI-related data transfer, do not use AI query/Text-to-SQL online flows.
- You can clear locally generated artifacts (such as diagnostics, snapshots, and export cache) through available app functions and by removing the app.

## 8. International Data Transfers

If AI features are used, request data may be processed by third-party providers and infrastructure in jurisdictions outside your country/region.

## 9. Children's Privacy

The App is not directed to children under 13, and we do not knowingly collect personal information from children under 13 through this App.

## 10. Changes to This Policy

We may update this policy to reflect product, legal, or operational changes. Updated versions will include a revised "Last Updated" date.

## 11. Contact

For privacy questions about this App, contact us through the contact channel published on the official website associated with this project.
