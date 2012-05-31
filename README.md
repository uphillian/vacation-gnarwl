vacation-gnarwl
===============

vacation command line interface for gnarwl

a python script to change the ldap attributes for gnarwl.  Wrote this for my users who like the vacation program.
Attempt to make the script menu like and somewhat customizable for other installations.

The script currently looks for /etc/vacation.cfg or vacation.cfg

This file has to have the following information:

[ldap]
base
server

[vacation]
active
end
info
start

[bool]
active
inactive

The [ldap] clause is to configure the ldap server.  The [vacation] clause is there in case you use different
ldap attributes to store your vacation information.  The [bool] clause is there in case you use something other than TRUE
and FALSE to store the booleans for setting gnarwl active.

Suggestions and rewrites always welcome...