# OAuth2ForFun



## Authentication and Authorization [Link](https://www.okta.com/identity-101/authentication-vs-authorization/)
Authentication: A prooof who you are, most common like username/password
Authorization: User permission to access some resources. 

When a user takes a flight, Authentication is like Passport to prove who you are and Authorization is like ticket to indicate which class u can sit


### There are 2 middleware in [asp.net core middleware](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/middleware/?view=aspnetcore-6.0)
The sequenece matters here
```
app.UseAuthentication();
app.UseAuthorization().AddJwtBearer(Config)
```

Authentication,
It uses the [Policy schema](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/policyschemes?view=aspnetcore-6.0)

