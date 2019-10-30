# howto-elixir


_Small_ intro to elixir and the procces oriented nature

Use [vscode-elixir](https://marketplace.visualstudio.com/items?itemName=mjmcloug.vscode-elixir) it will help a lot

[Documentation for Elixir](https://hexdocs.pm/elixir/Kernel.html)

## How to Install

[ASDF is a package manager](https://github.com/asdf-vm/asdf)

ASDF has a [plugin for Erlang](https://github.com/asdf-vm/asdf-erlang)

`asdf plugin-add erlang`
`asdf install erlang 22.0.5`

(Be patient, this may take some time)

ASDF also has a [plugin for Elixir](https://github.com/asdf-vm/asdf-elixir)

`asdf plugin-add elixir`

`asdf install elixir 1.9.0`

confirm the installation was successfull with `iex` (Elixir REPL)

## Mix

Mix is the tool used to ease development with elixir, it comes shipped with the language

Mix has a configuration file per project named `mix.exs`, this is were dependencies etc are declared.

`mix deps.get`
will download all dependencies.

`mix deps.update --all`
will update all deps

`mix test`
will run all tests in /test

`mix compile`
to compile the program, will show warnings and errors.

`mix docs`
will output the documentation for our application.

`mix escript.build`
will build a binary executable

Will open a REPL in the context of your mix project.
`iex -S mix`
