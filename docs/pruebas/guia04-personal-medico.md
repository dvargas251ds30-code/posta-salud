# Pruebas del módulo Personal médico (Guía 04)

Fecha: 26/11/2026 · Responsable: Daniel Vargas

| Caso | Resultado | Observación |
|------|-----------|-------------|
| CP01 | OK | 5 profesionales activos con etiqueta verde y conteo de citas en /personal-medico |
| CP02 | OK | Filtro Inactivos muestra 1 y Todos muestra 6 profesionales |
| CP03 | OK | Filtro por especialidad + búsqueda devuelve solo coincidencias de esa especialidad |
| CP04 | OK | Formulario vacío muestra errores en español; cuenta de usuario opcional |
| CP05 | OK | Colegiatura de 3 dígitos rechazada con mensaje «de 4 a 6 dígitos» |
| CP06 | OK | DNI o colegiatura repetidos rechazados con mensaje de duplicado (RN01) |
| CP07 | OK | Opción manipulada a «Cardiología» con F12 rechazada («Seleccione una especialidad de la lista») |
| CP08 | OK | Registro vinculado a medico2@posta.test con aviso verde y total de activos en 6 |
| CP09 | OK | En un nuevo registro, la cuenta medico2@posta.test ya no aparece disponible |
| CP10 | OK | Edición de especialidad sin falsos duplicados en DNI, colegiatura ni cuenta |
| CP11 | OK | Edición con colegiatura de otro profesional muestra «ya está registrada» (RN01) |
| CP12 | OK | Al desactivar a la Dra. Huamán aparece aviso de citas por reprogramar y estado Inactivo |
| CP13 | OK | Al activar nuevamente el estado vuelve a Activo |
| CP14 | OK | php artisan route:list --path=personal-medico sin ruta DELETE |