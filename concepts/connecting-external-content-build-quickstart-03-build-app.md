---
ms.localizationpriority: medium
ms.openlocfilehash: 5fb7ccc1c9e44db77f2ba199a556d229292cf7a4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59289513"
---
<!-- markdownlint-disable MD002 MD025 MD041 -->

在此步骤中，你将创建一个 .NET Core 控制台应用。 之后，您将创建一个新连接，注册架构并同步项目。

## <a name="create-a-net-core-console-app"></a>创建 .NET Core 控制台应用

1. 启动 Visual Studio 2019，然后转到"**文件**  >  **""新建**  >  **Project"。**
2. 选择控制台 **应用 (.NET 核心)** 模板，然后选择下一 **步**。
3. Enter the **Project name**： "PartsInventoryConnector"， and select the checkbox for " Place solution and project in the **same directory**"， and select **Create** as shown in the next image.

!["配置新项目"部分屏幕截图](images/connectors-images/build7.png)

> [!IMPORTANT]
> 在移动到下一步之前，ApplianceParts.csv文件复制到项目的根文件夹。

## <a name="add-nuget-packages"></a>添加 Nuget 程序包

若要添加NuGet程序包，请右键单击"Project **解决方案"，** 然后选择"**在终端中打开"。**

![显示"打开终端"选项的屏幕截图](images/connectors-images/build8.png)

接下来，在开发人员命令提示符中运行以下 CLI 命令。

```dotnetcli
dotnet add package CsvHelper --version 12.1.2
dotnet add package Microsoft.EntityFrameworkCore.Design --version 3.1.3
dotnet add package Microsoft.EntityFrameworkCore.Sqlite --version 3.1.3
dotnet add package Microsoft.Extensions.Configuration.UserSecrets --version 3.1.3
dotnet add package Microsoft.Graph.Beta --version 0.17.0-preview
dotnet add package Microsoft.Identity.Client --version 4.13.0
```

> [!TIP]
> 如果 `add package` 命令失败，请检查 **项目的程序包** 源：
> 1. 在"解决方案资源管理器"中选择项目。
> 2. 转到工具> Nuget 程序包管理器 > 程序包管理器 设置。
> 3. 检查程序包源，并确保 nuget.&#65279;组织作为程序包源安装。
>     * 名称：nuget.&#65279;org
>     *  源：https&#65279;：//api.nuget.org/v3/index.json

<!---Used "&#65279;" to prevent auto-generated links --->

## <a name="add-azure-ad-authentication"></a>添加 Azure AD 身份验证

需要此身份验证才能获取必要的 OAuth 访问令牌来调用连接器 API。

1. 在 **PartsInventoryConnector** 目录中新建一个名为 **Authentication** 的目录。
2. 在 Authentication 目录中新建一个名为 ClientCredentialAuthProvider.cs 的文件，将以下代码放在该文件中：

```c
// Copyright (c) Microsoft Corporation. All rights reserved.
// Licensed under the MIT license.
using Microsoft.Graph;
using Microsoft.Identity.Client;
using System;
using System.Net.Http;
using System.Net.Http.Headers;
using System.Threading.Tasks;

namespace PartsInventoryConnector.Authentication
{
    public class ClientCredentialAuthProvider : IAuthenticationProvider
    {
        private IConfidentialClientApplication _msalClient;
        private int _maxRetries = 3;

        public ClientCredentialAuthProvider(string appId, string tenantId, string secret)
        {
            _msalClient = ConfidentialClientApplicationBuilder
                .Create(appId)
                .WithTenantId(tenantId)
                .WithClientSecret(secret)
                .Build();
        }

        public async Task AuthenticateRequestAsync(HttpRequestMessage request)
        {
            int retryCount = 0;

            do
            {
                try
                {
                    var result = await _msalClient
                        .AcquireTokenForClient(new[] { "https://graph.microsoft.com/.default" })
                        .ExecuteAsync();

                    if (!string.IsNullOrEmpty(result.AccessToken))
                    {
                        request.Headers.Authorization =
                            new AuthenticationHeaderValue("bearer", result.AccessToken);
                        break;
                    }
                }
                catch (MsalServiceException serviceException)
                {
                    if (serviceException.ErrorCode == "temporarily_unavailable")
                    {
                        await Task.Delay(10000);
                    }
                    else
                    {
                        throw serviceException;
                    }
                }
                catch (Exception exception)
                {
                    throw exception;
                }

                retryCount++;
            } while (retryCount < _maxRetries);
        }
    }
}
```

