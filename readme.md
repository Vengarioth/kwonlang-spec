# Kwonlang Specification

## Elevator Pitch
__todo__

## Contribute
Fork, change, pull request.

## Functions
Functions are first class citizens. They can be anonymous, referenced via variables

## Async scopes
State: early draft

```
(
  (a) => { async(a); } => a
  (b) => { async(b); } => b
  (c) => { async(c); } => c
) => {
  async(a + b + c);
}
```

## Lambdas with arrow notation
```
(a, b) => { a + b; }
```

## Polymorphic Functions
State: early draft

```
add(a, b) {
  (string a, string b) => {
    return a + b;
  }

  (int a, int b) for a == 0 => {
    return b;
  }

  (int a, int b) => {
    return a + b;
  }

  (object a, object b) => {
    return a.toString() + b.toString();
  }
}
```

## Objects
__todo__
