Lux Access
===

Library to check user roles in AnyLogic models.

High-level flow:

- User is logged in via OIDC
- AnyLogic model is started from a web page
- OIDC ID token is set as a model input parameter
- Lux Access library is used to check the user role in order to display or hide GUI elements

## Usage in AnyLogic

Download jarfile from https://github.com/Zenmo/lux-access/releases and add to dependencies.

Then use the `hasRole` function to check if the user has a specific role.

```jshelllanguage
import static energy.lux.access.LuxAccessKt.hasRole;

if (hasRole("admin", idToken)) {
    // show GUI element
}
```

## Obtain an ID token

How to easily obtain an ID token to run a model locally?

(TODO)

## Building

```
./gradlew shadowJar
```