## <a name="add-user-experience"></a>添加用户体验

1. 在 **PartsInventoryConnector** 目录中新建一个名为 Console **的目录**。
2. 在控制台目录中新建一个名为MenuChoice.cs 的文件，将以下代码放在该文件中：

```c
// Copyright (c) Microsoft Corporation. All rights reserved.
// Licensed under the MIT license.

namespace PartsInventoryConnector.Console
{
    public enum MenuChoice
    {
        Invalid = 0,
        CreateConnection,
        RegisterSchema,
        PushAllItems,
        Exit
    }
}
```

## <a name="set-up-data-model"></a>设置数据模型

1. 在 **PartsInventoryConnector** 目录中新建一个名为 Models **的目录**。
2. 在 Models 目录中创建一个名为 AppliancePart.cs 的新文件，将以下代码放在该文件中：


```c
// Copyright (c) Microsoft Corporation. All rights reserved.
// Licensed under the MIT license.
using Microsoft.Graph;
using Newtonsoft.Json;
using System.Collections.Generic;
using System.ComponentModel.DataAnnotations;

namespace PartsInventoryConnector.Models
{
    public class AppliancePart
    {
        [Key]
        public int PartNumber { get; set; }
        public string Name { get; set; }
        public string Description { get; set; }
        public double Price { get; set; }
        public int Inventory { get; set; }
        [JsonProperty("appliances@odata.type")]
        private const string AppliancesODataType = "Collection(String)";
        public List<string> Appliances { get; set; }

        public Properties AsExternalItemProperties()
        {
            var properties = new Properties
            {
                AdditionalData = new Dictionary<string, object>
                {
                    { "partNumber", PartNumber },
                    { "name", Name },
                    { "description", Description },
                    { "price", Price },
                    { "inventory", Inventory },
                    { "appliances@odata.type", "Collection(String)" },
                    { "appliances", Appliances }
                }
            };

            return properties;
        }
    }
}
```



3. 在 Models 目录中创建一个名为 ApplianceDbContext.cs 的新文件，将以下代码放在该文件中：

