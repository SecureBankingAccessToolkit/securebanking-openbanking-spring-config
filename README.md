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

# Swagger properties

# Swagger Documentation Specification properties
**Root key**: `swagger`

| key                         | description                      |
|-----------------------------|----------------------------------|
| title                       | title                            |
| description                 | Subtitle description             |
| license                     | kind of license                  |
| license-url                 | URL license address              |
| terms-of-service-url        | terms of service address         |
| contact-name                | Contact name                     |
| contact-url                 | Contact url address              |
| docket-apis-basePackage     | Java package filter              |
| docket-paths-selector-regex | Pattern to filter selected paths |

```yaml
swagger:
  title: Secure Banking Access Toolkit
  .....
```
