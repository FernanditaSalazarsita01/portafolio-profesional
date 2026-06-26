# Comandos Git de la práctica

## I. Configuración local e inicialización

```bash
mkdir portafolio-profesional
cd portafolio-profesional
git init
git status
git add index.html
git commit -m "feat: setup inicial del portafolio"
```

## II. Segundo commit: diseño y contacto

```bash
git status
git add .
git commit -m "style: diseno visual y seccion de contacto"
```

## III. Conexión con GitHub

```bash
git remote add origin https://github.com/TU-USUARIO/portafolio-profesional.git
git branch -M main
git push -u origin main
```

## IV. Simulación de conflicto

Cambio local:

```bash
git add .
git commit -m "fix: actualizacion de titulo local"
git push origin main
```

Si Git rechaza el envío, ejecutar:

```bash
git pull origin main
```

Después de resolver el conflicto en `index.html`:

```bash
git add .
git commit -m "merge: resolucion de conflicto en titulo principal"
git push origin main
```

## V. GitHub Pages

1. Entrar al repositorio en GitHub.
2. Ir a `Settings > Pages`.
3. En `Build and deployment`, seleccionar la rama `main`.
4. Guardar la configuración.
5. Esperar a que GitHub genere el sitio.
```