```c
using Microsoft.Data.Sqlite;
using Microsoft.EntityFrameworkCore;
using Microsoft.EntityFrameworkCore.ChangeTracking;
using Newtonsoft.Json;
using System;
using System.Collections.Generic;
using System.Linq;

namespace PartsInventoryConnector.Models
{
    public class ApplianceDbContext : DbContext
    {
        public DbSet<AppliancePart> Parts { get; set; }

        protected override void OnConfiguring(DbContextOptionsBuilder options)
        {
            options.UseSqlite("Data Source=parts.db");
        }

        protected override void OnModelCreating(ModelBuilder modelBuilder)
        {
            // EF Core can't store lists, so add a converter for the Appliances
            // property to serialize as a JSON string on save to DB
            modelBuilder.Entity<AppliancePart>()
                .Property(ap => ap.Appliances)
                .HasConversion(
                    v => JsonConvert.SerializeObject(v),
                    v => JsonConvert.DeserializeObject<List<string>>(v)
                );

            // Add LastUpdated and IsDeleted shadow properties
            modelBuilder.Entity<AppliancePart>()
                .Property<DateTime>("LastUpdated")
                .HasDefaultValueSql("datetime()")
                .ValueGeneratedOnAddOrUpdate();
            modelBuilder.Entity<AppliancePart>()
                .Property<bool>("IsDeleted")
                .IsRequired()
                .HasDefaultValue(false);

            // Exclude any soft-deleted items (IsDeleted = 1) from
            // the default query sets
            modelBuilder.Entity<AppliancePart>()
                .HasQueryFilter(a => !EF.Property<bool>(a, "IsDeleted"));
        }

        public override int SaveChanges()
        {
            // Prevent deletes of data, instead mark the item as deleted
            // by setting IsDeleted = true.
            foreach(var entry in ChangeTracker.Entries()
              .Where(e => e.State == EntityState.Deleted))
            {
                if (entry.Entity.GetType() == typeof(AppliancePart))
                {
                    SoftDelete(entry);
                }

            }

            return base.SaveChanges();
        }

        private void SoftDelete(EntityEntry entry)
        {
            var partNumber = new SqliteParameter("@partNumber",
                entry.OriginalValues["PartNumber"]);

            Database.ExecuteSqlRaw(
                "UPDATE Parts SET IsDeleted = 1 WHERE PartNumber = @partNumber",
                partNumber);

            entry.State = EntityState.Detached;
        }
    }
}
```

4. 在 **PartsInventoryConnector** 目录中创建一个名为 **Data** 的新目录。
5. 在名为 CsvDataLoader.cs 的数据目录中创建一个新文件，将以下代码放在该文件中： 

```c
using CsvHelper;
using CsvHelper.Configuration;
using CsvHelper.TypeConversion;
using PartsInventoryConnector.Models;
using System.Collections.Generic;
using System.IO;
using System.Linq;

namespace PartsInventoryConnector.Data
{
    public static class CsvDataLoader
    {
        public static List<AppliancePart> LoadPartsFromCsv(string filePath)
        {
            using (var reader = new StreamReader(filePath))
            using (var csv = new CsvReader(reader))
            {
                csv.Configuration.RegisterClassMap<AppliancePartMap>();
                return new List<AppliancePart>(csv.GetRecords<AppliancePart>());
            }
        }
    }

    public class ApplianceListConverter : DefaultTypeConverter
    {
        public override object ConvertFromString(string text, IReaderRow row, MemberMapData memberMapData)
        {
            var appliances = text.Split(';');
            return new List<string>(appliances);
        }
    }

    public class AppliancePartMap : ClassMap<AppliancePart>
    {
        public AppliancePartMap()
        {
            Map(m => m.PartNumber);
            Map(m => m.Name);
            Map(m => m.Description);
            Map(m => m.Price);
            Map(m => m.Inventory);
            Map(m => m.Appliances).TypeConverter<ApplianceListConverter>();
        }
    }
}
```

## <a name="write-the-microsoft-graph-helper-service"></a>编写 Microsoft Graph帮助程序服务

1. 在 **PartsInventoryConnector** 目录中新建一个名为 **MicrosoftGraph** 的目录。
2. 在名为 CustomSerializer.cs 的 **MicrosoftGraph** 目录中创建一个新文件，将以下代码放在该文件中：

