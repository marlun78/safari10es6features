# EcmaScript features supported by Safari 10

## EcmaScript 2015 (aka “ES6”)

### Optimisation
* proper tail calls (tail call optimisation)
  * direct recursion
  * mutual recursion

### Syntax
* default function parameters
  * basic functionality
  * explicit undefined defers to the default
  * defaults can refer to previous params
  * arguments object interaction
  * temporal dead zone
  * separate scope
  * new Function() support
* rest parameters
  * basic functionality
  * function 'length' property
  * arguments object interaction
  * can't be used in setters
  * new Function() support
  * spread (...) operator
  * with arrays, in function calls
  * with arrays, in array literals
  * with sparse arrays, in function calls
  * with sparse arrays, in array literals
  * with strings, in function calls
  * with strings, in array literals
  * with astral plane strings, in function calls
  * with astral plane strings, in array literals
  * with generator instances, in calls
  * with generator instances, in arrays
  * with generic iterables, in calls
  * with generic iterables, in arrays
  * with instances of iterables, in calls
  * with instances of iterables, in arrays
  * spreading non-iterables is a runtime error
* object literal extensions
  * computed properties
  * shorthand properties
  * shorthand method
  * string-keyed shorthand methods
  * computed shorthand methods
  * computed accessors
* for..of loops
  * with arrays
  * with sparse arrays
  * with strings
  * with astral plane strings
  * with generator instances
  * with generic iterables
  * with instances of generic iterables
  * iterator closing, break
  * iterator closing, throw
* octal and binary literals
  * octal literals
  * binary literals
  * octal supported by Number()
  * binary supported by Number()
* template literals
  * basic functionality
  * toString conversion
  * tagged template literals
  * passed array is frozen
  * line break normalisation
* RegExp "y" and "u" flags
  * "y" flag
  * "y" flag, lastIndex
  * "u" flag
  * "u" flag, Unicode code point escapes
  * "u" flag, case folding
* destructuring, declarations
  * with arrays
  * with sparse arrays
  * with strings
  * with astral plane strings
  * with generator instances
  * with generic iterables
  * with instances of generic iterables
  * iterator closing
  * trailing commas in iterable patterns
  * with objects
  * object destructuring with primitives
  * trailing commas in object patterns
  * throws on null and undefined
  * computed properties
  * multiples in a single var statement
  * nested
  * in for-in loop heads
  * in for-of loop heads
  * in catch heads
  * rest
  * defaults
  * defaults, let temporal dead zone
* destructuring, assignment
  * with arrays
  * with sparse arrays
  * with strings
  * with astral plane strings
  * with generator instances
  * with generic iterables
  * with instances of generic iterables
  * iterator closing
  * iterable destructuring expression
  * chained iterable destructuring
  * trailing commas in iterable patterns
  * with objects
  * object destructuring with primitives
  * trailing commas in object patterns
  * object destructuring expression
  * parenthesised left-hand-side is a syntax error
  * chained object destructuring
  * throws on null and undefined
  * computed properties
  * nested
  * rest
  * nested rest
  * empty patterns
  * defaults
* destructuring, parameters
  * with arrays
  * with sparse arrays
  * with strings
  * with astral plane strings
  * with generator instances
  * with generic iterables
  * with instances of generic iterables
  * iterator closing
  * trailing commas in iterable patterns
  * with objects
  * object destructuring with primitives
  * trailing commas in object patterns
  * throws on null and undefined
  * computed properties
  * nested
  * 'arguments' interaction
  * new Function() support
  * in parameters, function 'length' property
  * rest
  * empty patterns
  * defaults
  * defaults, separate scope
  * defaults, new Function() support
* Unicode code point escapes
  * in strings
  * in identifiers
* new.target
  * in constructors
  * assignment is an early error

### Bindings
* const
  * basic support
  * is block-scoped
  * cannot be in statements
  * redefining a const is an error
  * for loop statement scope
  * for-in loop iteration scope
  * for-of loop iteration scope
  * temporal dead zone
  * basic support (strict mode)
  * is block-scoped (strict mode)
  * cannot be in statements (strict mode)
  * redefining a const (strict mode)
  * for loop statement scope (strict mode)
  * for-in loop iteration scope (strict mode)
  * for-of loop iteration scope (strict mode)
  * temporal dead zone (strict mode)
