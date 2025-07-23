# 📊 Lector de Insights para Reuniones Ejecutivas (n8n + OpenAI + Google Docs + Sheets)

Este workflow en [n8n](https://n8n.io/) automatiza el análisis de documentos ejecutivos. Extrae contenido desde un archivo de Google Docs, lo procesa con el LLM para generar un resumen ejecutivo e insights clave, y finalmente guarda los resultados en una hoja de cálculo de Google Sheets para su consulta y seguimiento.

---

## ⚙️ Funcionalidades principales

- 📥 **Lectura automática de documentos en Google Docs**
- 🤖 **Generación de insights y resumen ejecutivo usando OpenAI (GPT-3.5 Turbo)**
- 📊 **Registro de resultados en Google Sheets con fecha y título del documento**
- ✅ Flujo 100% automatizable con posibilidad de escalarlo vía Webhook

---

## 🔁 Flujo de trabajo

```mermaid
graph LR
A[Manual Trigger] --> B[Leer Google Docs]
B --> C[Procesar con OpenAI]
C --> D[Guardar en Google Sheets]