```c
using Microsoft.Graph;
using Newtonsoft.Json;
using Newtonsoft.Json.Converters;
using Newtonsoft.Json.Serialization;
using System;
using System.IO;

namespace PartsInventoryConnector.MicrosoftGraph
{
    // The Microsoft Graph SDK serializes enumerations in camelCase.
    // The Microsoft Graph service currently requires the PropertyType enum
    // to be PascalCase. This will override the Microsoft Graph serialization
    // If the Microsoft Graph service changes to accept camelCase this will no
    // longer be necessary.
    class CustomContractResolver : DefaultContractResolver
    {
        protected override JsonConverter ResolveContractConverter(Type objectType)
        {
            if (typeof(PropertyType).IsAssignableFrom(objectType))
            {
                // This default converter uses PascalCase
                return new StringEnumConverter();
            }
            return base.ResolveContractConverter(objectType);
        }
    }

    // In order to hook up the custom contract resolver for
    // PropertyType, we need to implement a custom serializer to
    // pass to the MicrosoftGraphServiceClient.
    public class CustomSerializer : ISerializer
    {

        private Serializer _microsoftGraphSerializer;
        private JsonSerializerSettings _jsonSerializerSettings;

        public CustomSerializer()
        {
            _microsoftGraphSerializer = new Serializer();

            _jsonSerializerSettings = new JsonSerializerSettings
            {
                ContractResolver = new CustomContractResolver()
            };
        }

        // For deserialize, just pass through to the default
        // Microsoft Graph SDK serializer
        public T DeserializeObject<T>(Stream stream)
        {
            return _microsoftGraphSerializer.DeserializeObject<T>(stream);
        }

        // For deserialize, just pass through to the default
        // Microsoft Graph SDK serializer
        public T DeserializeObject<T>(string inputString)
        {
            return _microsoftGraphSerializer.DeserializeObject<T>(inputString);
        }

        public string SerializeObject(object serializeableObject)
        {
            // If a Schema object is being serialized, do the conversion
            // ourselves
            if (serializeableObject is Schema)
            {
                var foo = JsonConvert.SerializeObject(serializeableObject, _jsonSerializerSettings);
                return foo;
            }

            // Otherwise, just pass through to the default Microsoft Graph SDK serializer
            return _microsoftGraphSerializer.SerializeObject(serializeableObject);
        }
    }
}
```

3. 在 Microsoft Graph  MicrosoftGraphHelper.cs 目录中创建一个新文件，将下面的代码放在该文件中。

    以下代码包含使用 **MicrosoftGraphServiceClient** 生成调用并将其发送到 Microsoft Graph 服务并处理响应的方法。

```c
// Copyright (c) Microsoft Corporation. All rights reserved.
// Licensed under the MIT license.
using Microsoft.Graph;
using Newtonsoft.Json;
using System.Net.Http;
using System.Threading.Tasks;

namespace PartsInventoryConnector.MicrosoftGraph
{
    public class MicrosoftGraphHelper
    {
        private class MicrosoftGraphServiceClient _microsoftGraphClient;

        public MicrosoftGraphHelper(IAuthenticationProvider authProvider)
        {
            // Configure a default HttpProvider with our
            // custom serializer to handle the PropertyType serialization
            var serializer = new CustomSerializer();
            var httpProvider = new HttpProvider(serializer);

            // Initialize the Microsoft Graph client
            _microsoftGraphClient = new MicrosoftGraphServiceClient(authProvider, httpProvider);
        }
    }
}
```

## <a name="initialize-the-microsoft-graph-helper-service"></a>初始化 Microsoft Graph帮助程序服务

打开 Program.cs，将整个内容替换为以下代码：

