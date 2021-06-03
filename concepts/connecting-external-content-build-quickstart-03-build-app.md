<!-- markdownlint-disable MD002 MD025 MD041 -->

<span data-ttu-id="a1ec6-101">在此步骤中，你将创建一个 .NET Core 控制台应用。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-101">In this step, you'll create a .NET Core console app.</span></span> <span data-ttu-id="a1ec6-102">之后，您将创建一个新连接，注册架构并同步项目。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-102">After that you will create a new connection, register the schema, and sync the items.</span></span>

## <a name="create-a-net-core-console-app"></a><span data-ttu-id="a1ec6-103">创建 .NET Core 控制台应用</span><span class="sxs-lookup"><span data-stu-id="a1ec6-103">Create a .NET Core console app</span></span>

1. <span data-ttu-id="a1ec6-104">启动 Visual Studio 2019，然后转到"**文件**  >  **""新建**  >  **Project"。**</span><span class="sxs-lookup"><span data-stu-id="a1ec6-104">Launch Visual Studio 2019 and go to **File** > **New** > **Project**.</span></span>
2. <span data-ttu-id="a1ec6-105">选择控制台 **应用 (.NET 核心)** 模板，然后选择下一 **步**。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-105">Select the **Console App (.NET Core)** template, and select **Next**.</span></span>
3. <span data-ttu-id="a1ec6-106">输入Project **名称**："PartsInventoryConnector"，然后选中"将解决方案和项目放置在同一目录中 **"的** 复选框，然后选择"创建 **"，如下** 图所示。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-106">Enter the **Project name**: "PartsInventoryConnector", and select the checkbox for "**Place solution and project in the same directory**", and select **Create** as shown in the next image.</span></span>

!["配置新项目"部分屏幕截图](images/connectors-images/build7.png)

> [!IMPORTANT]
> <span data-ttu-id="a1ec6-108">在移动到下一步之前，将ApplianceParts.csv文件复制到项目的根文件夹。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-108">Before moving to the next step, copy the ApplianceParts.csv file to the root folder of the project.</span></span>

## <a name="add-nuget-packages"></a><span data-ttu-id="a1ec6-109">添加 Nuget 程序包</span><span class="sxs-lookup"><span data-stu-id="a1ec6-109">Add NuGet packages</span></span>

<span data-ttu-id="a1ec6-110">若要添加NuGet包，请右键单击"Project **解决方案"，** 然后选择"**在终端中打开"。**</span><span class="sxs-lookup"><span data-stu-id="a1ec6-110">To add NuGet packages, first right-click **Project Solution** and select **Open in Terminal**.</span></span>

![显示"打开终端"选项的屏幕截图](images/connectors-images/build8.png)

<span data-ttu-id="a1ec6-112">接下来，在开发人员命令提示符中运行以下 CLI 命令。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-112">Next, run the following CLI commands in the developer command prompt.</span></span>

```dotnetcli
dotnet add package CsvHelper --version 12.1.2
dotnet add package Microsoft.EntityFrameworkCore.Design --version 3.1.3
dotnet add package Microsoft.EntityFrameworkCore.Sqlite --version 3.1.3
dotnet add package Microsoft.Extensions.Configuration.UserSecrets --version 3.1.3
dotnet add package Microsoft.Graph.Beta --version 0.17.0-preview
dotnet add package Microsoft.Identity.Client --version 4.13.0
```

> [!TIP]
> <span data-ttu-id="a1ec6-113">如果 `add package` 命令失败，请检查 **项目的程序包** 源：</span><span class="sxs-lookup"><span data-stu-id="a1ec6-113">If the `add package` command fails, check the **Package Source** of your project:</span></span>
> 1. <span data-ttu-id="a1ec6-114">在"解决方案资源管理器"中选择项目。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-114">Select the project in the Solution Explorer.</span></span>
> 2. <span data-ttu-id="a1ec6-115">转到工具> Nuget 程序包管理器 > 程序包管理器 设置。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-115">Go to Tools > Nuget Package Manager > Package Manager Settings.</span></span>
> 3. <span data-ttu-id="a1ec6-116">检查程序包源，并确保 nuget.&#65279;作为程序包源安装。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-116">Check the Package Sources, and make sure nuget.&#65279;org is installed as package source.</span></span>
>     * <span data-ttu-id="a1ec6-117">名称：nuget.&#65279;org</span><span class="sxs-lookup"><span data-stu-id="a1ec6-117">Name: nuget.&#65279;org</span></span>
>     *  <span data-ttu-id="a1ec6-118">源：https&#65279;：//api.nuget.org/v3/index.json</span><span class="sxs-lookup"><span data-stu-id="a1ec6-118">Source: https&#65279;://api.nuget.org/v3/index.json</span></span>