* let
  * basic support
  * is block-scoped
  * cannot be in statements
  * for loop statement scope
  * temporal dead zone
  * for/for-in loop iteration scope
  * basic support (strict mode)
  * is block-scoped (strict mode)
  * cannot be in statements (strict mode)
  * for loop statement scope (strict mode)
  * temporal dead zone (strict mode)
  * for/for-in loop iteration scope (strict mode)
* block-level function declaration

### Functions
* arrow functions
  * 0 parameters
  * 1 parameter, no brackets
  * multiple parameters
  * lexical "this" binding
  * "this" unchanged by call or apply
  * can't be bound, can be curried
  * lexical "arguments" binding
  * no line break between params and =>
  * correct precedence
  * no "prototype" property
  * lexical "super" binding in constructors
  * lexical "super" binding in methods
  * lexical "new.target" binding
* class
  * class statement
  * is block-scoped
  * class expression
  * anonymous class
  * constructor
  * prototype methods
  * string-keyed methods
  * computed prototype methods
  * optional semicolons
  * static methods
  * computed static methods
  * accessor properties
  * computed accessor properties
  * static accessor properties
  * computed static accessor properties
  * class name is lexically scoped
  * computed names, temporal dead zone
  * methods aren't enumerable
  * implicit strict mode
  * constructor requires new
  * extends
  * extends expressions
  * extends null
  * new.target
* super
  * statement in constructors
  * expression in constructors
  * in methods, property access
  * in methods, method calls
  * method calls use correct "this" binding
  * constructor calls use correct "new.target" binding
  * is statically bound
  * super() invokes the correct constructor
* generators
  * basic functionality
  * generator function expressions
  * correct "this" binding
  * can't use "this" with new
  * sending
  * %GeneratorPrototype%
  * %GeneratorPrototype% prototype chain
  * %GeneratorPrototype%.constructor
  * %GeneratorPrototype%.throw
  * %GeneratorPrototype%.return
  * yield operator precedence
  * yield *, arrays
  * yield *, sparse arrays
  * yield *, strings
  * yield *, astral plane strings
  * yield *, generator instances
  * yield *, generic iterables
  * yield *, instances of iterables
  * yield * on non-iterables is a runtime error
  * yield *, iterator closing
  * yield *, iterator closing via throw()
  * shorthand generator methods
  * string-keyed shorthand generator methods
  * computed shorthand generators
  * shorthand generator methods, classes
  * computed shorthand generators, classes
  * shorthand generators can't be constructors

### Built-ins
* typed arrays
  * Int8Array
  * Uint8Array
  * Uint8ClampedArray
  * Int16Array
  * Uint16Array
  * Int32Array
  * Uint32Array
  * Float32Array
  * Float64Array
  * DataView (Int8)
  * DataView (Uint8)
  * DataView (Int16)
  * DataView (Uint16)
  * DataView (Int32)
  * DataView (Uint32)
  * DataView (Float32)
  * DataView (Float64)
  * ArrayBuffer[Symbol.species]
  * constructors require new
  * constructors accept generic iterables
  * correct prototype chains
  * %TypedArray%.from
  * %TypedArray%.of
  * %TypedArray%.prototype.subarray
  * %TypedArray%.prototype.join
  * %TypedArray%.prototype.indexOf
  * %TypedArray%.prototype.lastIndexOf
  * %TypedArray%.prototype.slice
  * %TypedArray%.prototype.every
  * %TypedArray%.prototype.filter
  * %TypedArray%.prototype.forEach
  * %TypedArray%.prototype.map
  * %TypedArray%.prototype.reduce
  * %TypedArray%.prototype.reduceRight
  * %TypedArray%.prototype.reverse
  * %TypedArray%.prototype.some
  * %TypedArray%.prototype.sort
  * %TypedArray%.prototype.copyWithin
  * %TypedArray%.prototype.find
  * %TypedArray%.prototype.findIndex
  * %TypedArray%.prototype.fill
  * %TypedArray%.prototype.keys
  * %TypedArray%.prototype.values
  * %TypedArray%.prototype.entries
  * %TypedArray%.prototype[Symbol.iterator]
  * %TypedArray%[Symbol.species]
