# Keycloak theme EPFL login

Provide a [Keycloak] login theme with [EPFL] colors.

## How-To

Clone this repository to the Keycloak's themes folder, or use it as a volume in
a `docker-compose.yml` as below :

```
...
services:
  keycloak:
    image: quay.io/keycloak/keycloak
...
    volumes:
      - ./keycloak/themes/keycloak.theme-login-epfl:/opt/keycloak/themes/EPFL
...
```

To use it as a default, set the `  "loginTheme": "EPFL",` property in the
imported `realm.json` file.


## Links

* Keycloak themes documentation: https://www.keycloak.org/docs/11.0/server_development/#_themes
* EPFL theme reference: https://epfl-si.github.io/elements/#/organisms/form


## List of projects that use this theme

* https://github.com/epfl-si/react.starterkit
* https://github.com/epfl-si/lhd3-dev


[keycloak]: https://www.keycloak.org/
[EPFL]: https://www.epfl.ch
