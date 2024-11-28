# Advent of Code CLI Bundle

This skeleton application helps to create puzzle implementations for [Advent of Code](https://adventofcode.com/).

Key features:
* Tests your code against the demo input + expected answer
* Automatically downloads your full puzzle input
* Automatically submit your answer to Advent of Code

## Installation
Create a new local project with

```bash
composer create-project petervanderwal/adventofcode-skeleton
```

and authorize your project to access the [Advent of Code](https://adventofcode.com/) website by running

```bash
bin/console aoc:auth
```

## Usage
This skeleton follows [Symfony best practices](https://symfony.com/doc/6.4/best_practices.html).

Puzzles within the [`App\Puzzle`](./src/Puzzle) namespace as well as other classes in most other namespaces are 
automatically registered as service, and dependencies will automatically be injected. The namespaces `App\Dto`, 
`App\Entity` and `App\Model` are excluded from automatic service registration.

### Start with your first puzzle implementation
Open [`App\Puzzle\Year2024\Day01`](./src/Puzzle/Year2024/Day01.php) within this project, make the necessary adjustments
and implement your puzzle solution.

Then run 
```bash
bin/console aoc:run
```
which will test your implementation and (when the test was successful) submit your answer to Advent of Code.

Use `bin/console aoc:list` to list all the puzzle implementations within your project.

### More information
Run `bin/console aoc:run --help` for more info or read the full documentation of 
[`petervanderwal/adventofcode-cli`](https://github.com/petervanderwal/adventofcode-cli/blob/main/README.md)

## Credits
A big shout-out to [Eric Wastl](http://was.tl/) and his team for his dedication on creating [Advent of Code](https://adventofcode.com/)
for that many years in a row already! Note that Advent of Code was not involved in the development of this bundle and is
therefore not responsible for any shortcomings you may find here.

## License
This bundle is published under the [MIT License](LICENSE.md).