```c
using Microsoft.EntityFrameworkCore;
using Microsoft.Extensions.Configuration;
using Microsoft.Graph;
using PartsInventoryConnector.Authentication;
using PartsInventoryConnector.Console;
using PartsInventoryConnector.Data;
using PartsInventoryConnector.MicrosoftGraph;
using PartsInventoryConnector.Models;
using System;
using System.Collections.Generic;
using System.Linq;
using System.Threading.Tasks;

namespace PartsInventoryConnector
{
    class Program
    {
        private static MicrosoftGraphHelper _microsoftGraphHelper;

        private static ExternalConnection _currentConnection;

        private static string _tenantId;

        static async Task Main(string[] args)
        {
            try
            {
                // Load configuration from appsettings.json
                var appConfig = LoadAppSettings();
                if (appConfig == null)
                {
                    return;
                }

                // Save tenant ID for setting ACL on items
                _tenantId = appConfig["tenantId"];

                // Initialize the auth provider
                var authProvider = new ClientCredentialAuthProvider(
                    appConfig["appId"],
                    appConfig["tenantId"],
                    appConfig["appSecret"]
                );

                // Check if the database is empty
                using (var db = new ApplianceDbContext())
                {
                    if (db.Parts.IgnoreQueryFilters().Count() <= 0)
                    {
                        ImportCsvToDatabase(db, "ApplianceParts.csv");
                    }
                }

                _microsoftGraphHelper = new MicrosoftGraphHelper(authProvider);

                do
                {
                    var userChoice = DoMenuPrompt();

                    switch (userChoice)
                    {
                        case MenuChoice.CreateConnection:
                            await CreateConnectionAsync();
                            break;
                        case MenuChoice.RegisterSchema:
                            await RegisterSchemaAsync();
                            break;
                        case MenuChoice.PushAllItems:
                            await UpdateItemsFromDatabase();
                            break;
                        case MenuChoice.Exit:
                            // Exit the program
                            return;
                        case MenuChoice.Invalid:
                        default:
                            break;
                    }

                } while (true);
            }
            catch (Exception ex)
            {
                System.Console.WriteLine(ex.Message);
            }
        }

        private static void ImportCsvToDatabase(ApplianceDbContext db, string partsFilePath)
        {
            var parts = CsvDataLoader.LoadPartsFromCsv(partsFilePath);
            db.AddRange(parts);
            db.SaveChanges();
        }

        private static MenuChoice DoMenuPrompt()
        {
            System.Console.WriteLine($"Current connection: {(_currentConnection == null ? "NONE" : _currentConnection.Name)}");
            System.Console.WriteLine("Please choose one of the following options:");

            System.Console.WriteLine($"{Convert.ToInt32(MenuChoice.CreateConnection)}. Create a connection");
            System.Console.WriteLine($"{Convert.ToInt32(MenuChoice.RegisterSchema)}. Register schema for current connection");
            System.Console.WriteLine($"{Convert.ToInt32(MenuChoice.PushAllItems)}. Push ALL items to current connection");
            System.Console.WriteLine($"{Convert.ToInt32(MenuChoice.Exit)}. Exit");

            try
            {
                var choice = int.Parse(System.Console.ReadLine());
                return (MenuChoice)choice;
            }
            catch (FormatException)
            {
                return MenuChoice.Invalid;
            }
        }
        private static string PromptForInput(string prompt, bool valueRequired)
        {
            string response = null;

            do
            {
                System.Console.WriteLine($"{prompt}:");
                response = System.Console.ReadLine();
                if (valueRequired && string.IsNullOrEmpty(response))
                {
                    System.Console.WriteLine("You must provide a value");
                }
            } while (valueRequired && string.IsNullOrEmpty(response));

            return response;
        }

        private static IConfigurationRoot LoadAppSettings()
        {
            var appConfig = new ConfigurationBuilder()
                .AddUserSecrets<Program>()
                .Build();

            // Check for required settings
            if (string.IsNullOrEmpty(appConfig["appId"]) ||
                string.IsNullOrEmpty(appConfig["appSecret"]) ||
                string.IsNullOrEmpty(appConfig["tenantId"]))
            {
                return null;
            }

            return appConfig;
        }
    }
}
```

## <a name="create-the-connection"></a>创建连接

1. 在 **MicrosoftGraph** 下，打开 MicrosoftGraphHelper.cs 文件，在构造函数方法后添加 **以下** 代码。

```c
#region Connections

        public async Task<ExternalConnection> CreateConnectionAsync(string id, string name, string description)
        {
            var newConnection = new ExternalConnection
            {
                // Need to set to null, service returns 400
                // if @odata.type property is sent
                ODataType = null,
                Id = id,
                Name = name,
                Description = description
            };

            return await _microsoftGraphClient.External.Connections.Request().AddAsync(newConnection);
        }

#endregion
```

