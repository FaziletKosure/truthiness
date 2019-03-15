# Truthiness

Truthiness is very simple to understand.  Does a value convert to _true_ or _false_ when cast to boolean?

Paste this in the console to learn about truthiness, or study it [on python tutor](https://goo.gl/7tBTj3):
```js
{
  const x = ; // experiment with different values 
  const truthiness_x = Boolean(x);

  if (truthiness_x) {
    console.log("truthy: " + typeof x + ", " + x);
  } else {
    console.log("falsey: " + typeof x + ", " + x);
  };
};
```

This repo covers 4 important operators who's behavior is dependant on the _truthiness_ of their arguments.

### Index
* [() ? : ;](#ternary-operator)
* [&&](#and-operator)
* [||](#or-operator)
* [!](#not-operator)
* [resources](#resources)


---
---

## Ternary Operator

The ternary operator evaluates the _truthiness_ of a value and returns either the first option or the second 

[pytut link](https://goo.gl/xK4GcW)

Paste this in the console to learn about the ternary operator:
```js
{ 
  const x = ; // experiment with different values 
  const tern_value = (x) ? "truthy" : "falsey" ;

  const truthiness_x = Boolean(x);

  const tern_truthiness = (truthiness_x) ? "truthy" : "falsey" ;
  const tern_option = (truthiness_x) ? "first" : "second" ;
  const tern_numbers = (truthiness_x) ? 1 : 2 ;
  const tern_boolean = (truthiness_x) ? true : false ;

  console.log("truthyness: " + tern_truthiness);
  console.log("option: " + tern_option);
  console.log("numbers: " + tern_numbers);
  console.log("booleans: " + tern_boolean);
};
```
Ternary operators can only have two options.

[TOP](#truthiness)

---

## And Operator

The and operator will return the first value if it's falsey, and the second value if the first is truthy.

[pytut link](https://goo.gl/rKyyV9)

Paste this in the console to learn about &&:
```js
{ 
  const a = ; // experiment with different values 
  const b = ; // experiment with different values 

  const and = a && b;
  const replication = (a) ? b : a ;

  console.assert(and === replication, "JavaScript must be broken");
};
```

[TOP](#truthiness)

---

## Or Operator

The or operator will return the first value if it's truthy, and the second value if the first is falsey.

[pytut link](https://goo.gl/Jd3Wtr)

Paste this in the console to learn about ||:
```js
{ 
  const a = ; // experiment with different values 
  const b = ; // experiment with different values 

  const or = a || b;
  const replication = (a) ? a : b ;

  console.assert(or === replication, "JavaScript must be broken");
};
```

[TOP](#truthiness)

---

## Not Operator

The or operator will return the first value if it's truthy, and the second value if the first is falsey.

pytut links: [the snippet below](https://goo.gl/bfcLXg), [! expanded](https://goo.gl/79P1iF)  

Paste this in the console to learn about !:
```js
{ 
  const a = ; // experiment with different values 

  const not = !a;

  const a_to_boolean = Boolean(a);
  const coercion_replication = !a_to_boolean;

  const ternary_replication = (a) ? false : true ;

  console.assert(not === coercion_replication, "JavaScript must be broken 1");
  console.assert(not === coercion_replication, "JavaScript must be broken 2");
};
```

[TOP](#truthiness)

---

## Resources

* pytut:
    * [truthy & falsey values](https://goo.gl/jBTLFD) 
    * [&& vs. ||](https://goo.gl/BBXea6)  
* [truthiness & comparisons](https://dorey.github.io/JavaScript-Equality-Table/) - click on the "if()" tab for truthiness
* from __boolean by example__: 
    * [truthiness for the console](https://github.com/janke-learning/boolean-by-example/blob/master/README.md#truthiness) 
    * [&&, || for the console](https://github.com/janke-learning/boolean-by-example#and-or-operators)
    * [! for the console](https://github.com/janke-learning/boolean-by-example#not)
    * [live in devtools](https://janke-learning.github.io/boolean-by-example/)
* mdn: 
    * [boolean](https://developer.mozilla.org/en-US/docs/Glossary/Boolean)  
    * [truthy](https://developer.mozilla.org/en-US/docs/Glossary/Truthy)  
    * [falsey](https://developer.mozilla.org/en-US/docs/Glossary/Falsy)  
* [a codepen](https://codepen.io/philipwalton/pen/nufrk) 

[TOP](#truthiness)

___
___
### <a href="http://janke-learning.org" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/50098409-22575780-021c-11e9-99e1-962787adaded.png" width="40" height="40"></img> Janke Learning</a>
