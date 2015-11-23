## Change type of variable

#### Bad
```
var a = 1;
var b;
var n = 100;
function sumNumberToUndefined() {
    var sum = 0;
    for (var i = 0; i < n; ++i) {
        sum += (a + b);
    }
}
```

#### Good
```
var a = 1;
var c = 2;
var n = 100;
function sumNumberToNumber() {
    var sum = 0;
    for (var i = 0; i < n; ++i) {
        sum += (a + c);
    }
}
```

http://jsperf.com/js-best-practices-jit-2/4