2. 打开 Program.cs 文件，在 **Main** 方法后添加以下代码：


```c
private static async Task CreateConnectionAsync()
        {
            var connectionId = PromptForInput("Enter a unique ID for the new connection", true);
            var connectionName = PromptForInput("Enter a name for the new connection", true);
            var connectionDescription = PromptForInput("Enter a description for the new connection", false);

            try
            {
                // Create the connection
                _currentConnection = await _microsoftGraphHelper.CreateConnectionAsync(connectionId, connectionName, connectionDescription);
          System.Console.WriteLine("New connection created");
                System.Console.WriteLine(Newtonsoft.Json.JsonConvert.SerializeObject(_currentConnection, Newtonsoft.Json.Formatting.Indented));
            }
            catch (ServiceException serviceException)
            {
                System.Console.WriteLine(serviceException.Message);
                return;
            }
      }
```

## <a name="register-schema"></a>注册架构

1. 在 **MicrosoftGraph** 下，打开 MicrosoftGraphHelper.cs 文件，在构造函数方法后添加 **以下** 代码。

```c
#region Schema

        public async Task RegisterSchemaAsync(string connectionId, Schema schema)
        {
            // Need access to the HTTP response here since we are doing an
            // async request. The new schema object isn't returned, we need
            // the Location header from the response
            var asyncNewSchemaRequest = _microsoftGraphClient.External.Connections[connectionId].Schema
                .Request()
                .Header("Prefer", "respond-async")
                .GetHttpRequestMessage();

            asyncNewSchemaRequest.Method = HttpMethod.Post;
            asyncNewSchemaRequest.Content = _microsoftGraphClient.HttpProvider.Serializer.SerializeAsJsonContent(schema);

            var response = await _microsoftGraphClient.HttpProvider.SendAsync(asyncNewSchemaRequest);

            if (response.IsSuccessStatusCode)
            {
                // Get the operation ID from the Location header
                var operationId = ExtractOperationId(response.Headers.Location);
                await CheckSchemaStatusAsync(connectionId, operationId);
            }
            else
            {
                throw new ServiceException(
                    new Error
                    {
                        Code = response.StatusCode.ToString(),
                        Message = "Registering schema failed"
                    }
                );
            }
        }

        private string ExtractOperationId(System.Uri uri)
        {
            int numSegments = uri.Segments.Length;
            return uri.Segments[numSegments - 1];
        }

        public async Task CheckSchemaStatusAsync(string connectionId, string operationId)
        {
            do
            {
                var operation = await _microsoftGraphClient.External.Connections[connectionId]
                    .Operations[operationId]
                    .Request()
                    .GetAsync();

                if (operation.Status == ConnectionOperationStatus.Completed)
                {
                    return;
                }
                else if (operation.Status == ConnectionOperationStatus.Failed)
                {
                    throw new ServiceException(
                        new Error
                        {
                            Code = operation.Error.ErrorCode,
                            Message = operation.Error.Message
                        }
                    );
                }

                await Task.Delay(3000);
            } while (true);
        }

#endregion
```

2. 打开 Program.cs 文件，在 **Main** 方法后添加以下代码。

