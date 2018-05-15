# Higher order inducement problems


## Secondary higher order inducement does not work

Diagram of relevant roles

`orderConstraint-induced-role <---indirectly assigned by higher order inducement--- leaf (org) <---assignment--- user`

orderConstraint-induced-role defines two inducements:

- First order inducement with focus mapping that shoud set "locality" attribute of organization "leaf" to "zzz". This works.
- Higher order inducement with targetRef pointing to "other-role" and also focus mapping that should set "locality" attribute of user "user" to "yyy". Both focus mapping and role inducement (as seen in roleMembershipRef) does not work.
