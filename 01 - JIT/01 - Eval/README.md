## Eval

#### Bad
```
function f() {
    eval("");
    var sum = 0;
    for (var i = 0; i < N; ++i) {
        sum += i;
    }
}
```

#### Good
```
function f() {
    var sum = 0;
    for (var i = 0; i < N; ++i) {
        sum += i;
    }
}
```

http://jsperf.com/js-best-practices-jit-1