```c
private static async Task RegisterSchemaAsync()
        {
            if (_currentConnection == null)
            {
                System.Console.WriteLine("No connection selected. Please create a new connection or select an existing connection.");
                return;
            }

            System.Console.WriteLine("Registering schema, this may take a moment...");

            try
            {
                // Register the schema
                var schema = new Schema
                {
                    // Need to set to null, service returns 400
                    // if @odata.type property is sent
                    ODataType = null,
                    BaseType = "microsoft.graph.externalItem",
                    Properties = new List<Property>
                    {
                        new Property { Name = "partNumber", Type = PropertyType.Int64, IsQueryable = true, IsSearchable = false, IsRetrievable = true },
                        new Property { Name = "name", Type = PropertyType.String, IsQueryable = true, IsSearchable = true, IsRetrievable = true },
                        new Property { Name = "description", Type = PropertyType.String, IsQueryable = false, IsSearchable = true, IsRetrievable = true },
                        new Property { Name = "price", Type = PropertyType.Double, IsQueryable = true, IsSearchable = false, IsRetrievable = true },
                        new Property { Name = "inventory", Type = PropertyType.Int64, IsQueryable = true, IsSearchable = false, IsRetrievable = true },
                        new Property { Name = "appliances", Type = PropertyType.StringCollection, IsQueryable = true, IsSearchable = true, IsRetrievable = true }
                    }
                };

                await _microsoftGraphHelper.RegisterSchemaAsync(_currentConnection.Id, schema);
                System.Console.WriteLine("Schema registered");
            }
            catch (ServiceException serviceException)
            {
                System.Console.WriteLine($"{serviceException.StatusCode} error registering schema:");
                System.Console.WriteLine(serviceException.Message);
                return;
            }
        }
```

## <a name="sync-items"></a>同步项目

1. 在 **"microsoft Graph"** 下，打开 MicrosoftGraphHelper.cs 文件，在 **构造函数** 方法后添加以下代码。

```c
#region PushData

        public async Task AddOrUpdateItem(string connectionId, ExternalItem item)
        {
            // The SDK's auto-generated request builder uses POST here,
            // which isn't correct. For now, get the HTTP request and change it
            // to PUT manually.
            var putItemRequest = _microsoftGraphClient.External.Connections[connectionId]
                .Items[item.Id].Request().GetHttpRequestMessage();

            putItemRequest.Method = HttpMethod.Put;
            putItemRequest.Content = _microsoftGraphClient.HttpProvider.Serializer.SerializeAsJsonContent(item);

            var response = await _microsoftGraphClient.HttpProvider.SendAsync(putItemRequest);
            if (!response.IsSuccessStatusCode)
            {
                throw new ServiceException(
                    new Error
                    {
                        Code = response.StatusCode.ToString(),
                        Message = "Error indexing item."
                    }
                );
            }
        }

        #endregion
```

2. 打开 Program.cs 文件，在 **Main** 方法后添加以下代码。

```c
private static async Task UpdateItemsFromDatabase()
        {
            if (_currentConnection == null)
            {
                System.Console.WriteLine("No connection selected. Please create a new connection or select an existing connection.");
                return;
            }

            List<AppliancePart> partsToUpload = null;

            using (var db = new ApplianceDbContext())
            {
                partsToUpload = db.Parts
                    .ToList();
            }

            System.Console.WriteLine($"Processing {partsToUpload.Count()} add/updates");

            foreach (var part in partsToUpload)
            {
                var newItem = new ExternalItem
                {
                    Id = part.PartNumber.ToString(),
                    Content = new ExternalItemContent
                    {
                        // Need to set to null, service returns 400
                        // if @odata.type property is sent
                        ODataType = null,
                        Type = ExternalItemContentType.Text,
                        Value = part.Description
                    },
                    Acl = new List<Acl>
                    {
                        new Acl {
                            AccessType = AccessType.Grant,
                            Type = AclType.Everyone,
                            Value = _tenantId,
                            IdentitySource = "Azure Active Directory"
                        }
                    },
                    Properties = part.AsExternalItemProperties()
                };

                try
                {
                    System.Console.Write($"Uploading part number {part.PartNumber}...");
                    await _microsoftGraphHelper.AddOrUpdateItem(_currentConnection.Id, newItem);
                    System.Console.WriteLine("DONE");
                }
                catch (ServiceException serviceException)
                {
                    System.Console.WriteLine("FAILED");
                    System.Console.WriteLine($"{serviceException.StatusCode} error adding or updating part {part.PartNumber}");
                    System.Console.WriteLine(serviceException.Message);
                }
            }
        }
```