<!---Used "&#65279;" to prevent auto-generated links --->

## <a name="add-azure-ad-authentication"></a><span data-ttu-id="a1ec6-119">添加 Azure AD 身份验证</span><span class="sxs-lookup"><span data-stu-id="a1ec6-119">Add Azure AD authentication</span></span>

<span data-ttu-id="a1ec6-120">需要此身份验证才能获取必要的 OAuth 访问令牌来调用连接器 API。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-120">This authentication is required to get the necessary OAuth access token to call the connectors API.</span></span>

1. <span data-ttu-id="a1ec6-121">在 **PartsInventoryConnector** 目录中新建一个名为 **Authentication** 的目录。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-121">Create a new directory named **Authentication** in the **PartsInventoryConnector** directory.</span></span>
2. <span data-ttu-id="a1ec6-122">在 Authentication 目录中新建一个名为 ClientCredentialAuthProvider.cs 的文件，将以下代码放在该文件中：</span><span class="sxs-lookup"><span data-stu-id="a1ec6-122">Create a new file in the **Authentication** directory named ClientCredentialAuthProvider.cs and place the following code in that file:</span></span>

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

## <a name="add-user-experience"></a><span data-ttu-id="a1ec6-123">添加用户体验</span><span class="sxs-lookup"><span data-stu-id="a1ec6-123">Add user experience</span></span>

1. <span data-ttu-id="a1ec6-124">在 **PartsInventoryConnector** 目录中新建一个名为 Console **的目录**。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-124">Create a new directory in the **PartsInventoryConnector** directory named **Console**.</span></span>
2. <span data-ttu-id="a1ec6-125">在控制台目录中新建一个名为MenuChoice.cs 的文件，将以下代码放在该文件中：</span><span class="sxs-lookup"><span data-stu-id="a1ec6-125">Create a new file in the **Console** directory named MenuChoice.cs and place the following code in that file:</span></span>

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

## <a name="set-up-data-model"></a><span data-ttu-id="a1ec6-126">设置数据模型</span><span class="sxs-lookup"><span data-stu-id="a1ec6-126">Set up data model</span></span>

1. <span data-ttu-id="a1ec6-127">在 **PartsInventoryConnector** 目录中新建一个名为 Models **的目录**。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-127">Create a new directory in the **PartsInventoryConnector** directory named **Models**.</span></span>
2. <span data-ttu-id="a1ec6-128">在 Models 目录中创建一个名为 AppliancePart.cs 的新文件，将以下代码放在该文件中：</span><span class="sxs-lookup"><span data-stu-id="a1ec6-128">Create a new file in the **Models** directory named AppliancePart.cs, and place the following code in that file:</span></span>


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



3. <span data-ttu-id="a1ec6-129">在 Models 目录中创建一个名为 ApplianceDbContext.cs 的新文件，将以下代码放在该文件中：</span><span class="sxs-lookup"><span data-stu-id="a1ec6-129">Create a new file in the **Models** directory named ApplianceDbContext.cs, and place the following code in that file:</span></span>

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

4. <span data-ttu-id="a1ec6-130">在 **PartsInventoryConnector** 目录中创建一个名为 **Data** 的新目录。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-130">Create a new directory named **Data** in the **PartsInventoryConnector** directory.</span></span>
5. <span data-ttu-id="a1ec6-131">在名为 CsvDataLoader.cs 的数据目录中创建一个新文件，将以下代码放在该文件中： </span><span class="sxs-lookup"><span data-stu-id="a1ec6-131">Create a new file in the **Data** directory named CsvDataLoader.cs and place the following code in that file:</span></span>

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

## <a name="write-the-microsoft-graph-helper-service"></a><span data-ttu-id="a1ec6-132">编写 Microsoft Graph帮助程序服务</span><span class="sxs-lookup"><span data-stu-id="a1ec6-132">Write the Microsoft Graph helper service</span></span>

