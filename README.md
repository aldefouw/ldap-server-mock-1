# ldap-server-mock
Mock ldap server for tests

## Run
docker run -d -p 3004:3004 ldap-server-mock

## Overriding default config and users
docker run -d -v <path-to-conf>:/srv/ldap-server-mock.conf.json -v <path-to-userdb>:/srv/ldap-server-mock-users.json -p 3004:3004 ldap-server-mock
