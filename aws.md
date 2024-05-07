


# Example SSO Config in ~/.aws/config 
```
[profile AWSAdministratorAccess-126169105268]
sso_session = firstsession
sso_account_id = 126169105268
sso_role_name = AWSAdministratorAccess
region = us-east-2
[sso-session firstsession]
sso_start_url = https://d-9a6711ce5f.awsapps.com/start#
sso_region = us-east-2
sso_registration_scopes = sso:account:access
```