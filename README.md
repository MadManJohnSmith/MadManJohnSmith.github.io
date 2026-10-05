# Alan

Construyo sistemas que se mantienen solos. Me interesan los servidores pequeños, la
automatización que no necesita que estés mirando, y el código que alguien más pueda auditar.

## Lo que hago

- **Servidores domésticos que no gastan nada.** El proyecto del que más presumo es
  [ezarr-stack](https://github.com/MadManJohnSmith/ezarr-stack): un servidor completo de
  medios y *arr corriendo **dentro de un teléfono Android** que ya no quería usar como
  teléfono. Chroot sobre TWRP, sin systemd, 7 GB de RAM, consumo eléctrico ridículo.
- **Software de escritorio.** [Syncify](https://github.com/MadManJohnSmith/Syncify) es una
  app Tauri (Rust + Vue) para tener tu música en máxima calidad y bajo tu control,
  importada desde Qobuz, Tidal, Spotify, Deezer y SoundCloud.
- **Auditoría automática.** [Improvement](https://github.com/MadManJohnSmith/Improvement)
  revisa un repositorio y repara lo que encuentra, con hallazgos verificados contra tus
  propias pruebas en vez de suposiciones.

## Proyectos

| | |
|---|---|
| [ezarr-stack](https://github.com/MadManJohnSmith/ezarr-stack) | Servidor de medios y *arr en Android con chroot. Instalable en un solo comando. |
| [Syncify](https://github.com/MadManJohnSmith/Syncify) | Gestor de música FLAC en Rust + Vue + Tauri. |
| [Improvement](https://github.com/MadManJohnSmith/Improvement) | Auditoría y reparación de repositorios con agentes locales. |
| [oci-a1-capacity](https://github.com/MadManJohnSmith/oci-a1-capacity) | Instancia OCI Always Free que se recupera sola. |
| [RehabWeb](https://github.com/MadManJohnSmith/RehabWeb-WebApp) · [API](https://github.com/MadManJohnSmith/RehabWeb-Api) | Proyecto de tesis: fisioterapia en web (Django + TypeScript). |

## Cómo trabajo

Un par de reglas que se notan en el código:

- **Nada de estado oculto.** Los servicios se manejan con scripts explícitos, no con un
  supervisor que nadie puede inspeccionar cuando algo falla a las 3 de la mañana.
- **Un fallo se avisa solo.** Si el servidor está caído, me entero por el móvil, no por
  un cliente quejándose.
- **El plan de recuperación se escribe antes de necesitarlo.** Cada uno de mis proyectos
  tiene un runbook con el triaje paso a paso.

## Sobre por qué un teléfono

El servidor corre en un Xiaomi Poco X3 Pro al que ya le quedaba poca vida como
teléfono. Con TWRP instalado da servicio como servidor, y consume una fracción de lo que
consumiría una máquina dedicada. La lección no es que los teléfonos sean mejores
servidores, es que **el hardware que ya tienes, y no usas, puede convertirse en
infraestructura** si lo cuidas con el mismo criterio que si lo hubieras comprado para eso.

## Abierto a

Trabajo en sistemas, open source y automatización. Si tienes un proyecto donde importe
que las cosas se reparen solas, escríbeme.