1. <span data-ttu-id="a1ec6-133">在 **PartsInventoryConnector** 目录中新建一个名为 **MicrosoftGraph** 的目录。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-133">Create a new directory named **MicrosoftGraph** in the **PartsInventoryConnector** directory.</span></span>
2. <span data-ttu-id="a1ec6-134">在名为 CustomSerializer.cs 的 **MicrosoftGraph** 目录中创建一个新文件，将以下代码放在该文件中：</span><span class="sxs-lookup"><span data-stu-id="a1ec6-134">Create a new file in the **MicrosoftGraph** directory named CustomSerializer.cs and place the following code in that file:</span></span>

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

3. <span data-ttu-id="a1ec6-135">在 Microsoft Graph目录中创建一个名为 MicrosoftGraphHelper.cs 的新文件，将下面的代码放在该文件中。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-135">Create a new file in the **Microsoft Graph** directory named MicrosoftGraphHelper.cs and place the code below in that file.</span></span>

    <span data-ttu-id="a1ec6-136">以下代码包含使用 **MicrosoftGraphServiceClient** 生成调用并将其发送到 Microsoft Graph 服务并处理响应的方法。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-136">The following code contains methods that use the **MicrosoftGraphServiceClient** to build and send calls to the Microsoft Graph service and process the response.</span></span>

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

## <a name="initialize-the-microsoft-graph-helper-service"></a><span data-ttu-id="a1ec6-137">初始化 Microsoft Graph帮助程序服务</span><span class="sxs-lookup"><span data-stu-id="a1ec6-137">Initialize the Microsoft Graph helper service</span></span>

<span data-ttu-id="a1ec6-138">打开 Program.cs，将整个内容替换为以下代码：</span><span class="sxs-lookup"><span data-stu-id="a1ec6-138">Open Program.cs and replace the entire content with the following code:</span></span>

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

## <a name="create-the-connection"></a><span data-ttu-id="a1ec6-139">创建连接</span><span class="sxs-lookup"><span data-stu-id="a1ec6-139">Create the connection</span></span>

1. <span data-ttu-id="a1ec6-140">在 **MicrosoftGraph** 下，打开 MicrosoftGraphHelper.cs 文件，在构造函数方法后添加 **以下** 代码。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-140">Under **MicrosoftGraph**, open the MicrosoftGraphHelper.cs file and add the following code after the **constructor** method.</span></span>

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

2. <span data-ttu-id="a1ec6-141">打开 Program.cs 文件，在 **Main** 方法后添加以下代码：</span><span class="sxs-lookup"><span data-stu-id="a1ec6-141">Open the Program.cs file and add the following code after the **Main** method:</span></span>


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

## <a name="register-schema"></a><span data-ttu-id="a1ec6-142">注册架构</span><span class="sxs-lookup"><span data-stu-id="a1ec6-142">Register schema</span></span>

1. <span data-ttu-id="a1ec6-143">在 **MicrosoftGraph** 下，打开 MicrosoftGraphHelper.cs 文件，在构造函数方法后添加 **以下** 代码。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-143">Under **MicrosoftGraph**, open the MicrosoftGraphHelper.cs file and add the following code after the **constructor** method.</span></span>

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

2. <span data-ttu-id="a1ec6-144">打开 Program.cs 文件，在 **Main** 方法后添加以下代码。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-144">Open the Program.cs file and add the following code after the **Main** method.</span></span>

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

## <a name="sync-items"></a><span data-ttu-id="a1ec6-145">同步项目</span><span class="sxs-lookup"><span data-stu-id="a1ec6-145">Sync items</span></span>

1. <span data-ttu-id="a1ec6-146">在 **"Microsoft Graph"** 下，打开 MicrosoftGraphHelper.cs 文件，在 **构造函数** 方法后添加以下代码。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-146">Under **Microsoft Graph**, open the MicrosoftGraphHelper.cs file and add the following code after the **Constructor** method.</span></span>

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

2. <span data-ttu-id="a1ec6-147">打开 Program.cs 文件，在 **Main** 方法后添加以下代码。</span><span class="sxs-lookup"><span data-stu-id="a1ec6-147">Open the Program.cs file and add the following code after the **Main** method.</span></span>

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
