# TODOAPP-abp-CSharp


| 中文步骤                                     | English Steps                                                       |
|---------------------------------------------|---------------------------------------------------------------------|
| 1. **创建数据库**                             | 1. **Create the Database**                                          |
| 在项目根目录下运行命令 `dotnet run --migrate-database`，创建数据库并植入初始数据。 | Run the command `dotnet run --migrate-database` in the root directory of your project to create the database and seed the initial data. |
| 2. **运行应用前的准备**                       | 2. **Before Running the Application**                               |
| 手动运行 `abp install-libs` 命令安装必要的NPM包。 | Manually run the `abp install-libs` command to install required NPM packages. |
| 3. **运行应用程序**                           | 3. **Run the Application**                                          |
| 使用支持.NET的IDE或在项目目录下运行 `dotnet run` 命令。 | Use any IDE that supports .NET or run the `dotnet run` command in the directory of your project. |
| 4. **定义实体**                               | 4. **Defining the Entity**                                          |
| 在项目的Entities文件夹下创建一个新的 `TodoItem` 类。 | Create a new `TodoItem` class in the Entities folder of the project. |
| 5. **数据库集成**                             | 5. **Database Integration**                                         |
| 在 `TodoAppDbContext` 类中添加新的 `DbSet` 属性和映射配置。 | Add a new `DbSet` property and mapping configuration in the `TodoAppDbContext` class. |
| 6. **代码首次迁移**                           | 6. **Code First Migrations**                                        |
| 在项目根目录下运行 `dotnet ef migrations add Added_TodoItem` 和 `dotnet ef database update` 命令，创建并应用数据库迁移。 | Run `dotnet ef migrations add Added_TodoItem` and `dotnet ef database update` commands in the root directory of your project to create and apply the database migration. |
| 7. **创建应用服务**                           | 7. **Creating the Application Service**                             |
| 实现应用服务来管理ToDo项，包括获取列表、创建新项和删除项。 | Implement application services to manage ToDo items, including getting the list, creating new items, and deleting items. |
| 8. **创建数据传输对象（DTO）**                | 8. **Creating the Data Transfer Object (DTO)**                      |
| 在Services/Dtos文件夹下创建 `TodoItemDto` 类。 | Create a `TodoItemDto` class in the Services/Dtos folder.           |
| 9. **实现应用服务**                           | 9. **The Application Service Implementation**                       |
| 在Services文件夹下创建 `TodoAppService` 类，注入并使用 `IRepository`。 | Create a `TodoAppService` class in the Services folder, injecting and using `IRepository`. |
| 10. **用户界面实现**                          | 10. **User Interface Implementation**                               |
| 在UI层展示ToDo项，通过动态JavaScript代理与后端进行交互。 | Display ToDo items on the UI, interacting with the backend via dynamic JavaScript proxies. |
