# What is it?

Pybit is a library written in python that allows you to convert binary to decimal, binary to hex. One of its key features is bit arrays.

## Conversions

str->bool_tuple <br/>
```py
print("String -> Bool_tuple:",pybit.str_binary_to_bool("1010"))
```
bool_tuple -> str
```py
print("Bool_tuple -> string:",pybit.bool_to_str_binary((True,False,True,True)))
```

binary -> decimal
```py
print("Binary -> Decimal:",pybit.binary_to_decimal("1010"))
```

decimal -> binary
```py
print("Decimal -> Binary",pybit.decimal_to_binary(10))
```

Binary -> Hex
```py
print("Binary -> Hex",pybit.binary_to_hex("1010"))
#Alternatives:
print("Using built in funtion",hex(pybit.binary_to_decimal((True,False,True))))
```

## Bit Array

```py
x = pybit.bitarray()


x.appendbits((True,False))

print("Tuple containing two bits:",x.raw_data())
```