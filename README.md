# Secondary higher order inducement problem

Metarole.xml defines an unbounded inducement of orderConstraint-induced-role.xml
which in turn defines another pair of inducements of
focusMapping for locality attribute
(focus mapping is used only as a marker, might be any other inducement feature).
First mapping is of implicit order 1 and works ok as seen on any org - root.xml
intermediate.xml or leaf.xml (as long as metarole declares
resetOrder=1 for the first inducement), but second mapping explicitly declares
order=2 and does not work as seen on user.xml who is member of leaf.xml.