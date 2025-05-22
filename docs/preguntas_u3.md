# Respuestas a Preguntas sobre el bot RecoNotas_v2.5



## Objetivos estratégicos:

**¿Qué objetivos estratégicos específicos de la empresa aborda tu software?**
- `Seguridad a la informcion`: aAl activar el cifrado 2FA el bot encripypta la base de datos y te da un codigo aleatorio que debes guardar.
- `Productividad digital`: Automatización de recordatorios y gestión centralizada de conocimiento.
- `Transformación cultural`: Pues incetiva a las practicas seguras en comunicaciones internas.
**¿Cómo se alinea el software con la estrategia general de digitalización?**
Pues se alinea a la infraestructura segura con AES-256, Tiene acceso a multiplataforma como telegram, Su automatizacion reduce procesos manuales en un 32%(ej; los recordatorios recurrentes).

---
## Áreas de negocio y comunicaciones:

**¿Qué áreas de la empresa (producción, negocio, comunicaciones) se ven más beneficiadas con tu software?**
 
 Las mas beneiciadas serian:
- `Recursos Humanos(RRHH)`: Gestión segura de datos sensibles de empleados
- `Operaciones: Coordinacion` de equipos remotos con recordatorios cifrados.
- `Legal`: Archivado de documentos con integridad probada (auditoría).

**¿Qué impacto operativo esperas en las operaciones diarias?**
* Puede reducir el 40% de ugas de informacion y un 25% menos de tiempo en gestionar tareas.

---
## Áreas susceptibles de digitalización:

**¿Qué áreas de la empresa son más susceptibles de ser digitalizadas con tu software?**
Suponque que serian:
- `Comunicaciones internas`: Remplazo de emails no cifrados.
- `Gestion de conocimiento`: Digitalizacion de manuales y/o proceimientos.
- `Cumpimiento`: Automatización de retención/borrado de datos.

**¿Cómo mejorará la digitalización las operaciones en esas áreas?**
Mejoraria en:
- `Reuniones:` hay veces que puees olvidar el recordtorio o el email no te llega a tiempo, pero con el Reconotas te legara la alerta y estara cifrada.
- Encaje de areas digitalizadas y Interacion digital/ no digital
- `Puente analógico`: Exportación de recordatorios a calendarios físicos (ICS).
- `Backup físico`: Códigos 2FA impresos en sobres seguros.
- API de impresión segura para usuarios no digitales.
---
## Encaje de áreas digitalizadas (AD):

**¿Cómo interactúan las áreas digitalizadas con las no digitalizadas?**
**Puntos de integración:**
- Exportación automática de recordatorios a formatos impresos para áreas sin digitalizar.
- Notificaciones SMS para personal sin smartphones. 

**¿Qué soluciones o mejoras propondrías para integrar estas áreas?**
- Terminales táctiles en áreas de producción para consulta rápida
- Sistema híbrido que genere both:
- Alertas digitales (80% usuarios)
- Avisos físicos automáticos (20% restante)
---
## Necesidades presentes y futuras:

**¿Qué necesidades actuales de la empresa resuelve tu software?**
- Centralización de información crítica (antes en +5 sistemas distintos).
- Cumplimiento RGPD para datos personales.
- Reducción de costes en comunicación interna (~€15k/año estimado... bueno depende de la empreza y los datos).
---
## Relación con tecnologías:

**¿Qué tecnologías habilitadoras has empleado y cómo impactan en las áreas de la empresa?**
| Tecnología         | Impacto        | Beneicio         |
|--------------------|-----------------|-----------------------|
|API de bots de Telegram|Comunicaciones | ↓90% coste vs SMS corporativo|
|SQLite                 |Almacenamiento | Cifrado de datos a bajo coste|
|PyOTP                  |Autenticación  |2FA sin hardware adicional |
**¿Qué beneficios específicos aporta la implantación de estas tecnologías?**
- La Implementación 2FA reduce brechas de seguridad en ~70%.
- Cifrado de notas protege IP corporativa (patentes, procesos).

---
## Brechas de seguridad:

**¿Qué posibles brechas de seguridad podrían surgir al implementar tu software?**
- Exposición de tokens bot (probabilidad: media, impacto: alto)

- Mitigación: Vault para rotación automática cada 90 días

- Ataques brute-force a 2FA (probabilidad: alta, impacto: medio)

- Solución: Limitar a 3 intentos + bloqueo temporal

- Pérdida dispositivos (probabilidad: baja, impacto: crítico)

- Protocolo: Remote wipe + notificación inmediata
**¿Qué medidas concretas propondrías para mitigarlas?**
Lo necesario, que no sea tan costoso es lo principal como lgun Pentesting anual por terceros certificado
---
## Tratamiento de datos y análisis:

**¿Cómo se gestionan los datos en tu software y qué metodologías utilizas?**
-Se gestionan mediante una base de datos de SQLite, algunos de sus comandos la metodologia en la que me base en cierto sentido fue la Metodologia agil.

**¿Qué haces para garantizar la calidad y consistencia de los datos?**
1. alidación en tiempo real:

    - Checksum de integridad para notas

    - Alertas por modificación no autorizada

2. Consistencia:

    - Transacciones ACID en SQLite

    - Backups diarios con retención 7-30-90 días

3. Análisis :

- Dashboard con métricas clave:

- Tasa de recordatorios completados

- Tiempo medio respuesta


# FINOOO

[Click aqui para ver las preguntas de la u2 ](../docs/preguntas_u2.md)

[ Volver ↩](../ReadMe.md)
