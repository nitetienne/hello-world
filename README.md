# hello-world
my work

create another repository:lapply() and sapply()
lapply() always returns a list.
Here below there is an example:
x <- list(a = 1:6, b = rnorm(12), c = rnorm(20, 1), d = rnorm(100, 5))
lapply(x, mean)
which a result is:
$a
[1] 3.5

$b
[1] 0.1398673

$c
[1] 1.066277

$d
[1] 5.09533

The sapply() function behaves similarly to lapply(); 
the only real difference is in the return value.
sapply() attempts to simplify the result:
example:
x <- list(a = 1:6, b = rnorm(12), c = rnorm(20, 1), d = rnorm(100, 5))
sapply(x, mean)
        a         b         c         d 
3.5000000 0.0454311 1.1199622 5.1071292 
