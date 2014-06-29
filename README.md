# HexStr
A simple module for HexStr encoding / decoding in Elixir

### Usage

Encode to binary:
```elixir
iex> HexStr.encode("This is a test.")
     "54686973206973206120746573742e"

iex> HexStr.encode('This is a test.')
     "54686973206973206120746573742e"

iex> HexStr.encode(123456)
     "1e240"
```

Decode to binary:
```elixir
iex> HexStr.decode("54686973206973206120746573742e")
     "This is a test."

iex> HexStr.decode('54686973206973206120746573742e')
     "This is a test."
```

Encode to list:
```elixir
iex> HexStr.encode_to_list('This is a test.')
     '54686973206973206120746573742e'

iex> HexStr.encode_to_list("This is a test.")
     '54686973206973206120746573742e'

iex> HexStr.encode(123456)
     '1e240'
```

Decode to list:
```elixir
iex> HexStr.decode('54686973206973206120746573742e')
     'This is a test.'

iex> HexStr.decode("54686973206973206120746573742e")
     'This is a test.'
```

Convert hex to integer:
```elixir
iex> HexStr.to_integer('54686973206973206120746573742e')
     438270661302729020147902120434299950

iex> HexStr.to_integer("54686973206973206120746573742e")
     438270661302729020147902120434299950
```
