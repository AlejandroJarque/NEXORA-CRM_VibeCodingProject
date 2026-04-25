# NEXORA CRM — Roadmap

## Progreso
- **Total:** 24 tareas
- **Completadas:** 0
- **Restantes:** 24

---

## 🔴 Alta prioridad

- [ ] 1. Gitflow profesional (estandarizar ramas, commits convencionales y protección de main/develop)
- [ ] 2. Convención respuestas JSON (unificar estructura de respuesta en todos los endpoints)
- [ ] 3. Rate limiting (limitar peticiones por token y por IP con middleware throttle)
- [ ] 4. Deals / Oportunidades (nueva entidad con importe, etapa y fecha de cierre ligada a clientes)
- [ ] 5. Timeline por cliente (vista cronológica agregada de actividades, notas y cambios de estado)

---

## 🟡 Media prioridad

- [ ] 6. Notificaciones / recordatorios (email automático cuando una actividad vence o está próxima)
- [ ] 7. Importación desde CSV (subida y mapeo de clientes, contactos y actividades desde archivo CSV)
- [ ] 8. Modelo contactos (pivot) (migrar client_id directo a tabla pivot para relación muchos a muchos)
- [ ] 9. Comunicación por email SMTP (envío real de emails desde el CRM vía SendGrid)
- [ ] 10. Multi-usuario / Asignación (asignación y transferencia de clientes entre usuarios del sistema)
- [ ] 11. Campos personalizados (permitir que cada usuario añada campos propios a clientes y contactos)
- [ ] 12. Reporting avanzado (embudos de conversión, métricas por vendedor y filtros configurables)

---

## 🎨 Frontend / UX

- [ ] 13. Nuevo design system (nueva paleta, tipografía y componentes con light mode como predeterminado)
- [ ] 14. Bug logout — resetear tema (al hacer logout el tema vuelve a light independientemente del estado anterior)
- [ ] 15. UX Admin — panel completo (interfaz específica para el rol admin, actualmente sin desarrollar)

---

## 🤖 IA — Claude API

- [ ] 16. Asistente conversacional (chat dentro del CRM para consultar datos en lenguaje natural)
- [ ] 17. Sugerencias automáticas (la IA detecta patrones y genera alertas proactivas sobre clientes)
- [ ] 18. Generación de contenido (ayuda a redactar emails, notas y resúmenes desde el contexto del cliente)
- [ ] 19. Análisis del dashboard (Claude interpreta las métricas del dashboard y devuelve conclusiones)

---

## 🟢 Calidad

- [ ] 20. Refresh tokens + revocación (validar renovación de token antes de expirar y revocación en logout)
- [ ] 21. Audit log completo (registrar quién modificó qué, en qué entidad y con qué valores anterior/posterior)
- [ ] 22. Staging environment (entorno intermedio entre local y producción para probar antes de subir)
- [ ] 23. Webhooks salientes (notificar a sistemas externos cuando ocurre un evento en el CRM)
- [ ] 24. Cobertura de tests (ampliar la suite actual para cubrir todos los módulos nuevos)

---

## Notas
- Ritmo: 2h/día — ~14h/semana
- Cada tarea completada: cambia `- [ ]` por `- [x]` y actualiza el contador de arriba
- Al iniciar un chat nuevo: comparte este archivo para que el asistente sepa el estado actual
- Stack: Laravel 12 · React 19 · TypeScript · Claude API · SendGrid
- Repo: CRM_APIrest en GitHub — ramas activas: main y develop