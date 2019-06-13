# docker-aglio

A Docker Container for [Aglio](https://github.com/danielgtaylor/aglio).

## Usage examples

Read the official [Aglio Documentation](https://github.com/danielgtaylor/aglio) first.

```bash
docker run --rm -v "$PWD:/aglio" jaceju/aglio -i <source_file> -o <output_file> --theme-variables slate
```

For short, you can use alias for the long command line text. Place the alias statement in your `.bashrc` or `.zshrc`.

```bash
alias aglio='docker run --rm -v "$PWD":/aglio jaceju/aglio'
```

## Build Docker Image

```
docker build --no-cache -t jaceju/aglio .
```

## License

[The MIT License (MIT)](https://opensource.org/licenses/MIT)
