# Magic Particles

Aplicacion web interactiva que genera efectos de particulas 3D controlados con gestos de la mano en tiempo real. Utiliza la camara del dispositivo para detectar la mano mediante MediaPipe Hand Landmarker y renderiza distintas visualizaciones con Three.js segun la cantidad de dedos levantados.

## 📺 Preview

**🌐 Visita el sitio:**  [https://portfolio-notexer.vercel.app](https://portfolio-notexer.vercel.app)

## Tecnologias

- **Three.js** - Renderizado 3D y postprocesado (bloom)
- **MediaPipe Tasks Vision** - Deteccion de manos y landmarks
- **Node.js** - Servidor local con cabeceras COOP/COEP

## Tabla de gestos

| Dedos | Gesto | Efecto |
|-------|-------|--------|
| Sin mano | -- | Polvo ambiental sutil |
| 0 | Puno cerrado | Jaula wireframe digital (verde) |
| 1 | Un dedo | Red de rayos (cyan/blanco) |
| 2 | Dos dedos | Doble helice de ADN (cyan/magenta) |
| 3 | Tres dedos | Arbol fractal (dorado/ambar) |
| 4 | Cuatro dedos | Red de constelaciones (purpura/rosa) |
| 5 | Mano abierta | Explosion cosmica multicolor |

## Requisitos

- Node.js (v16 o superior)
- Navegador con soporte para WebGL y acceso a camara
- Conexion a internet (Three.js se carga desde CDN)

## Instalacion y ejecucion

```bash
git clone https://github.com/NotExer/Magic-Particles.git
cd Magic-Particles
npm install
npm start
```

Abrir en el navegador: `http://localhost:3000`

## Notas

- El navegador pedira permiso para acceder a la camara.
- Debe ejecutarse desde `localhost` o `HTTPS` para que funcione el acceso a la camara.
