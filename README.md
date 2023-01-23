# best-coding-practices

1. JS - When number of arguments is large in a function consider wrapping the arguments in the function declaration with "{ }" so that it becomes an object. Now when invoking the function the order of arguments will not matter.

```
function fun({ var1, var2, var3, var4 }) {
    //fun defination
}

fun({ var1: 'a', var2: 'b', var3: 'c', var4: 'd' })
fun({ var3: 'c', var2: 'b', var1: 'a', var4: 'd' })

//both function calls will work and order doesn't matter in this.
```
