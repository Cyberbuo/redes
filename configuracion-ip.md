# 🌐 Configuración IP: ¿Estática o DHCP?
> **Misión:** Entender cómo se asignan las matrículas (IPs) en nuestra red.

---

## 🚦 Las dos formas de obtener una IP

Imagina que la IP es el **DNI** de tu ordenador. Hay dos formas de conseguirlo:

### 1. IP Estática (Manual) ✍️
Tú escribes los números a mano en la configuración del equipo.
* **Uso típico:** Servidores, Impresoras, Routers. (Equipos que **nunca** deben cambiar de dirección).
* **Ventaja:** Siempre sabes dónde están.
* **Inconveniente:** Si te equivocas en un número, ¡conflicto de IP y nada funciona!

### 2. DHCP (Automático) 🤖
Un servidor (normalmente el Router) le da una IP al equipo en cuanto se conecta.
* **Uso típico:** Móviles, Laptops de oficina, PCs de casa.
* **Ventaja:** Conectas y listo. El servidor se encarga de que no haya repetidas.
* **Inconveniente:** Si el servidor DHCP se cae, nadie tiene red.

---

## 💻 En Cisco Packet Tracer (Práctica)

Para configurar un PC en el simulador, sigue estos pasos:

1. Haz clic en el **PC**.
2. Ve a la pestaña **Desktop** > **IP Configuration**.
3. Selecciona el "botón" correspondiente:

### Configurando Estática:
Debes rellenar los **3 mosqueteros** de la red:
* **IP Address:** `192.168.1.10` (La identidad del PC).
* **Subnet Mask:** `255.255.255.0` (Dice que somos de la misma familia).
* **Default Gateway:** `192.168.1.1` (La puerta para salir a Internet).

### Configurando DHCP:
* Simplemente marca el círculo **DHCP**. 
* Verás que pone *"Requesting IP..."* y, si tienes un router configurado, los números aparecerán solos. ¡Magia! ✨

---

## 🥊 Tabla Comparativa: El Resumen Final

| Característica | IP Estática | DHCP (Dinámica) |
| :--- | :--- | :--- |
| **¿Quién la pone?** | El Administrador (Tú) | El Router / Servidor |
| **¿Cambia?** | Nunca | Cada cierto tiempo |
| **Riesgo de error** | Alto (Duplicados) | Muy bajo (Automático) |
| **Esfuerzo** | Pesado (Uno a uno) | Mínimo (Plug & Play) |

---

## 💡 Tip de Cyberbuo para el Examen:
> "Si es un **Servidor**, ponle **Estática**. Si es un **Usuario**, dale **DHCP**. ¡No te líes!"

---
[⬅️ Volver al índice de Redes](./README.md)
