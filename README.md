System in Asp.Net Mvc using Entity Framework Core 6.0 and Sql Server with Add, Edit and Delete users functions.

1. Need install the packages: "Microsoft.EntityFrameworkCore", "Microsoft.EntityFrameworkCore.Design" and "Microsoft.EntityFrameworkCore.Tools".
2. To update settings from Entity Core Framework version 5.0- to 6.0+, we do not use anymore the class "Startup.cs", the changes now are made in the "Program.cs".
3. In 2022+ versions usually encrypt the files sending to DataBase, so make sure in "appsettings.json" file, the configuration with DataBase must have: "Encrypt = False; Trust Server Certificate=true"".
4. If the solution did not work, for first, delete the "Migration" folder files, you can solve opening the "NuGetPackageManager' Console" and creating new ones:
"Add-Migration CriandoTabelaContatos -Context BancoContext"
and updating it: "Update-Database -Context BancoContext".
