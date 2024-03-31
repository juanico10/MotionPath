Hacer la app PWA:

Añadir en el index.html dentro del <head>:

```html
    <!-- Añadido para PWA -->
    <meta name="theme-color" content="#2f4f4f">
    <link rel="apple-touch-icon" sizes="180x180" href="./images/logo.png">
    <link rel="manifest" href="./pwa/manifest.json" />
```

Y al final encima del </body>:
<script src="./pwa/regist_serviceWorker.js"></script>