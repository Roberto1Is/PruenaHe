```markdown
# Monolito ejemplo: .NET API + SignalR + React

Resumen:
- Backend: ASP.NET Core Web API (.NET 7/8) + EF Core (SQL Server o PostgreSQL).
- Real-time: SignalR (sin Redis, ideal para una sola instancia).
- Frontend: React (SignalR client).
- Autenticación: JWT + roles (admin, analista, técnico).

Archivos de ejemplo incluidos:
- schema.sql (DDL)
- Program.cs (configuración)
- Models/Herramental.cs
- Data/AppDbContext.cs
- Hubs/OrdersHub.cs
- Controllers/HerramentalesController.cs
- src/components/OrderTracker.jsx (React)

Comandos iniciales (backend):
1. Actualiza connection string en appsettings.json (ej: SQL Server o Postgres).
2. dotnet ef migrations add Init
3. dotnet ef database update
4. dotnet run

Comandos iniciales (frontend):
1. npx create-react-app my-app
2. npm install @microsoft/signalr
3. Copiar src/components/OrderTracker.jsx al proyecto y usarlo en una página.

Notas operativas:
- Para entorno de producción con múltiples réplicas y SignalR, añade un backplane (Redis) más adelante.
- Implementa verificación en DELETE para evitar borrar herramentales vinculados a pedidos/producción activa.
- Implementa registros (status_history) para auditar quién y cuándo cambió estatus.
```