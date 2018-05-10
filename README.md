# Possible bugs

## Higher order inducement problem

Higher order inducement does not work for `targetRef` if it is set up using
`orderConstraint` configuration element instead of simple
`order`.

Basic diagram:

`regular-metarole <---assignment--- regular-role <---assignment--- user`

Inducements in "regular-metarole" defines following behavior:

- Role "regular-role" should have indirectly assigned "regular-role-companion": This works OK.
- User "user" should also have indirectly assigned "regular-role-companion": This don't work.

This bug holds even for secondary higher order inducement
(inducement of role which is itself induced, because higher order inducement surprisingly
works for OrgTypes) as seen in
"orderConstraint-induced-role" which defines following behavior:

- Secondary first order inducement: organization "leaf" should have it's
    "locality" set to "xxx". This works OK.
- Secondary higher order inducement: user "user" should have it's
    "locality" set to "yyy". This does not work.