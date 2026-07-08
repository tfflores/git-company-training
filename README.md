# 🎓 Taller de Git y GitHub

Repositorio de práctica para la capacitación. Hola amigos y amigas 👋

## ¿Qué vamos a hacer?

En este taller vas a aprender el flujo básico de trabajo con Git:
crear una rama, hacer cambios, subirlos, abrir un Pull Request y
(lo más divertido) **resolver conflictos**.

## Los archivos del juego

| Archivo | Misión | Nivel de caos |
|---|---|---|
| [muro.md](muro.md) | Agrega tu tarjeta de presentación al final | 🌶️ Bajo |
| [pizzeria.md](pizzeria.md) | Inserta tu pizza favorita en el menú | 🌶️🌶️ Medio |
| [debates.md](debates.md) | Impón tu opinión reemplazando la respuesta oficial | 🌶️🌶️🌶️ Conflicto garantizado |

## Paso a paso

1. **Abre tu Codespace** desde el botón verde `Code > Codespaces`.
2. **Crea tu rama** (usa tu nombre para que sea única):
   ```bash
   git checkout -b tu-nombre/mi-primer-cambio
   ```
3. **Edita** uno de los archivos del juego.
4. **Guarda y sube tus cambios**:
   ```bash
   git add .
   git commit -m "feat: agrego mi respuesta"
   git push -u origin tu-nombre/mi-primer-cambio
   ```
5. **Abre un Pull Request** hacia `main` desde GitHub.
6. **Haz merge**... y si aparece un conflicto, ¡no entres en pánico!
   Es parte del plan 😄

## ¿Y si hay conflicto?

Un conflicto solo significa que dos personas cambiaron las mismas líneas.
Git te muestra ambas versiones y tú decides con cuál quedarte (o combinar las dos):

```
<<<<<<< tu-rama
Tu versión
=======
La versión que ya está en main
>>>>>>> main
```

Borra las marcas (`<<<<<<<`, `=======`, `>>>>>>>`), deja el texto final
como quieres que quede, guarda, haz commit y listo. 🎉
