# Conversor ARS · UYU · USD

Conversor de monedas entre pesos argentinos, pesos uruguayos y dólares que funciona sin internet.

**App en vivo:** https://ann0nip.github.io/conversor-monedas/

## Uso

- Ingresá un monto y elegí la moneda de origen (USD, UYU o ARS); el resultado aparece en las otras dos.
- Para pesos argentinos elegí el tipo de dólar: MEP (bolsa), Tarjeta u Oficial.
- "Actualizar cotizaciones" trae los valores del día. Sin conexión usa las últimas cotizaciones guardadas.
- Recuerda el último monto, la moneda y el tipo de dólar.
- Se puede instalar en el celular ("Agregar a pantalla de inicio") y funciona offline.

## Fuentes de cotización

- ARS: [DolarApi](https://dolarapi.com) (`/v1/dolares`)
- UYU: [ExchangeRate-API](https://open.er-api.com) (`/v6/latest/USD`)

## Estructura

- `index.html`: la app completa (HTML, CSS y JS en un solo archivo)
- `sw.js`: service worker que cachea la app para uso offline
- `manifest.json` e `icon.png`: datos para instalarla como app (PWA)

## Deploy

Se publica con GitHub Pages desde la rama `main`. Cada push a `main` actualiza el sitio.
