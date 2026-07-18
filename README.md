# Kinesiólogo - Landing Page

Landing page para un kinesiólogo profesional (kinesiólogo oficial del Club Atlético Belgrano), pensada para captar pacientes mediante contacto directo por WhatsApp y un formulario de reserva de turnos.

## Demo en vivo

https://421310-1w3-gatica-nahuel.github.io/Kinesiologo-Page/

## Características

- Diseño responsive (mobile / tablet / desktop)
- Secciones: Hero, Sobre mí, Metodología, Servicios, CTA, Contacto y Footer
- Botones de contacto directo por WhatsApp con mensaje predefinido
- Formulario de contacto con honeypot anti-spam, integrable con Formspree
- Animaciones de aparición al hacer scroll (Intersection Observer)
- SEO local con datos estructurados (schema.org `MedicalBusiness`) y meta tags Open Graph / Twitter Card
- Menú mobile con panel deslizante

## Tecnologías usadas

- HTML5
- Tailwind CSS (vía CDN)
- JavaScript (vanilla)
- [Lucide Icons](https://lucide.dev/)
- Google Fonts (Inter, Oswald, Nothing You Could Do)
- GitHub Pages (deploy)

## Estructura del proyecto

```
Kinesiologo-Page/
├── index.html      # Página completa (markup, estilos y lógica)
├── images/
│   └── hero.png     # Imagen principal de la sección de inicio
└── README.md
```

## Configuración

Antes de usar este proyecto en producción, hay que editar dentro de `index.html`:

- `WA_PHONE_NUMBER`: número de WhatsApp real (con código de país, sin `+`)
- `action` del formulario de contacto: reemplazar el endpoint placeholder de Formspree por uno real
- `og:image` / `twitter:image` / JSON-LD `image`: reemplazar por una imagen propia
- `og:url`: reemplazar por el dominio real del sitio

## Cómo correrlo localmente

Al ser un único archivo HTML sin dependencias de build, alcanza con abrir `index.html` en el navegador, o servirlo con cualquier servidor estático:

```bash
npx serve .
```
