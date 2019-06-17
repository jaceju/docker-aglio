# docker-aglio

A Docker Container for [Aglio](https://github.com/danielgtaylor/aglio).

## Usage examples

Read the official [Aglio Documentation](https://github.com/danielgtaylor/aglio) first.

```bash
# build
docker run --rm -v "$PWD:/aglio" jaceju/aglio -i <source_file> -o <output_file> --theme-variables slate
# serve
docker run --rm -v "$PWD:/aglio" -p 3000:3000 jaceju/aglio -i <source_file> -s
```

For short, you can use alias for the long command line text. Place the alias statement in your `.bashrc` or `.zshrc`.

```bash
alias aglio='docker run --rm -v "$PWD":/aglio -p 3000:3000 jaceju/aglio'
```

## Build Docker Image

```
docker build --no-cache -t jaceju/aglio .
```

## License

[The MIT License (MIT)](https://opensource.org/licenses/MIT)
