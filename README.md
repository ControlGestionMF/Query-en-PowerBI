 Supabase + Power BI: Consulta sin límite de filas

Este repositorio contiene un script en Power Query (lenguaje M) que permite conectar una tabla de Supabase a Power BI usando paginación automática para evitar el límite de 1000 registros por defecto.

## Características

- Conexión REST a Supabase usando API Key (rol `anon`)
- Descarga todas las filas usando paginación (limit/offset)
- Manejo de errores 416 (Range Not Satisfiable)
- Compatible con tablas con seguridad RLS habilitada

## Requisitos

- Tener una tabla llamada `clientes` en tu proyecto Supabase
- Obtener la `anon public key` desde Settings → API en Supabase

## Uso

1. Abre Power BI → Obtener datos → Consulta en blanco → Editor Avanzado
2. Pega el contenido del archivo `clientes_supabase.pq`
3. Reemplaza tu `apiKey` si es necesario
4. Carga los datos
