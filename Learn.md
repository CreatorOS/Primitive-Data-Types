# Primitive Data Types

Here we introduce you to some primitive data types available in Solidity.

- `bool` - Boolean type. It can have true/false values
- `uint` - Unsigned integers
- `int` - signed integers
- `address` - address holds the 20 byte value representing the size of an Ethereum address

## Boolean

In Solidity, booleans are represented by the `bool` type. It can have the values `true` or `false`.
Let's see how to use it.
Create a variable boo and assign it the value `true`.

```
    bool public boo = true;

```

## Unsigned Integers

- In Solidity, unsigned integers are represented by the `uint` type.
- uint stands for unsigned integer, meaning non negative integers
- different sizes are available
  - uint8 ranges from 0 to 2 \*\* 8 - 1
  - uint16 ranges from 0 to 2 \*\* 16 - 1
  - ...
  - uint256 ranges from 0 to 2 \*\* 256 - 1
- uint is an alias for uint256

Write these lines in the editor:

```
    uint8 public u8 = 1;
    uint public u256 = 456;
    uint public u = 123;
```

## Negative/Signed Integers

- In Solidity, signed integers are represented by the `int` type.
- Negative numbers are allowed for int types
- Like uint, different ranges are available from int8 to int256
  - int256 ranges from -2 ** 255 to 2 ** 255 - 1
  - int128 ranges from -2 ** 127 to 2 ** 127 - 1
- int is an alias for int256

Write these lines in the editor:

```
    int8 public i8 = -1;
    int public i256 = 456;
    int public i = -123;
```

## Address Type

- Solidity has a built-in type called `address` which is used to represent an Ethereum address.
  Here is an example:

Code this in the editor:

```
    address public addr = 0xCA35b7d915458EF540aDe6068dFe2F44E8fa733c;
```

## Default Values

- Unassigned variables are given a default values
- For booleans, the default value is `false`
- For unsigned integers, the default value is `0`
- For signed integers, the default value is `0`
- For address, the default value is `0x0000000000000000000000000000000000000000`

```
    bool public defaultBoo; // false
    uint public defaultUint; // 0
    int public defaultInt; // 0
    address public defaultAddr; // 0x0000000000000000000000000000000000000000
```