* Map
  * basic functionality
  * constructor arguments
  * constructor requires new
  * constructor accepts null
  * constructor invokes set
  * iterator closing
  * Map.prototype.set returns this
  * -0 key converts to +0
  * Map.prototype.size
  * Map.prototype.delete
  * Map.prototype.clear
  * Map.prototype.forEach
  * Map.prototype.keys
  * Map.prototype.values
  * Map.prototype.entries
  * Map.prototype[Symbol.iterator]
  * Map.prototype isn't an instance
  * Map iterator prototype chain
  * Map[Symbol.species]
* Set
  * basic functionality
  * constructor arguments
  * constructor requires new
  * constructor accepts null
  * constructor invokes add
  * iterator closing
  * Set.prototype.add returns this
  * -0 key converts to +0
  * Set.prototype.size
  * Set.prototype.delete
  * Set.prototype.clear
  * Set.prototype.forEach
  * Set.prototype.keys
  * Set.prototype.values
  * Set.prototype.entries
  * Set.prototype[Symbol.iterator]
  * Set.prototype isn't an instance
  * Set iterator prototype chain
  * Set[Symbol.species]
* WeakMap
  * basic functionality
  * constructor arguments
  * constructor requires new
  * constructor accepts null
  * constructor invokes set
  * frozen objects as keys
  * iterator closing
  * WeakMap.prototype.set returns this
  * WeakMap.prototype.delete
  * no WeakMap.prototype.clear method
  * .has, .get and .delete methods accept primitives
  * WeakMap.prototype isn't an instance
* WeakSet
  * basic functionality
  * constructor arguments
  * constructor requires new
  * constructor accepts null
  * constructor invokes add
  * iterator closing
  * WeakSet.prototype.add returns this
  * WeakSet.prototype.delete
  * no WeakSet.prototype.clear method
  * .has and .delete methods accept primitives
  * WeakSet.prototype isn't an instance
* Proxy
  * constructor requires new
  * no "prototype" property
  * "get" handler
  * "get" handler, instances of proxies
  * "get" handler invariants
  * "set" handler
  * "set" handler, instances of proxies
  * "set" handler invariants
  * "has" handler
  * "has" handler, instances of proxies
  * "has" handler invariants
  * "deleteProperty" handler
  * "deleteProperty" handler invariant
  * "getOwnPropertyDescriptor" handler
  * "getOwnPropertyDescriptor" handler invariants
  * "defineProperty" handler
  * "defineProperty" handler invariants
  * "getPrototypeOf" handler
  * "getPrototypeOf" handler invariant
  * "setPrototypeOf" handler
  * "setPrototypeOf" handler invariant
  * "isExtensible" handler
  * "isExtensible" handler invariant
  * "preventExtensions" handler
  * "preventExtensions" handler invariant
  * "ownKeys" handler
  * "ownKeys" handler invariant
  * "apply" handler
  * "apply" handler invariant
  * "construct" handler
  * "construct" handler invariants
  * Proxy.revocable
  * Array.isArray support
  * JSON.stringify support
* Reflect
  * Reflect.get
  * Reflect.set
  * Reflect.has
  * Reflect.deleteProperty
  * Reflect.getOwnPropertyDescriptor
  * Reflect.defineProperty
  * Reflect.getPrototypeOf
  * Reflect.setPrototypeOf
  * Reflect.isExtensible
  * Reflect.preventExtensions
  * Reflect.ownKeys, string keys
  * Reflect.ownKeys, symbol keys
  * Reflect.apply
  * Reflect.construct
  * Reflect.construct sets new.target meta-property
  * Reflect.construct creates instances from third argument
  * Reflect.construct, Array subclassing
  * Reflect.construct, RegExp subclassing
  * Reflect.construct, Function subclassing
  * Reflect.construct, Promise subclassing
* Promise
  * basic functionality
  * constructor requires new
  * Promise.prototype isn't an instance
  * Promise.all
  * Promise.all, generic iterables
  * Promise.race
  * Promise.race, generic iterables
  * Promise[Symbol.species]
* Symbol
  * basic functionality
  * typeof support
  * symbol keys are hidden to pre-ES6 code
  * Object.defineProperty support
  * symbols inherit from Symbol.prototype
  * cannot coerce to string or number
  * can convert with String()
  * new Symbol() throws
  * Object(symbol)
  * JSON.stringify ignores symbols
  * global symbol registry
