---
type: feature
---

- `lore-server`: `[plugins.aws.immutable_store] s3_access_key_id` and `s3_secret_access_key` give
  the S3 client its own keys, so an S3-compatible store that issues its own credentials can be
  used alongside DynamoDB, which keeps the default AWS credential chain. Set both or neither; the
  secret is never logged.
