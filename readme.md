## ⚠️ Run as Administrator

This tool collects market data from **Star Resonance**.  
To function correctly, the game must be running in **1080p resolution** and the interface must be **open to the Trading Center**.

## 📁 Data Storage

Collected data is saved to:
~/xhgm_prices.json

You can customize item outputs and crafting recipes by editing:
/good/templates/items.json

## 🧩 Dependencies

Before running, make sure you have installed:
- [Golang](https://go.dev/)
- [Wails](https://wails.io/zh-Hans/docs/gettingstarted/installation)

## ▶️ Running the Project

**First-time setup:**

go get github.com/go-vgo/robotgo

go mod tidy

Start development mode:

wails dev

## 🏗️ Build Commands
wails build -clean -o srpt.exe

## 🔹 Cross-Platform (Building Windows Binary from Another OS)
GOOS=windows GOARCH=amd64 CGO_ENABLED=1 \
CC=x86_64-w64-mingw32-gcc \
CXX=x86_64-w64-mingw32-g++ \
wails build -clean -o srpt.exe -platform windows/amd64
