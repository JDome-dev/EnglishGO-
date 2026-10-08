# EnglishGo

Aplicación web móvil para aprender inglés mediante lecciones desde A1 hasta C1.

## Funciones

- Perfiles locales protegidos con PIN.
- Niveles A1, A2, B1, B2 y C1.
- Ejercicios de selección, escritura, traducción, orden y escucha.
- XP, vidas, racha y progreso.
- Diseño adaptable para celular, tableta y computador.
- Instalación como aplicación web y funcionamiento básico sin conexión.

## Estructura

```text
englishgo-github/
├── index.html
├── manifest.webmanifest
├── sw.js
├── README.md
├── LICENSE
└── .gitignore
```

## Ejecutar localmente

El service worker requiere un servidor HTTP. Desde la carpeta del proyecto:

```bash
python -m http.server 8000
```

Después abre `http://localhost:8000`.

## Publicar con GitHub Pages

1. Crea un repositorio nuevo en GitHub.
2. Sube todos los archivos de esta carpeta a la raíz del repositorio.
3. Abre **Settings > Pages**.
4. En **Build and deployment**, selecciona **Deploy from a branch**.
5. Elige la rama `main` y la carpeta `/ (root)`.
6. Guarda y espera a que GitHub publique la dirección.

## Almacenamiento

Los perfiles y avances se guardan en `localStorage`. Por eso, el progreso permanece únicamente en el navegador y dispositivo donde se creó. Para sincronizarlo entre equipos se necesita un backend como Firebase o Supabase.

## Licencia

MIT. Consulta `LICENSE`.
