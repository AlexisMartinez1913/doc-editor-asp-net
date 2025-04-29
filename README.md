Este es un editor de texto enriquecido desarrollado con **ASP.NET Core MVC** que permite a los usuarios crear, editar, ver y eliminar documentos personalizados. Utiliza **TinyMCE** como editor WYSIWYG para una experiencia de escritura fluida y moderna.

## 🚀 Características

- ✍️ Editor de texto enriquecido con [TinyMCE](https://www.tiny.cloud/)
- 🧑‍💼 Autenticación de usuarios con ASP.NET Identity
- 📄 CRUD completo de documentos
- 🧠 Cada documento está vinculado al usuario que lo creó
- 🔐 Control de acceso a documentos por usuario
- 📋 Validaciones de formulario con Data Annotations
- 🎨 Interfaz limpia y responsive con Bootstrap

## 🧰 Tecnologías utilizadas

- ASP.NET Core MVC
- Entity Framework Core
- SQL Server
- TinyMCE (con API Key)
- ASP.NET Core Identity
- Bootstrap 5



## 🔧 Instalación y ejecución local

1. Clona el repositorio:

```bash
git clone https://github.com/AlexisMartinez1913/doc-editor-asp-net.git
cd doc-editor-asp-net
Configura la base de datos en appsettings.json:

"ConnectionStrings": {
  "DefaultConnection": "Server=(localdb)\\mssqllocaldb;Database=RichTextDocsDb;Trusted_Connection=True;"
}

```
2. Aplica las migraciones:
```bash

dotnet ef database update
Ejecuta la aplicación:

dotnet run
```

## Configurar la API Key de TinyMCE
Crea una cuenta gratuita en https://www.tiny.cloud/

Obtén tu API Key.

Reemplaza en la vista Create.cshtml:
```bash
<script src="https://cdn.tiny.cloud/1/tu-api-key/tinymce/7/tinymce.min.js" referrerpolicy="origin"></script>
