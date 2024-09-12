# springboot-angular

Requires some environtment variables to run

Create auth0 app with 

```
auth0 apps create \
  --name "Bootiful Angular" \
  --description "Spring Boot + Angular = ❤️" \
  --type regular \
  --callbacks http://localhost:8080/login/oauth2/code/okta,http://localhost:4200/login/oauth2/code/okta \
  --logout-urls http://localhost:8080,http://localhost:4200 \
  --reveal-secrets
```

This requires auth0 account and `auth0 login` Copy the outputs into the env variables below

export OKTA_OAUTH2_ISSUER=
export OKTA_OAUTH2_CLIENT_ID=
export OKTA_OAUTH2_CLIENT_SECRET=
export CYPRESS_E2E_DOMAIN=
export CYPRESS_E2E_USERNAME=
export CYPRESS_E2E_PASSWORD=

Thank you to this great article on auth0.com https://auth0.com/blog/spring-boot-angular-crud/