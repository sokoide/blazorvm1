# Blazor VM1

* The project is to compile and run a vm1-assembler and vm1-console (vm) @ <https://github.com/sokoide/vm1> in a browser in web assembly usinb Blazor WASM.

## How to build

```bash
# only once
dotnet add package MatBlazor

dotnet build

# to make a release build
dotnet build -c release
```

## How to run

```bash
# debug run
dotnet run
# and visit http://localhost:5000 to see it

# to detect file changes and restart automatically
dotnet watch run

# to run a release build
dotnet run -c release
```

## How to debug

1. Run the app ```dotnet run -c debug```
1. Open Chrome ```/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --remote-debugging-port=9222 http://localhost:5000```
1. In Chrome, focus on the app content and ```Shift-Cmd-D`` to open DevToos
1. Split the tab and show the content and DevTools side by side
1. Navigate to file://, open your target source and set a breakpoint
1. Operate in Chrome until it hits the breakpoint

## How to publish

* To publish in a `publish` directory

```bash
dotnet publish -o publish -c release
```
