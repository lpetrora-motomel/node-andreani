# Andreani Shipping Library

En esta librería se ofrecen interfaces y métodos que faciliten el uso de la API de Andreani. Se corrigió el bug para la descarga de etiquetas.

## Instalación

```
npm install --save node-andreani-api
```

## Uso

```js
import { Andreani } from "node-andreani";

const andreani = new Andreani({
  credentials: {
    CONTRATO_DOMICILIO: "CONTRATO_DOMICILIO",
    CONTRATO_SUCURSAL: "CONTRATO_SUCURSAL",
    CODIGO_CLIENTE: "CODIGO_CLIENTE",
    USER: "USER",
    PASS: "PASS",
  },
  options: {
    use: "sandbox",
    sandbox_url: "https://apisqa.andreani.com/",
    production_url: "https://apis.andreani.com",
  },
});

//.....


await andreani.obtenerTrazas(trackingNumber);

```
