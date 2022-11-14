# Code reading

## Question 1

Take a look at the following code:

```
1    let x = 1;
2    function f1()
3    {
4        let x = 2;
5        console.log(x);
6    }
7    console.log(x);
```

Explain why line 4 and line 6 output different numbers.
Beacause the first variable is Global but the second one is local.and they are completley different from differnet scopes.
## Question 2

Take a look at the following code:

```
let x = 10

function f1()
{
    console.log(x)
    let y = 20
}

console.log(f1())
console.log(y)
```

What will be the output of this code. Explain your answer in 50 words or less.
the output will be 10 and undefined because they first variable is global so we can access anywhere in code but the seond variable is local ssope so we can not access out of scope.

## Question 3

Take a look at the following code:

```
const x = 9;

function f1(val) {
  val = val + 1;
  return val;
}

f1(x);
console.log(x);
it will return : 9
const y = { x: 9 };

function f2(val) {
  val.x = val.x + 1;
  return val;
}

f2(y)
console.log(y); it will return { x: 10}
```

What will be the output of this code. Explain your answer in 50 words or less.
when f2(y)is called y is reassigned by this fun.