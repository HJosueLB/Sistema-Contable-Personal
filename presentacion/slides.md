---
theme: seriph
title: Homelab Personal
info: |
  Presentación de un pequeño homelab para multimedia, monitoreo y seguridad.
transition: slide-left
duration: 20min
---

# Homelab Personal
## Un centro de servicios en casa

<div class="grid grid-cols-2 gap-4 mt-8 text-left">
  <div class="rounded border border-gray-400/30 p-4">
    <div class="font-semibold">📺 Multimedia</div>
    <div class="text-sm opacity-80">Plex para streaming local y remoto</div>
  </div>
  <div class="rounded border border-gray-400/30 p-4">
    <div class="font-semibold">📈 Monitoreo</div>
    <div class="text-sm opacity-80">PRTG para supervisar red y servicios</div>
  </div>
  <div class="rounded border border-gray-400/30 p-4">
    <div class="font-semibold">🛡️ Seguridad</div>
    <div class="text-sm opacity-80">Firewall y control de acceso</div>
  </div>
  <div class="rounded border border-gray-400/30 p-4">
    <div class="font-semibold">⚙️ Automatización</div>
    <div class="text-sm opacity-80">Docker, VMs y servicios autoejecutables</div>
  </div>
</div>

<div class="mt-8 flex items-center justify-center gap-3">
  <button @click="$slidev.nav.prev()" class="rounded bg-white/10 px-4 py-2 text-sm hover:bg-white/20">← Anterior</button>
  <button @click="$slidev.nav.next()" class="rounded bg-white/10 px-4 py-2 text-sm hover:bg-white/20">Siguiente →</button>
</div>

<div class="mt-3 text-sm opacity-70">También puedes usar las flechas del teclado o la barra espaciadora.</div>

---

# ¿Qué es un homelab?

Un homelab es un entorno de laboratorio en casa donde se ejecutan servicios propios para:

- aprender y experimentar
- mejorar privacidad y control
- reducir dependencia de la nube
- centralizar funciones digitales del hogar

> Ideal para probar nuevas tecnologías sin riesgo alto.

---

# Servicios propuestos

## Núcleo del proyecto

- 📺 Plex Media Server
- 📈 PRTG Monitoring
- 🛡️ Firewall con OPNsense o pfSense
- 🗂️ Almacenamiento y respaldos
- 🧰 Docker + Portainer para gestión sencilla

## Opcionales

- VPN para acceso remoto
- Nextcloud o Vaultwarden
- Home Assistant para automatización del hogar

---

# Arquitectura propuesta

<div class="grid grid-cols-2 gap-6 mt-4">
  <div>
    <h3 class="font-semibold">Componentes</h3>
    <ul>
      <li>Router y firewall</li>
      <li>Mini PC o NAS como servidor</li>
      <li>Switch gestionado</li>
      <li>Puntos de acceso Wi-Fi</li>
    </ul>
  </div>
  <div>
    <h3 class="font-semibold">Flujo de funcionamiento</h3>
    <ul>
      <li>Internet → Firewall</li>
      <li>Firewall → Red local</li>
      <li>Servidor → Plex, PRTG y otros servicios</li>
      <li>Monitorización continua de la infraestructura</li>
    </ul>
  </div>
</div>

---

# Stack tecnológico

## Herramientas recomendadas

- Proxmox o VMware ESXi para virtualización
- Docker + Portainer para contenedores
- Plex Media Server para multimedia
- PRTG para monitoreo de red y dispositivos
- OPNsense/pfSense para seguridad y filtrado

## Ventaja

Permite escalar el proyecto de forma sencilla, agregando nuevos servicios con poco esfuerzo.

---

# Seguridad y monitoreo

## Medidas clave

- Segmentación de red por zonas
- Reglas de firewall estrictas
- VPN para acceso remoto seguro
- Alertas de disponibilidad y rendimiento
- Registro y auditoría de actividad

> La seguridad no solo protege el equipo, también protege la red completa del hogar.

---

# Beneficios del homelab

- Mayor control sobre los servicios
- Mejor privacidad que soluciones cloud básicas
- Aprendizaje práctico en redes, servidores y seguridad
- Escalabilidad progresiva según se necesiten más funciones
- Experiencia real de administración de infraestructura

---

# Roadmap inicial

1. Instalar el firewall y segmentar la red
2. Preparar el servidor y el almacenamiento
3. Desplegar Plex y PRTG
4. Añadir respaldos y alertas
5. Expandir con más servicios según el uso

---

# Gracias

## ¿Preguntas?

Si quieres, puedo ayudarte a convertir esta presentación en una versión más profesional con:

- estilo empresarial
- imagenes y diagramas
- una introducción más técnica
- una versión para exponer en clase
