# Identity Server 4 Quickstart

This code follows the quickstarts from here: https://identityserver4.readthedocs.io/en/latest/quickstarts/0_overview.html

"IdentityServer is middleware that adds the spec compliant OpenID Connect and OAuth 2.0 endpoints to an arbitrary ASP.NET Core application."

## OAuth Roles
OAuth defines four roles:

* Resource Owner
* Client
* Resource Server
* Authorization Server

### Resource Owner: User
The resource owner is the user who authorizes an application to access their account. The application’s access to the user’s account is limited to the “scope” of the authorization granted (e.g. read or write access).

### Client: Application
The client is the application that wants to access the user’s account. Before it may do so, it must be authorized by the user, and the authorization must be validated by the API.

### Resource Server
The resource server hosts the protected user accounts.

### Authorization Server
The authorization server verifies the identity of the user then issues access tokens to the application.

From an application developer’s point of view, a service’s API fulfills both the resource and authorization server roles. We will refer to both of these roles combined, as the Service or API role.

Source: https://www.digitalocean.com/community/tutorials/an-introduction-to-oauth-2
