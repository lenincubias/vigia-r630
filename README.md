# Vigía del R630

Revisa desde **fuera** del servidor, **cada 5 minutos** (cada corrida dura ~6 h y la siguiente la releva), que los servicios del R630 respondan
(ver `.github/workflows/vigia.yml`). Si alguno no responde después de 3 intentos, la corrida
falla y GitHub manda un correo al dueño del repositorio.

- Probarlo a mano: pestaña **Actions → Vigía del R630 → Run workflow**, o `gh workflow run vigia.yml`.
- Agregar un servicio: una línea `Nombre|https://…` en la lista `SERVICIOS`.
- El correo depende de *Settings → Notifications → Actions* de la cuenta de GitHub
  («Send notifications for failed workflows only» por correo).

- Es **público** a propósito (22-oct): así GitHub no cobra los minutos. No contiene claves: solo direcciones que ya son públicas.
- `mantener.yml` anota un latido al mes para que GitHub no apague las tareas programadas por inactividad.
