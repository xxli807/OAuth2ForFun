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


Authorization
JWT Token 
![Basci token based flow](https://user-images.githubusercontent.com/5093598/140633499-5addcedc-144a-4ae4-9d96-7b1919ff9921.png)




### concept
Scopt: client include in the reuqest to ask for permission
Claim: server receies the scopt and issue different cliam to indicate the information. 


External [doc](https://www.linkedin.com/pulse/api-security-part-3-design-oauth-scopes-claims-based-neeli/) explained how it works


and asp.net core has a special policy, Check [Policy based cliam](https://docs.microsoft.com/en-us/aspnet/core/security/authorization/policies?view=aspnetcore-6.0)


