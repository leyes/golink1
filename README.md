What does Go actually link in the executable?

```
$ go install github.com/leyes/golink1/link
$ bin/link 
I am calling IReturnFoo(): 
SomeRandomPrefix_foo

$ strings bin/link |grep SomeRandomPrefix
SomeRandomPrefix_foo
$
```

Doesn't seem like `IPrintBoo` got linked despite being in the same package.