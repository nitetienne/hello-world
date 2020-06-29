# hello-world
my work

-create another repository:lapply() and sapply()
#lapply() always returns a list.Here below there is an example:
x <- list(a = 1:6, b = rnorm(12), c = rnorm(20, 1), d = rnorm(100, 5))
lapply(x, mean)
#which a result is:
$a
[1] 3.5

$b
[1] 0.1398673

$c
[1] 1.066277

$d
[1] 5.09533

#The sapply() function behaves similarly to lapply(); the only real difference is in the return value.sapply() attempts to simplify the result:
#example:
x <- list(a = 1:6, b = rnorm(12), c = rnorm(20, 1), d = rnorm(100, 5))
sapply(x, mean)
        a         b         c         d 
3.5000000 0.0454311 1.1199622 5.1071292 

+vapply() and tapply()
#tapply() is used to apply a function over subsets of a vector:
#example:
y <- c(rnorm(10), runif(10), rnorm(10, 1))
f <- gl(3, 10)
tapply(y, f, mean)
        1         2         3 
0.3396135 0.3738863 0.9549690 
#vapply() as being 'safer' than sapply(), since it requires you to specify the format of the output in advance, instead of just allowing R to 'guess'what you wanted. 
In addition, vapply() may perform faster than sapply() for large datasets.



