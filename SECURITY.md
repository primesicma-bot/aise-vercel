# Security notes — Aise

Cette version est un site/app statique. Elle applique des protections côté navigateur et hébergeur : CSP, anti-clickjacking, MIME sniffing protection, HSTS, Referrer-Policy, Permissions-Policy et isolation cross-origin.

Ces mesures ne rendent pas une application invulnérable. Si un backend est ajouté, il devra notamment gérer l'authentification, l'autorisation, la validation serveur, le rate limiting, les secrets, les journaux et la protection des API.
