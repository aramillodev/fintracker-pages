# Política de Privacidad - FinTracker

Esta carpeta contiene la página web de la Política de Privacidad para FinTracker, diseñada para ser publicada en GitHub Pages y utilizada como URL oficial en Google Play Store.

## Contenido

- `index.html` - Página web con la política de privacidad completa

## Pasos para publicar en GitHub Pages

### 1. Crear un nuevo repositorio en GitHub

```bash
# Opción A: Crear un repositorio específico para la política
# Nombre sugerido: fintracker-privacy-policy

# Opción B: Usar el mismo repositorio de tu app y publicar desde una rama específica
```

### 2. Subir estos archivos al repositorio

```bash
# Navega a la carpeta privacy-policy
cd privacy-policy

# Inicializa un nuevo repositorio git (si es un repo nuevo)
git init

# Agrega los archivos
git add .

# Haz el commit
git commit -m "Add privacy policy page"

# Conecta con tu repositorio remoto
git remote add origin https://github.com/TU_USUARIO/TU_REPOSITORIO.git

# Sube los archivos
git push -u origin main
```

### 3. Activar GitHub Pages

1. Ve a tu repositorio en GitHub
2. Haz clic en **Settings** (Configuración)
3. En el menú lateral, haz clic en **Pages**
4. En **Source**, selecciona la rama (generalmente `main` o `master`)
5. Si pusiste los archivos en la raíz, selecciona `/root`
6. Si los pusiste en una carpeta específica, selecciona `/docs` (deberás renombrar la carpeta a `docs`)
7. Haz clic en **Save**

### 4. Obtener la URL

Después de unos minutos, GitHub Pages generará tu sitio. La URL será:

```
https://TU_USUARIO.github.io/TU_REPOSITORIO/
```

O si usas un dominio personalizado:

```
https://tu-dominio.com/
```

### 5. Usar la URL en Google Play Store

Una vez que el sitio esté activo:

1. Ve a la consola de Google Play
2. En la configuración de tu aplicación, busca **"Privacy Policy"**
3. Pega la URL de tu GitHub Pages
4. Guarda los cambios

## Antes de publicar

### Información que debes actualizar en `index.html`

Busca y reemplaza los siguientes marcadores de posición:

1. **Línea ~258**: `[TU_EMAIL_DE_CONTACTO]` - Tu email de contacto real
2. **Línea ~259**: `[TU_NOMBRE_O_EMPRESA]` - Tu nombre o el nombre de tu empresa
3. **Línea 15**: Verifica la fecha de última actualización

### Opcional: Personalizaciones adicionales

- **Colores**: Puedes cambiar el color principal (`#4CAF50`) en el CSS
- **Idiomas**: Considera crear una versión en inglés si tu app será internacional
- **Logo**: Puedes agregar el logo de FinTracker en el header

## Vista previa local

Para ver cómo se verá antes de publicar:

1. Simplemente abre `index.html` en tu navegador
2. O usa un servidor local:

```bash
# Con Python 3
python -m http.server 8000

# Con Node.js (si tienes http-server instalado)
npx http-server
```

Luego visita `http://localhost:8000` en tu navegador.

## Estructura alternativa para GitHub Pages

Si prefieres mantener todo en el mismo repositorio de tu app:

```
fintracker/
├── privacy-policy/
│   └── index.html
├── lib/
├── android/
└── ...
```

Entonces configura GitHub Pages para publicar desde la carpeta `/privacy-policy` o renómbrala a `/docs`.

## Notas importantes

- La URL de GitHub Pages puede tardar 5-10 minutos en activarse la primera vez
- Google Play Store requiere que la URL sea accesible públicamente
- Asegúrate de que el repositorio sea público para que GitHub Pages funcione (o usa GitHub Pro para repos privados)
- Mantén esta política actualizada si cambias la forma en que manejas los datos

## Soporte

Si tienes problemas al configurar GitHub Pages, consulta:
- [Documentación oficial de GitHub Pages](https://docs.github.com/es/pages)
- [Guía de inicio rápido](https://docs.github.com/es/pages/quickstart)
