Julp
====

MILP modelling with Julia


    Julia
    +  LP
    -----
    =Julp.

Example code (so far)

    m = Model("max")

    x = Variable(m,"x")
    y = Variable(m,"y")

    m.objective = 5*x + 3*y
    AddConstraint(m, 1.0*x + 5*y <= 3.0)
    AddConstraint(m, 1.0*x >= 0.0)
    AddConstraint(m, 1.0*y >= 0.0)
    PrintModel(m)

