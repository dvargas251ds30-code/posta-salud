# Pruebas unitarias del módulo Pacientes (Guía 03)

Fecha: 23/11/2026 · Responsable: Daniel Vargas Quispe

| Caso | Resultado | Observación |
|------|-----------|-------------|
| CP01 | OK | Listado inicial muestra 10 registros, total 40 y paginación |
| CP02 | OK | Búsqueda por DNI exacto devuelve 1 paciente |
| CP03 | OK | Búsqueda por apellido en minúsculas filtra coincidencias |
| CP04 | OK | Al pasar a página 2 se mantiene el filtro ?buscar= |
| CP05 | OK | Muestra errores en español en campos obligatorios |
| CP06 | OK | Rechaza DNI de 7 dígitos y conserva los datos escritos |
| CP07 | OK | Rechaza DNI duplicado con mensaje personalizado |
| CP08 | OK | Rechaza fecha de nacimiento futura |
| CP09 | OK | Rechaza celular que no empieza con 9 |
| CP10 | OK | Registra paciente válido y redirige a su ficha (total 41) |
| CP11 | OK | Edita celular sin marcar el DNI propio como duplicado |
| CP12 | OK | Impide editar usando el DNI de otro paciente |
| CP13 | OK | Impide eliminar paciente con citas y muestra aviso rojo |
| CP14 | OK | Elimina paciente sin citas y muestra aviso verde (total 40) |
| CP15 | OK | Ruta inexistente /pacientes/99999 devuelve error 404 |