# Blazor VM1

* The project is to compile and run a vm1-assembler and vm1-console (vm) @ <https://github.com/sokoide/vm1> in a browser in web assembly usinb Blazor WASM.

## How to build

```bash
dotnet build

# to make a release build
dotnet build -c release
```

## How to run

```bash
# debug run
dotnet run
# and visit http://localhost:5000 to see it

# to run a release build
dotnet run -c release
```

## How to publish

* To publish in a `publish` directory

```bash
dotnet publish -o publish -c release
```
