# ExpasswordExternalBcrypt

This module add support for Bcrypt to ExPassword via an external command (php) for environments where a NIF can't be compiled

## Prerequisites

* [PHP](https://www.php.net/downloads) available via the PATH variable environment

## Installation

If [available in Hex](https://hex.pm/docs/publish), the package can be installed by adding `expassword_external_bcrypt` to your list of dependencies in `mix.exs`:

```elixir
def deps do
  [
    {:expassword, "~> 0.2"},
    {:expassword_external_bcrypt, "~> 0.2", only: ~W[dev test]a},
  ]
end
```

Documentation can be generated with [ExDoc](https://github.com/elixir-lang/ex_doc) and published on [HexDocs](https://hexdocs.pm). Once published, the docs can be found at [https://hexdocs.pm/expassword_external_bcrypt](https://hexdocs.pm/expassword_external_bcrypt).

## Options

Reasonable *options* are:

```elixir
%{
  # the algorithmic cost, defines the number of iterations
  cost: 10,
}
```

(you should lower these values in config/test.exs to speed up your tests)
