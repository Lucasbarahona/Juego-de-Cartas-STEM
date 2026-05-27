# 🧬 Memoria STEM

---

## Demo

Abre `stem_memory_game.html` directamente en tu navegador — no necesita servidor ni dependencias locales.

---

## Cómo se juega

1. Haz clic en cualquier carta para voltearla.
2. Encuentra su pareja antes de que se vuelva a ocultar.
3. Pasa el cursor sobre una carta boca abajo para ver su **pista**.
4. Completa los 8 pares en el menor número de movimientos posible.

---

## Conceptos incluidos

| Concepto | Descripción |
|---|---|
| 🧬 ADN | Ácido desoxirribonucleico — molécula de doble hélice |
| ⚛️ Átomo | Unidad básica de la materia |
| 𝜋 Pi | Número irracional fundamental de la geometría |
| ⚡ Electricidad | Flujo de carga eléctrica |
| 🔬 Célula | Bloque básico de los seres vivos |
| 🪐 Gravedad | F = G·m₁m₂/r² |
| 🌿 CO₂ | Dióxido de carbono |
| 〰️ Onda | Energía en movimiento |

---

## Características técnicas

- **Vanilla HTML/CSS/JS** — sin frameworks ni dependencias locales
- Iconos: [Tabler Icons](https://tabler-icons.io/) (cargados desde CDN)
- Animación de volteo 3D con CSS `transform-style: preserve-3d`
- Tablero aleatorio en cada partida
- Tooltip de pista al pasar el cursor sobre cada carta
- Contador de movimientos y pares encontrados
- Pantalla de victoria con resumen

---

## Estructura del proyecto

```
stem_memory_game.html   ← archivo único, todo incluido
README.md               ← este archivo
```

---

## Personalización

Para añadir o cambiar conceptos, edita el array `PAIRS` en el `<script>`:

```js
{ 
  id: 'wave',           // identificador único del par
  icon: 'ti-wave-sine', // icono de Tabler Icons
  label: 'Onda',        // nombre visible en la carta
  hint: 'Luz y sonido viajan así', // pista al hacer hover
  sub: 'Energía en movimiento',    // subtítulo en la carta volteada
  color: '#D4537E',     // color del icono y texto secundario
  bg: '#FBEAF0',        // fondo de la carta volteada
  text: '#4B1528',      // color del texto principal
  border: '#993556'     // color del borde al hacer match
}
```

---

## Despliegue

Para publicar en GitHub Pages:

```bash
git init
git add stem_memory_game.html README.md
git commit -m "feat: juego de memoria STEM"
git branch -M main
git remote add origin https://github.com/tu-usuario/stem-memory
git push -u origin main
```

Luego activa **GitHub Pages** desde `Settings → Pages → Branch: main`.

---

## Licencia

MIT — libre para usar, modificar y distribuir.
