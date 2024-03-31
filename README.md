# ActivityAnalyzer

Analiza archivos GPX, TCX y FIT. Identifica automáticamente los intervalos. No almacena ningún dato personal, todos los cálculos se realizan en el navegador utilizando WebAssembly.

Trabajo en curso. Con el tiempo se conectará a Strava y tal vez otros servicios.

# Building

Descargar el repositorio y el submodule:
```bash
git clone https://github.com/juanico10/TCXAnalyzer.git
git submodule update --init
```

Compilamos primero rust
```bash
cd activity-analyzer
wasm-pack build --target web
```

Despues creamos los build para Windows, linux o macos:
```bash
npx electron-packager . MotionPath --platform=linux --arch=x64
```

Adicionalmente puede ir a la carpeta docs, pueden crear con nginx estatico y crear el pwa de la app.