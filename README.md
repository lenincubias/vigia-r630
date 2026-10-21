# Vigía del R630

Revisa desde **fuera** del servidor, cada 30 minutos, que los servicios del R630 respondan
(ver `.github/workflows/vigia.yml`). Si alguno no responde después de 3 intentos, la corrida
falla y GitHub manda un correo al dueño del repositorio.

- Probarlo a mano: pestaña **Actions → Vigía del R630 → Run workflow**, o `gh workflow run vigia.yml`.
- Agregar un servicio: una línea `Nombre|https://…` en la lista `SERVICIOS`.
- El correo depende de *Settings → Notifications → Actions* de la cuenta de GitHub
  («Send notifications for failed workflows only» por correo).
