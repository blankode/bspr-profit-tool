# README

## MAC
GOOS=windows GOARCH=amd64 CGO_ENABLED=1 CC=x86_64-w64-mingw32-gcc CXX=x86_64-w64-mingw32-g++ wails build -clean -o srpt.exe -platform windows/amd64

## Windows
wails build -clean -o srpt.exe
