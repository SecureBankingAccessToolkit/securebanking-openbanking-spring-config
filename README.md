# securebanking-openbanking-spring-config
The Spring configuration for Open Banking applications within the Secure Banking Access Toolkit (SBAT)

| profile | service | Config server URI                                        |
|---------|---------|----------------------------------------------------------|
| docker  | RCS     | ${config-server}/securebanking-openbanking-uk-rcs/docker |
| docker  | RS      | ${config-server}/securebanking-openbanking-uk-rs/docker  |

## Common cors library properties map
- **Root key**: `common`
- **Library key**: `cors`

```yaml
common:
  cors:
    .....
```

| key                 | description                                    | default value |
|---------------------|------------------------------------------------|---------------|
| allowed_origins     | CORS Domains allowed (list)                    | localhost     |
| allowed_headers     | Headers can be used (string)                   |               |
| allowed_methods     | Allowed methods for preflight request (string) |               |
| allowed_credentials | Credentials mode accepted (boolean)            | true          |
| max_age             | Expiration time of preflight request (string)  | 3600          |

