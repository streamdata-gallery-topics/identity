---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 0
info:
  title: AWS Cognito API Delete Identity Pool
  version: 1.0.0
  description: Deletes a user pool.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateIdentityPool:
    get:
      summary: Create Identity Pool
      description: Creates a new identity pool.
      operationId: createIdentityPool
      x-api-path-slug: actioncreateidentitypool-get
      parameters:
      - in: query
        name: AllowUnauthenticatedIdentities
        description: TRUE if the identity pool supports unauthenticated logins
        type: string
      - in: query
        name: CognitoIdentityProviders
        description: An array of Amazon Cognito Identity user pools and their client
          IDs
        type: string
      - in: query
        name: DeveloperProviderName
        description: The domain by which Cognito will refer to your users
        type: string
      - in: query
        name: IdentityPoolName
        description: A string that you provide
        type: string
      - in: query
        name: OpenIdConnectProviderARNs
        description: A list of OpendID Connect provider ARNs
        type: string
      - in: query
        name: SamlProviderARNs
        description: An array of Amazon Resource Names (ARNs) of the SAML provider
          for your identity         pool
        type: string
      - in: query
        name: SupportedLoginProviders
        description: Optional key:value pairs mapping provider names to provider app
          IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pool
  /?Action=DeleteIdentityPool:
    get:
      summary: Delete Identity Pool
      description: Deletes a user pool.
      operationId: deleteIdentityPool
      x-api-path-slug: actiondeleteidentitypool-get
      parameters:
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pool
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---