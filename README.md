<h1 style="color:red;" align=center>-----This program is might be depricated-----</h1>

# cs2go

cs2go is a simple external ESP for FPS game, written in Go.

## Building the source code

To build this project, you will need to download and install Go from the official website: https://go.dev/doc/install.

Once you have installed Go, follow these steps:

1. Download the source code and extract the ZIP file to a directory of your choice.
2. Open the directory in your terminal or command prompt.
3. Make sure your environment variables `GOOS` is set to `windows` and `GOARCH` is set to `amd64`. You can set these variables by running the following commands:
   ```
   set GOOS=windows
   set GOARCH=amd64
   ```
4. Build the project using the following command:
   ```
   go build -ldflags "-s -w"
   ```
   The `ldflags` are optional and remove debugger functionality and strip the binary resulting in smaller file size.
5. Run the program while in a match to use.

If the compiler complains about not having `"github.com/lxn/win"`, `"golang.org/x/sys/windows"`, `"golang.org/x/sys/windows"` run `go get github.com/lxn/win`, `go get golang.org/x/sys/windows`, and `go get golang.org/x/sys/windows` | Finalize with `go mod tidy`

## Issues
Esp lagging?
Search for cs2go.exe in task manager, expand, right click the process click "go to details"
Set your priority to High, this should fix it.

Thank you for using cs2go!
