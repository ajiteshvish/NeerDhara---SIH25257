# Security and privacy

- **Login:** first access verifies the phone with an OTP, then the user sets a password for later visits.
- **Demo-only OTP:** `123456` is enabled only for the hackathon demonstration and must be turned off for real use.
- **Least access:** every request checks the user's role and assigned household, village, block or district.
- **Private media:** photos and voice notes are private; authorised viewers receive short-lived links.
- **Auditability:** administrative changes and operational actions are recorded with actor and time.
- **Safer field use:** the Android app stores its session in protected device storage and keeps queued actions tied to the same user.
- **Privacy option:** an admin can erase a user's personal name and phone while retaining non-personal operational history.
- **Transport:** hosted web, app and sensor connections use encrypted transport.

The public showcase contains demo identities and demo data only. Production deployment requires unique OTP delivery,
consented phone numbers, operational monitoring and a documented retention policy.

