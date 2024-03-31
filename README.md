# ActivityAnalyzer

Analiza archivos GPX, TCX y FIT. Identifica automáticamente los intervalos. No almacena ningún dato personal, todos los cálculos se realizan en el navegador utilizando WebAssembly.

Trabajo en curso. Con el tiempo se conectará a Strava y tal vez otros servicios.

# Building

```
git clone https://github.com/juanico10/TCXAnalyzer.git
git submodule update --init
cd activity-analyzer
wasm-pack build --target web
```
