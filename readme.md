# The Coding Gnome

https://codestool.coding-gnome.com/courses/take/elixir-for-programmers

## Getting Started

Exercises
1. Use IEx to calculate 999999999 * 111111111
2. Find the name of a function in the String module that
   removes leading and trailing whitespace from its parameter.
3. Use the v helper to divide the result calculated in step 1
   by 9.
4. Try typing h (for help) on its own.

## Our First Project

### Introduction

By the end of this chapter, you’ll know how to:
- use mix to create and build projects
- navigate inside the project directories
- integrate iex and mix to let you explore your code

You’ll have seen:
- the basic syntax of modules and functions
- how atoms are written
- We’re going to explore some of Elixir’s tooling by building the first
  part of our Hangman game: the dictionary module.

### Create a New Project

I’m going to be building the Hangman project in a series of units. We’ll
start with a Dictionary application, then add the game logic later.

```bash
mix new dictionary
```

```bash
tree

# .
# ├── README.md
# ├── lib
# │   └── dictionary.ex
# ├── mix.exs
# └── test
#     ├── dictionary_test.exs
#     └── test_helper.exs
```

Key Points: create a new Elixir project using
- `$ mix new dictionary`
- your code goes under `lib/`, and 
- tests go under `test/`
- `mix.exs` defines the configuration of your project
- `mix` to compile the application
- :point_up: must be used in the top-level directory of the application
  (the one containing the `mix.exs` file)

Your Turn
- Try entering `mix help` in your terminal.
- Then try `mix help run`,
- and `iex -h`,
- and finally `elixir -h`

### Start Coding

Now we have our project structure in place, it’s time to start coding. As
our source code lives under `lib/`, and our project is called dictionary,
mix already created a file called `lib/dictionary.ex`, just waiting for us
to start hacking.

xxx

#### Things we saw: Language Stuff

You can group a chunk of Elixir code between the keywords `do` and `end`.

This is used in our example to delineate the body of our module, and the
bodies of the two functions it contains:

```elixir
defmodule Dictionary do
  # body of module . . .
end

def random_word() do
  # body of function . . .
end
```

modules in Elixir are defined using `defmodule` followed by the module
name and a `do/end` block.

functions are defined using `def` followed by the function name, any
parameters, and the body in a `do/end` block.

module names must be an Elixir atom. Conventionally we use Capitalized
words (`MyFirstModule`). There’s a section about atoms later in this
chapter.

Function names are either names or one of the Elixir operators. Names must
start with a lowercase letter or underscore, and may contain letters,
digits, and underscores. 

The name may end with an exclamation point or a question mark.

`IO.puts` writes a string to standard output.

#### Tool stuff

`mix` on its own compiles your project

`mix run` runs it

`mix run -e ⟪code⟫` executes the code in the context of your project

`iex -S mix` starts iex in the context of your project—it uses mix to
build the application environment and then enters iex

inside iex:
```elixir
iex> r ModuleName       # recompiles the file containing ModuleName

iex> c "lib/name.ex"    # compiles the given file
```

#### Your Turn

- If you haven’t already coded along with the video, do it now.
- Run the hello function you wrote using both mix and iex.
- Keep iex running, and change the message you output in the program
  source. Save it away. Reload the file in iex using the r command and
  rerun your function.
- Introduce some syntax errors into your module. Leave off a do or an end,
  misspell def and so on. Have a look at the error messages when you
  compile, and see how they relate to the changes you made.



## A Mad Dash Through Elixir Types 0 / 10

## Pattern Matching 0 / 6

## Write the Hangman Game 0 / 10

## Text Interface to the Game 0 / 4

## Refactor the Dictionary 0 / 2

## Processes and Maintaining State 0 / 6

## Using an Agent for the Dictionary 0 / 2

## Make the Dictionary a Free Standing Application 0 / 2

## No, Mr Dictionary, I Expect You To Die 0 / 2

## The Story So Far… 0 / 1

## Hangman: the OTP Server 0 / 5

## Nodes and Distributed Elixir 0 / 4

## Distributed Text Clients 0 / 4

## Getting Started with Phoenix 0 / 6

## Hangman and Phoenix 0 / 5

## Channels and a Single Page App 0 / 7

## Wrapping Up 0 / 1