* well-known symbols
  * Symbol.hasInstance
  * Symbol.isConcatSpreadable
  * Symbol.iterator, existence
  * Symbol.iterator, arguments object
  * Symbol.species, existence
  * Symbol.species, Array.prototype.concat
  * Symbol.species, Array.prototype.filter
  * Symbol.species, Array.prototype.map
  * Symbol.species, Array.prototype.slice
  * Symbol.species, Array.prototype.splice
  * Symbol.species, RegExp.prototype[Symbol.split]
  * Symbol.species, Promise.prototype.then
  * Symbol.replace
  * Symbol.search
  * Symbol.split
  * Symbol.match
  * Symbol.match, RegExp constructor
  * Symbol.match, String.prototype.startsWith
  * Symbol.match, String.prototype.endsWith
  * Symbol.match, String.prototype.includes
  * Symbol.toPrimitive
  * Symbol.toStringTag
  * Symbol.toStringTag affects existing built-ins
  * Symbol.toStringTag, new built-ins
  * Symbol.toStringTag, misc. built-ins
  * Symbol.unscopables

### Built-in extensions
* Object static methods
  * Object.assign
  * Object.is
  * Object.getOwnPropertySymbols
  * Object.setPrototypeOf
* function "name" property
  * function statements
  * function expressions
  * new Function
  * bound functions
  * variables (function)
  * object methods (function)
  * accessor properties
  * shorthand methods
  * shorthand methods (no lexical binding)
  * symbol-keyed methods
  * class statements
  * class expressions
  * variables (class)
  * object methods (class)
  * class prototype methods
  * class static methods
  * isn't writable, is configurable
* String static methods
  * String.raw
  * String.fromCodePoint
* String.prototype methods
  * String.prototype.codePointAt
  * String.prototype.normalize
  * String.prototype.repeat
  * String.prototype.startsWith
  * String.prototype.startsWith throws on RegExp
  * String.prototype.endsWith
  * String.prototype.endsWith throws on RegExp
  * String.prototype.includes
  * String.prototype[Symbol.iterator]
  * String iterator prototype chain
* RegExp.prototype properties
  * RegExp.prototype.flags
  * RegExp.prototype[Symbol.match]
  * RegExp.prototype[Symbol.replace]
  * RegExp.prototype[Symbol.split]
  * RegExp.prototype[Symbol.search]
  * RegExp[Symbol.species]
* Array static methods
  * Array.from, array-like objects
  * Array.from, generator instances
  * Array.from, generic iterables
  * Array.from, instances of generic iterables
  * Array.from map function, array-like objects
  * Array.from map function, generator instances
  * Array.from map function, generic iterables
  * Array.from map function, instances of iterables
  * Array.from, iterator closing
  * Array.of
  * Array[Symbol.species]
* Array.prototype methods
  * Array.prototype.copyWithin
  * Array.prototype.find
  * Array.prototype.findIndex
  * Array.prototype.fill
  * Array.prototype.keys
  * Array.prototype.values
  * Array.prototype.entries
  * Array.prototype[Symbol.iterator]
  * Array iterator prototype chain
  * Array.prototype[Symbol.unscopables]
* Number properties
  * Number.isFinite
  * Number.isInteger
  * Number.isSafeInteger
  * Number.isNaN
  * Number.EPSILON
  * Number.MIN_SAFE_INTEGER
  * Number.MAX_SAFE_INTEGER
* Math methods
  * Math.clz32
  * Math.imul
  * Math.sign
  * Math.log10
  * Math.log2
  * Math.log1p
  * Math.expm1
  * Math.cosh
  * Math.sinh
  * Math.tanh
  * Math.acosh
  * Math.asinh
  * Math.atanh
  * Math.trunc
  * Math.fround
  * Math.cbrt
  * Math.hypot
* Date.prototype[Symbol.toPrimitive]

### Subclassing
* Array is subclassable
  * length property (accessing)
  * length property (setting)
  * correct prototype chain
  * Array.isArray support
  * Array.prototype.concat
  * Array.prototype.filter
  * Array.prototype.map
  * Array.prototype.slice
  * Array.prototype.splice
  * Array.from
  * Array.of
* RegExp is subclassable
  * basic functionality
  * correct prototype chain
  * RegExp.prototype.exec
  * RegExp.prototype.test
* Function is subclassable
  * can be called
  * correct prototype chain
  * can be used with "new"
  * Function.prototype.call
  * Function.prototype.apply
  * Function.prototype.bind
* Promise is subclassable
  * basic functionality
  * correct prototype chain
  * Promise.all
  * Promise.race
