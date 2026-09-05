# POLÍTICA DE PRIVACIDAD
## El Cuaderno de Mario — SiReBAi

**Última actualización:** 05 de septiembre de 2026
**Versión del documento:** v2026.09

---

## 1. RESPONSABLE DEL TRATAMIENTO

**SiReBAi** (en adelante, "nosotros" o "el Desarrollador"), identificado con RIF/Cédula: V-20.235.191, domiciliado en Barquisimeto, Venezuela, es el responsable del tratamiento de los datos personales que se recopilan a través de la aplicación "El Cuaderno de Mario" (en adelante, "la Aplicación").

**Contacto:**
- WhatsApp: 0412 058 3113
- Correo: leonelsirae@outlook.com

---

## 2. FINALIDAD DEL TRATAMIENTO

Los datos personales se recopilan con las siguientes finalidades:

a) Prestar el servicio de gestión comercial y control interno ofrecido por la Aplicación.
b) Gestionar la suscripción, facturación y soporte técnico.
c) Enviar notificaciones relacionadas con el servicio (actualizaciones, incidencias, cambios en los Términos).
d) Captar leads comerciales a través del modo demo (solo con consentimiento del Usuario).
e) Mejorar la calidad del servicio mediante análisis de crash reports (datos técnicos anónimos).
f) Cumplir con obligaciones legales aplicables.

---

## 3. DATOS QUE RECOPILAMOS

### 3.1. Datos recopilados directamente por SiReBAi

| Dato | Finalidad | Almacenamiento |
|------|-----------|----------------|
| Nombre de la bodega | Identificación | Firebase Maestro (leads/) |
| Nombre del contacto | Identificación | Firebase Maestro (leads/) |
| Teléfono | Contacto comercial | Firebase Maestro (leads/) |
| Ciudad | Segmentación | Firebase Maestro (leads/) |
| Correo del negocio | Autenticación | Firebase Auth Maestro |
| Contraseña del negocio | Autenticación | Firebase Auth Maestro (hash) |
| Datos de crash (stack trace, dispositivo, versión) | Diagnóstico técnico | Sentry (servidores UE/USA) |

### 3.2. Datos ingresados por la Bodega (Usuario final)

La Bodega es la **responsable directa** de los siguientes datos que ingresa voluntariamente en la Aplicación. SiReBAi solo provee la infraestructura tecnológica:

| Dato | Responsable | Almacenamiento |
|------|-------------|----------------|
| Datos de cajeros (nombre, correo, rol) | La Bodega | Firebase del Cliente (usuarios/) |
| Datos de clientes (nombre, cédula, teléfono) | La Bodega | Firebase del Cliente (clientes/) |
| Datos fiscales (RIF, dirección, teléfono) | La Bodega | Firebase del Cliente (configuracion/) |
| Datos de ventas, inventario, caja | La Bodega | Firebase del Cliente |
| Logo e imágenes de marca | La Bodega | Cloudinary (CDN global) |
| Configuración de la bodega (colores, slogan) | La Bodega | Firebase del Cliente (configuracion/) |

### 3.3. Datos técnicos automáticos

- Dirección IP (para control de acceso a Firebase).
- Identificador del dispositivo (para diagnóstico de crash).
- Versión de la Aplicación y sistema operativo.
- Timestamps de conexión (para kill switch y verificación de suscripción).

---

## 4. BASE LEGAL PARA EL TRATAMIENTO

El tratamiento de datos se fundamenta en:

a) **Ejecución contractual:** Los datos necesarios para prestar el servicio (Art. 1.133 y siguientes del Código Civil venezolano).
b) **Consentimiento del Usuario:** Aceptación expresa durante el onboarding (Art. 60 de la Constitución de la República Bolivariana de Venezuela).
c) **Interés legítimo del responsable:** Para la mejora del servicio y prevención de fraudes.
d) **Cumplimiento legal:** Obligaciones tributarias o administrativas aplicables.

---

## 5. SUB-PROCESADORES Y TRANSFERENCIA INTERNACIONAL

Para la prestación del servicio, SiReBAi utiliza los siguientes servicios de terceros, que pueden implicar **transferencia internacional de datos**:

| Proveedor | Servicio | Ubicación de servidores | Finalidad |
|-----------|----------|------------------------|-----------|
| **Google LLC** | Firebase (Auth, Firestore) | Estados Unidos | Autenticación y base de datos |
| **Cloudinary Ltd.** | Cloudinary | CDN global (USA/UE) | Almacenamiento de imágenes (logos, backups) |
| **Sentry (Functional Software)** | Sentry | Estados Unidos / UE | Crash reporting y monitoreo |
| **GitHub Inc.** | GitHub Pages | Estados Unidos | Alojamiento de documentos legales |

Al utilizar la Aplicación, el Usuario **consiente expresamente** estas transferencias internacionales de datos, conforme a la legislación venezolana aplicable.

