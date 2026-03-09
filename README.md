# 🛡️ Proyecto: Simulación de Ataque de Fuerza Bruta y Auditoría SMB

Bienvenido a mi proyecto de laboratorio para el desafío de **Ciberseguridad de DIO**. En este repositorio presento una simulación práctica de Pentesting enfocada en la explotación controlada de servicios y la importancia de la gestión de identidades.

---

## 🚀 Resumen del Proyecto
Este laboratorio simula un escenario de ataque real sobre un servidor vulnerable (**Metasploitable 2**). El objetivo principal es demostrar cómo un atacante puede escalar desde un simple descubrimiento de red hasta el control de recursos compartidos mediante técnicas de fuerza bruta y **Password Spraying**.

### 🛠️ Tecnologías y Herramientas
* **SO Atacante:** Kali Linux
* **SO Víctima:** Metasploitable 2 (VM)
* **Escaneo:** Nmap, Enum4linux
* **Explotación:** Medusa (Brute Force)
* **Acceso:** Smbclient, FTP

---

## 📂 Contenido del Repositorio
Para ver el detalle técnico paso a paso con mis explicaciones lógicas y comandos utilizados, consulta el siguiente archivo:

📄 **[Ver Informe Técnico Detallado (TXT)](./Laboratorio_Pentesting_Gonzalo.txt)**

*(En este archivo encontrarás el flujo completo: Reconocimiento -> Fingerprinting -> Fuerza Bruta FTP -> Password Spraying SMB -> Acceso Final).*

---

## 🔍 Puntos Clave del Laboratorio
1.  **Reconocimiento:** Identificación de la red local y descubrimiento de la IP víctima.
2.  **Fingerprinting:** Análisis de banners de servicio (`vsftpd 2.3.4`) para confirmar el objetivo.
3.  **Fuerza Bruta Dirigida:** Uso de diccionarios personalizados para comprometer el servicio FTP.
4.  **Movimiento Lateral Silencioso:** Uso de `Password Spraying` en SMB para evadir detecciones y ganar acceso a sub-sistemas.

---

## 🛡️ Conclusiones y Mitigación
La ejecución de este laboratorio resalta la necesidad crítica de:
* Deshabilitar protocolos de texto plano como FTP.
* Implementar políticas de **bloqueo de cuenta** ante intentos fallidos.
* Realizar auditorías periódicas de robustez de contraseñas.

---
**Desarrollado por:** Gonzalo - *Sistemas & Ciberseguridad*