* miscellaneous subclassables
  * Boolean is subclassable
  * Number is subclassable
  * String is subclassable
  * Error is subclassable
  * Map is subclassable
  * Set is subclassable

### Misc
* prototype of bound functions
  * basic functions
  * generator functions
  * arrow functions
  * classes
  * subclasses
* Proxy, internal 'get' calls
  * ToPrimitive
  * CreateListFromArrayLike
  * instanceof operator
  * HasBinding
  * CreateDynamicFunction
  * ClassDefinitionEvaluation
  * IteratorComplete, IteratorValue
  * ToPropertyDescriptor
  * Object.assign
  * Object.defineProperties
  * Function.prototype.bind
  * Error.prototype.toString
  * String.raw
  * RegExp constructor
  * RegExp.prototype.flags
  * RegExp.prototype.test
  * RegExp.prototype.toString
  * RegExp.prototype[Symbol.match]
  * RegExp.prototype[Symbol.replace]
  * RegExp.prototype[Symbol.search]
  * RegExp.prototype[Symbol.split]
  * Array.from
  * Array.prototype.concat
  * Array.prototype iteration methods
  * Array.prototype.pop
  * Array.prototype.reverse
  * Array.prototype.shift
  * Array.prototype.splice
  * Array.prototype.toString
  * JSON.stringify
  * Promise resolve functions
  * String.prototype.match
  * String.prototype.replace
  * String.prototype.search
  * String.prototype.split
  * Date.prototype.toJSON
* Proxy, internal 'set' calls
  * Object.assign
  * Array.from
  * Array.of
  * Array.prototype.copyWithin
  * Array.prototype.fill
  * Array.prototype.pop
  * Array.prototype.push
  * Array.prototype.reverse
  * Array.prototype.shift
  * Array.prototype.splice
  * Array.prototype.unshift
* Proxy, internal 'defineProperty' calls
  * [[Set]]
  * SetIntegrityLevel
* Proxy, internal 'deleteProperty' calls
  * Array.prototype.copyWithin
  * Array.prototype.pop
  * Array.prototype.reverse
  * Array.prototype.shift
  * Array.prototype.splice
  * Array.prototype.unshift
* Proxy, internal 'getOwnPropertyDescriptor' calls
  * [[Set]]
  * Object.assign
  * Object.prototype.hasOwnProperty
  * Function.prototype.bind
* Proxy, internal 'ownKeys' calls
  * SetIntegrityLevel
  * TestIntegrityLevel
  * SerializeJSONObject
* Object static methods accept primitives
  * Object.getPrototypeOf
  * Object.getOwnPropertyDescriptor
  * Object.getOwnPropertyNames
  * Object.seal
  * Object.freeze
  * Object.preventExtensions
  * Object.isSealed
  * Object.isFrozen
  * Object.isExtensible
  * Object.keys
* own property order
  * Object.keys
  * Object.getOwnPropertyNames
  * Object.assign
  * JSON.stringify
  * JSON.parse
  * Reflect.ownKeys, string key order
  * Reflect.ownKeys, symbol key order
* miscellaneous
  * no escaped reserved words as identifiers
  * duplicate property names in strict mode
  * no semicolon needed after do-while
  * no assignments allowed in for-in head
  * accessors aren't constructors
  * Invalid Date
  * RegExp constructor can alter flags
  * RegExp.prototype.toString generic and uses "flags" property
  * built-in prototypes are not instances
  * function 'length' is configurable

### Annex b
* non-strict function semantics
  * hoisted block-level function declaration
  * labeled function statements
  * function statements in if-statement clauses
* __proto__ in object literals
  * basic support
  * multiple __proto__ is an error
  * not a computed property
  * not a shorthand property
  * not a shorthand method
* Object.prototype.__proto__
  * get prototype
  * set prototype
  * absent from Object.create(null)
  * present in hasOwnProperty()
  * correct property descriptor
  * present in Object.getOwnPropertyNames()
* String.prototype HTML methods
  * existence
  * tags' names are lowercase
  * quotes in arguments are escaped
* RegExp.prototype.compile
* RegExp syntax extensions
  * hyphens in character sets
  * invalid character escapes
  * invalid control-character escapes
  * invalid Unicode escapes
  * invalid hexadecimal escapes
  * incomplete patterns and quantifiers
  * octal escape sequences
  * invalid backreferences become octal escapes
* HTML-style comments