SiReBAi ha suscrito o se adhiere a los mecanismos legales adecuados para garantizar un nivel de protección suficiente en dichas transferencias (Cláusulas Contractuales Tipo, Privacy Shield para USA, etc., según aplique).

---

## 6. MEDIDAS DE SEGURIDAD

SiReBAi implementa las siguientes medidas técnicas y organizativas para proteger los datos:

a) **Cifrado en tránsito:** Todas las comunicaciones utilizan HTTPS/TLS.
b) **Cifrado en reposo:** Firebase aplica cifrado automático en sus servidores.
c) **Control de acceso:** Reglas de Firestore restringen el acceso solo a usuarios autenticados y autorizados.
d) **Arquitectura multi-tenant:** Cada Bodega tiene su propio proyecto Firebase, aislando los datos entre clientes.
e) **No hardcodeo de credenciales:** Las credenciales del cliente nunca se almacenan en el código fuente.
f) **Monitoreo continuo:** Sentry detecta y reporta incidentes de seguridad en tiempo real.
g) **Copias de seguridad:** Los planes pagos incluyen backup automático a Cloudinary.

---

## 7. DERECHOS DEL USUARIO (DERECHOS ARCO)

Conforme al Art. 60 de la Constitución de la República Bolivariana de Venezuela (autodeterminación informativa), el Usuario tiene derecho a ejercer los siguientes derechos sobre sus datos personales:

a) **Acceso:** Conocer qué datos personales se están tratando.
b) **Rectificación:** Corregir datos inexactos o incompletos.
c) **Cancelación (Supresión):** Solicitar la eliminación de sus datos personales.
d) **Oposición:** Oponerse al tratamiento de sus datos para finalidades específicas.

### ¿Cómo ejercer tus derechos?

El Usuario puede ejercer estos derechos enviando una solicitud a:
- **WhatsApp:** +58 412 058 3113
- **Correo:** leonelsirae@outllok.com

La solicitud debe incluir:
- Nombre completo del titular.
- Cédula de identidad o RIF.
- Descripción clara del derecho que se ejerce.
- Documentos que acrediten la identidad.

SiReBAi responderá en un plazo máximo de **15 días hábiles**.

### Exportación de datos

El Usuario puede solicitar en cualquier momento la **exportación completa de sus datos** en formato JSON. SiReBAi generará un archivo con toda la información almacenada en su proyecto Firebase y lo entregará a través del canal solicitado.

### Eliminación de cuenta

El Usuario puede solicitar la **eliminación total de su cuenta y datos**. El proceso es el siguiente:
1. Solicitud vía WhatsApp o correo.
2. Verificación de identidad.
3. Programación de eliminación del proyecto Firebase del Cliente (30 días de gracia para arrepentimiento).
4. Eliminación de los datos del Maestro (negocios/{correo}).
5. Confirmación al Usuario.

**Nota:** Los datos ingresados por la Bodega sobre terceros (clientes, cajeros) son responsabilidad exclusiva de la Bodega. SiReBAi solo eliminará la infraestructura, no los datos específicos ingresados por el Usuario.

---

## 8. CONSERVACIÓN DE DATOS

| Tipo de dato | Plazo de conservación |
|--------------|----------------------|
| Leads del modo demo | 90 días desde la captura (luego se eliminan automáticamente) |
| Datos de cuenta activa | Mientras la suscripción esté vigente |
| Datos de cuenta cancelada | 30 días tras la solicitud de eliminación |
| Crash reports (Sentry) | 90 días desde el evento |
| Backups de base de datos | 30 días rotativos (planes pagos) |
| Registros de auditoría | 1 año |

---

## 9. MENORES DE EDAD

La Aplicación está dirigida exclusivamente a **personas mayores de 18 años** o representantes legales de comercios. SiReBAi no recopila conscientemente datos de menores de edad. Si se detecta el registro de un menor, se procederá a la eliminación inmediata de sus datos.

---

## 10. MODIFICACIONES A LA POLÍTICA

SiReBAi se reserva el derecho de modificar esta Política de Privacidad en cualquier momento. Las modificaciones serán notificadas al Usuario mediante la Aplicación o correo electrónico. El uso continuado de la Aplicación implica la aceptación de los cambios.

**Versión anterior:** v2026.01 | **Versión actual:** v2026.09

---

## 11. CONTACTO Y AUTORIDAD DE CONTROL

Para consultas, reclamos o ejercicios de derechos:
- **WhatsApp:** +58 412 058 3113
- **Correo:** leonelsirae@outlook.com

En caso de no obtener respuesta satisfactoria, el Usuario puede acudir a la **Defensoría del Pueblo** o a los tribunales competentes de la República Bolivariana de Venezuela.

---

**FIN DEL DOCUMENTO**
Versión: v2026.09 | Fecha: 05/09/2026
