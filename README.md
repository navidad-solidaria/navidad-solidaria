# Navidad Solidaria 🎄

## 📋 Índice
- [Descripción](#descripción)
- [Guía de Despliegue](#guía-de-despliegue)
- [Actualización de Datos](#actualización-de-datos)
- [Transparencia](#transparencia)
- [Configuración](#configuración)
- [Editar Información de Bizum](#editar-información-de-bizum)
- [Ética del Uso del Material](#ética-del-uso-del-material)
- [Contacto](#contacto)

## Descripción

Navidad Solidaria es una plataforma web diseñada para facilitar donaciones y ayuda durante la temporada navideña. Este proyecto busca conectar a personas que desean ayudar con causas solidarias.

## 🚀 Guía de Despliegue

### Prerrequisitos
- Git instalado en tu sistema
- Cuenta de GitHub
- (Opcional) Node.js si deseas probar localmente

### Pasos para Desplegar

1. **Clonar el repositorio**
   ```bash
   git clone https://github.com/navidad-solidaria/navidad-solidaria.git
   cd navidad-solidaria
   ```

2. **Configurar GitHub Pages**
   - Ve a la configuración del repositorio (Settings)
   - En la sección "Pages", selecciona la rama `main` como fuente
   - Guarda los cambios y espera a que se despliegue

3. **Verificar el despliegue**
   - El sitio estará disponible en: `https://navidad-solidaria.github.io/navidad-solidaria/`
   - El despliegue puede tardar unos minutos

### Despliegue Local (Opcional)

```bash
# Instalar un servidor HTTP simple
npm install -g http-server

# Ejecutar el servidor
http-server

# Abrir en el navegador
# http://localhost:8080
```

## 🔄 Actualización de Datos

### Actualizar Información de Donaciones

1. **Editar el archivo de configuración**
   - Navega a la carpeta de datos del proyecto
   - Modifica los archivos JSON o HTML según corresponda

2. **Realizar el commit y push**
   ```bash
   git add .
   git commit -m "Actualizar datos de donaciones"
   git push origin main
   ```

3. **Esperar redespliegue automático**
   - GitHub Pages se actualizará automáticamente en 1-5 minutos

### Frecuencia Recomendada
- Actualizar los datos al menos una vez por semana durante la campaña
- Revisar y actualizar información de contacto mensualmente
- Verificar enlaces y recursos antes de cada temporada navideña

## 🔍 Transparencia

### Compromiso de Transparencia

Este proyecto se compromete a:

- **Transparencia Total**: Todas las donaciones y su uso son documentados
- **Código Abierto**: El código fuente está disponible públicamente en GitHub
- **Reportes Periódicos**: Se publican actualizaciones sobre el uso de los fondos
- **Trazabilidad**: Cada contribución es registrada y puede ser verificada

### Acceso a la Información

- **Repositorio Público**: [github.com/navidad-solidaria/navidad-solidaria](https://github.com/navidad-solidaria/navidad-solidaria)
- **Historial de Cambios**: Visible en el historial de commits
- **Issues y Discusiones**: Abiertos para la comunidad

### Auditoría

Cualquier persona puede:
- Revisar el código fuente
- Verificar las actualizaciones de datos
- Proponer mejoras mediante pull requests
- Reportar problemas a través de issues

## ⚙️ Configuración

### Estructura del Proyecto

```
navidad-solidaria/
├── index.html          # Página principal
├── css/               # Estilos
├── js/                # Scripts
├── assets/            # Imágenes y recursos
├── data/              # Archivos de datos
├── .well-known/       # Configuración de dominio
└── README.md          # Este archivo
```

### Archivos de Configuración

#### Personalización de Colores
Editar `css/styles.css` para cambiar el esquema de colores:

```css
:root {
  --primary-color: #c41e3a;
  --secondary-color: #165b33;
  --accent-color: #ffd700;
}
```

#### Configuración de Metadatos
Editar las etiquetas meta en `index.html`:

```html
<meta name="description" content="Tu descripción aquí">
<meta name="keywords" content="navidad, solidaridad, donaciones">
```

### Variables de Entorno

Si utilizas integraciones con APIs:

```javascript
// config.js
const CONFIG = {
  apiEndpoint: 'tu-endpoint-aqui',
  contactEmail: 'contacto@ejemplo.com'
};
```

## 💳 Editar Información de Bizum

### Actualizar Número de Bizum

1. **Localizar el archivo de datos de pago**
   - Abre `index.html` o el archivo correspondiente donde se muestra la información de Bizum

2. **Modificar el número**
   ```html
   <!-- Buscar la sección de Bizum -->
   <div class="bizum-info">
     <p>Número de Bizum: <strong>TU_NUMERO_AQUI</strong></p>
   </div>
   ```

3. **Actualizar también en otros lugares**
   - Verifica que el número esté actualizado en todas las páginas
   - Busca en todos los archivos HTML: `grep -r "Bizum" *.html`

4. **Añadir información adicional**
   ```html
   <div class="donation-info">
     <h3>Cómo Donar por Bizum</h3>
     <ol>
       <li>Abre tu app bancaria</li>
       <li>Selecciona Bizum</li>
       <li>Introduce el número: <strong>TU_NUMERO</strong></li>
       <li>Añade el concepto: "Navidad Solidaria"</li>
       <li>Confirma la donación</li>
     </ol>
   </div>
   ```

5. **Guardar y desplegar**
   ```bash
   git add .
   git commit -m "Actualizar información de Bizum"
   git push origin main
   ```

### Seguridad
- ⚠️ **Nunca compartas PIN o códigos de seguridad**
- ✅ Solo publica el número de teléfono asociado a Bizum
- ✅ Verifica que el número sea correcto antes de publicar

## 🤝 Ética del Uso del Material

### Principios Éticos

Este proyecto se rige por los siguientes principios éticos:

#### 1. **Uso Responsable**
- El material de este proyecto debe usarse exclusivamente para fines solidarios
- No está permitido el uso comercial sin autorización explícita
- Cualquier modificación debe mantener el espíritu solidario del proyecto

#### 2. **Atribución**
- Si utilizas este código o material, debes dar crédito apropiado
- Incluye un enlace al repositorio original
- Indica si realizaste cambios al material original

```markdown
Basado en Navidad Solidaria
https://github.com/navidad-solidaria/navidad-solidaria
```

#### 3. **No Discriminación**
- Este proyecto es inclusivo y no discrimina por motivos de:
  - Raza, etnia o nacionalidad
  - Religión o creencias
  - Género u orientación sexual
  - Capacidades físicas o mentales
  - Situación económica o social

#### 4. **Protección de Datos**
- Respeta la privacidad de los donantes
- No publiques información personal sin consentimiento
- Cumple con el RGPD y legislación aplicable
- Implementa medidas de seguridad adecuadas

#### 5. **Transparencia y Honestidad**
- Sé honesto sobre el uso de las donaciones
- Publica información clara y verificable
- No exageres ni falsifiques necesidades
- Mantén actualizados los reportes de actividad

#### 6. **Responsabilidad**
- Usa los fondos únicamente para los fines declarados
- Mantén registros precisos de todas las transacciones
- Responde a preguntas de la comunidad
- Acepta feedback y críticas constructivas

### Licencia

Este proyecto se distribuye bajo licencia MIT, lo que significa:

✅ **Permitido:**
- Uso comercial
- Modificación
- Distribución
- Uso privado

⚠️ **Condiciones:**
- Incluir la licencia original
- Dar crédito apropiado

❌ **Prohibido:**
- Eliminar avisos de copyright
- Usar sin atribución

### Código de Conducta

Todos los contribuidores deben:
- Ser respetuosos y profesionales
- Aceptar críticas constructivas
- Enfocarse en lo mejor para la comunidad
- Mostrar empatía hacia otros miembros

## 📞 Contacto

### Formas de Contacto

#### GitHub
- **Issues**: [Reportar un problema](https://github.com/navidad-solidaria/navidad-solidaria/issues)
- **Discussions**: [Participar en discusiones](https://github.com/navidad-solidaria/navidad-solidaria/discussions)
- **Pull Requests**: Contribuye al proyecto

#### Correo Electrónico
Para consultas generales, sugerencias o colaboraciones:
- 📧 Email: contacto@navidad-solidaria.org (configurar según tu caso)

#### Redes Sociales
- 🐦 Twitter: [@navidadsolidaria](https://twitter.com/navidadsolidaria) (ejemplo)
- 📘 Facebook: [NavidadSolidaria](https://facebook.com/navidadsolidaria) (ejemplo)
- 📸 Instagram: [@navidadsolidaria](https://instagram.com/navidadsolidaria) (ejemplo)

### Preguntas Frecuentes

**¿Cómo puedo contribuir?**
- Revisa las issues abiertas
- Propón mejoras mediante pull requests
- Ayuda a documentar el proyecto
- Difunde el proyecto en tus redes

**¿Es seguro donar?**
- Todas las transacciones usan métodos oficiales y seguros
- No almacenamos información bancaria
- Puedes verificar el código fuente

**¿Cómo sé que mi donación se usa correctamente?**
- Publicamos reportes periódicos
- El historial de cambios es público
- Puedes solicitar información específica

### Horario de Respuesta

- **Issues en GitHub**: 24-48 horas
- **Email**: 2-5 días laborables
- **Urgencias**: Marca como urgente en el asunto

---

## 🌟 Agradecimientos

Gracias a todos los que hacen posible este proyecto:
- Contribuidores de código
- Donantes y colaboradores
- Organizaciones aliadas
- Comunidad de GitHub

---

## 📄 Licencia

MIT License - ver el archivo [LICENSE](LICENSE) para más detalles.

---

**¿Necesitas ayuda?** No dudes en [abrir un issue](https://github.com/navidad-solidaria/navidad-solidaria/issues/new) o contactarnos.

**¡Juntos hacemos la diferencia! 🎄❤️**
