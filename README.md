# ff-js

A JavaScript implementation of the Flippy Flop data structure.

## Background

A Flippy Flop is an unpredictable data structure.
Flip (insertion) and flop (removal) operations succeed at a random.

## Usage

As you'll see in the example below, the Flippy Flop is sufficiently unpredictable.

### Node.js

```javascript
var FlippyFlop = require("flippy-flop");

var ff = new FlippyFlop();

// Attempt to insert a value
ff.flip(5);

// Could be 5, or undefined if the flip call failed.
var flop1 = ff.flop();

// Could be 5 if the flop() didn't remove the value, or undefined if the flip call failed.
var flop2 = ff.flop();

// However, it's easy verify the number of elements in a FlippyFlop
var count = ff.count();
```

# Contact

You can most easily reach me on twitter [@_Shakeel](http://twitter.com/_Shakeel).

# License

This project is licensed under the terms of [the MIT license](LICENSE).