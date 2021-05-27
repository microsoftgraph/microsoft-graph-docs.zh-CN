<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="45710-101">在此部分中，我们将生成第一 ASP.NET 应用程序，用于处理已导出的 Microsoft Graph 数据连接数据。</span><span class="sxs-lookup"><span data-stu-id="45710-101">In this section we will be building your first ASP.NET project application for to process the Microsoft Graph Data Connect data that was exported.</span></span>

## <a name="create-a-new-aspnet-project"></a><span data-ttu-id="45710-102">新建项目 ASP.NET 项目</span><span class="sxs-lookup"><span data-stu-id="45710-102">Create a new ASP.NET project</span></span>

1. <span data-ttu-id="45710-103">打开Visual Studio，然后选择"文件 **">"新建> Project"。**</span><span class="sxs-lookup"><span data-stu-id="45710-103">Open Visual Studio and select **File > New > Project**.</span></span>

1. <span data-ttu-id="45710-104">在"**新建Project** 对话框中，执行以下操作。</span><span class="sxs-lookup"><span data-stu-id="45710-104">In the **New Project** dialog, do the following.</span></span>

    1. <span data-ttu-id="45710-105">在 **ASP.NET 中** 搜索 Web 应用程序，然后选择"ASP.NET Web **应用程序** (.NET Framework) 选项。</span><span class="sxs-lookup"><span data-stu-id="45710-105">Search **ASP.NET Web Application** in the search box and select the **ASP.NET Web Application (.NET Framework)** option.</span></span>
    1. <span data-ttu-id="45710-106">单击"下一 **步"。**</span><span class="sxs-lookup"><span data-stu-id="45710-106">Click on **Next**.</span></span>

        ![显示使用 Visual Studio Web 应用程序创建新项目的选项的 ASP.NET 屏幕截图。](images/data-connect-vs-create-app.png)

    1. <span data-ttu-id="45710-108">输入 **EmailMetrics** 作为项目名称。</span><span class="sxs-lookup"><span data-stu-id="45710-108">Enter **EmailMetrics** for the name of the project.</span></span>
    1. <span data-ttu-id="45710-109">选择 **.NET Framework 4.7.2** 作为框架选项。</span><span class="sxs-lookup"><span data-stu-id="45710-109">Select **.NET Framework 4.7.2** for the framework option.</span></span>
    1. <span data-ttu-id="45710-110">选择 **创建**。</span><span class="sxs-lookup"><span data-stu-id="45710-110">Select **Create**.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="45710-111">确保为此快速启动说明中指定的Visual Studio Project输入完全相同的名称。</span><span class="sxs-lookup"><span data-stu-id="45710-111">Ensure that you enter the exact same name for the Visual Studio Project that is specified in this quick start instructions.</span></span> <span data-ttu-id="45710-112">Visual Studio 项目名称在代码中成为了命名空间的一部分。</span><span class="sxs-lookup"><span data-stu-id="45710-112">The Visual Studio Project name becomes part of the namespace in the code.</span></span> <span data-ttu-id="45710-113">在这些说明里的代码依赖于匹配在这些说明中指定的 Visual Studio 项目名称的命名空间。</span><span class="sxs-lookup"><span data-stu-id="45710-113">The code inside these instructions depends on the namespace matching the Visual Studio Project name specified in these instructions.</span></span> <span data-ttu-id="45710-114">如果你使用不同的项目名称，代码不会编译，除非你调整所有的命名空间来匹配你在创建项目时输入的 Visual Studio 项目名称。</span><span class="sxs-lookup"><span data-stu-id="45710-114">If you use a different project name the code will not compile unless you adjust all the namespaces to match the Visual Studio Project name you enter when you create the project.</span></span>

    1. <span data-ttu-id="45710-115">在"新建 web **ASP.NET** 项目"对话框中，选择"MVC"。</span><span class="sxs-lookup"><span data-stu-id="45710-115">In the new **ASP.NET Web Application** project dialog, select MVC.</span></span>
    1. <span data-ttu-id="45710-116">选择 **创建**。</span><span class="sxs-lookup"><span data-stu-id="45710-116">Select **Create**.</span></span>

    ![显示用于选择模型Visual Studio-控制器选项的选项的 (MVC) ASP.NET Web 应用程序。](images/data-connect-vs-create-app-mvc.png)

## <a name="add-and-configure-your-azure-storage-as-a-connected-service"></a><span data-ttu-id="45710-118">添加和配置Azure 存储连接服务</span><span class="sxs-lookup"><span data-stu-id="45710-118">Add and configure your Azure Storage as a Connected Service</span></span>

1. <span data-ttu-id="45710-119">在"**解决方案资源管理器**"工具窗口中，右键单击"连接的 **服务**"节点，然后选择"**添加已连接服务"。**</span><span class="sxs-lookup"><span data-stu-id="45710-119">In the **Solution Explorer** tool window, right-click the **Connected Services** node and select **Add Connected Service**.</span></span>

    ![Visual-Studio-Add-Connected-Service](images/data-connect-vs-add-connected-service-sa.png)

1. <span data-ttu-id="45710-121">在" **连接的服务** "对话框中，选择位于对话框右上角 **+** 的绿色符号。</span><span class="sxs-lookup"><span data-stu-id="45710-121">On the **Connected Services** dialog, select the green **+** sign which is located in the upper-right corner of the dialog.</span></span>

1. <span data-ttu-id="45710-122">在"**添加依赖关系"** 对话框中，**选择"Azure 存储"** 下一 **步"。**</span><span class="sxs-lookup"><span data-stu-id="45710-122">In the **Add dependency** dialog, select **Azure Storage** and select **Next**.</span></span>

    ![显示"Visual Studio"选项的"添加依赖关系"对话框的Azure 存储屏幕截图。](images/data-connect-vs-add-dependency-azsa.png)

1. <span data-ttu-id="45710-124">在 **"Azure 存储"** 对话框中，选择在上一练习中导出数据的订阅和存储帐户，选择"下一 **步"。**</span><span class="sxs-lookup"><span data-stu-id="45710-124">In the **Azure Storage** dialog, select the subscription and storage account where you exported the data in the previous exercise, select **Next**.</span></span>

    ![显示配置Visual Studio的 Azure 存储 界面屏幕截图，选择订阅和存储帐户。](images/data-connect-vs-configure-az-storage.png)

1. <span data-ttu-id="45710-126">为连接 **Azure 存储** **AzureStorageConnectionString 的名称，然后选择**"下一 **步"。**</span><span class="sxs-lookup"><span data-stu-id="45710-126">Provide the **Azure Storage connection** a name of **AzureStorageConnectionString** and select **Next**.</span></span>
1. <span data-ttu-id="45710-127">选择 **“完成”**。</span><span class="sxs-lookup"><span data-stu-id="45710-127">Select **Finish**.</span></span>

    ![显示"配置Visual Studio摘要的Azure 存储屏幕截图。](images/data-connect-vs-configure-sa-summary.png)

## <a name="create-a-new-model-class-that-will-be-used-to-store-the-email-metrics"></a><span data-ttu-id="45710-129">创建将用于存储电子邮件指标的新模型类</span><span class="sxs-lookup"><span data-stu-id="45710-129">Create a new model class that will be used to store the email metrics</span></span>

1. <span data-ttu-id="45710-130">在"**解决方案资源管理器**"工具窗口中，右键单击 **"模型**"文件夹，然后选择"**添加>类"。**</span><span class="sxs-lookup"><span data-stu-id="45710-130">In the  **Solution Explorer** tool window, right-click the **Models** folder and select **Add > Class**.</span></span>

    ![显示如何在 models Visual Studio中右键单击来添加新类的屏幕快照。](images/data-connect-vs-add-new-model-class.png)

1. <span data-ttu-id="45710-132">在"**添加新项"对话框中**，选择 **"类**"，将文件名称设置为 _EmailMetric.cs，_ 然后选择"**添加"。**</span><span class="sxs-lookup"><span data-stu-id="45710-132">In the **Add New Item** dialog, select **Class**, set the name of the file to _EmailMetric.cs_ and select **Add**.</span></span>

1. <span data-ttu-id="45710-133">将以下代码添加到刚创建的 EmailMetric 类。</span><span class="sxs-lookup"><span data-stu-id="45710-133">Add the following code to the class EmailMetric you just created.</span></span>

    ```csharp
    public string Email;
    public double RecipientsToEmail;
    ```

## <a name="create-a-new-controller-that-will-calculate-and-display-the-results"></a><span data-ttu-id="45710-134">创建一个将计算和显示结果的新控制器</span><span class="sxs-lookup"><span data-stu-id="45710-134">Create a new controller that will calculate and display the results</span></span>

1. <span data-ttu-id="45710-135">右键单击 **Controllers** 文件夹，然后选择"**添加>控制器"。**</span><span class="sxs-lookup"><span data-stu-id="45710-135">Right-click the **Controllers** folder and select **Add > Controller**.</span></span>

1. <span data-ttu-id="45710-136">在"**添加基** 架"对话框中，选择 **"MVC 5 控制器 - 空"，** 然后选择"**添加"。**</span><span class="sxs-lookup"><span data-stu-id="45710-136">In the **Add Scaffold** dialog, select **MVC 5 Controller - Empty** and select **Add**.</span></span>

1. <span data-ttu-id="45710-137">当系统提示时，命名控制器 **EmailMetricsController，** 然后选择"确定 **"。**</span><span class="sxs-lookup"><span data-stu-id="45710-137">When prompted, name the controller **EmailMetricsController** and select **OK**.</span></span>

1. <span data-ttu-id="45710-138">在包含 **EmailMetricsController** 类的文件顶部的现有 using 语句后添加以下 using 语句。</span><span class="sxs-lookup"><span data-stu-id="45710-138">Add the following using statements after the existing using statements at the top of the file containing the **EmailMetricsController** class.</span></span>

    ```csharp
    using System.Collections.Generic;
    using System.Configuration;
    using System.IO;
    using System.Linq;
    using System.Threading.Tasks;
    using System.Web.Mvc;
    using Azure.Storage.Blobs;
    using Azure.Storage.Blobs.Models;
    using Newtonsoft.Json.Linq;
    ```

1. <span data-ttu-id="45710-139">将以下代码添加到 **EmailMetricsController** 类。</span><span class="sxs-lookup"><span data-stu-id="45710-139">Add the following code to the **EmailMetricsController** class.</span></span> <span data-ttu-id="45710-140">这些将用于连接到包含导出 **Azure 存储** 的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="45710-140">These will be used to connect to the **Azure Storage Account** that contains the exported data.</span></span>

    ```csharp
    private const string connectionStringName = "AzureStorageConnectionString";
    private const string emailBlobName = "m365mails";

    ```

1. <span data-ttu-id="45710-141">将以下方法添加到 **EmailMetricsController** 类。</span><span class="sxs-lookup"><span data-stu-id="45710-141">Add the following method to the **EmailMetricsController** class.</span></span> <span data-ttu-id="45710-142">这将处理 **Azure Blob** 并更新一个集合，该集合代表电子邮件帐户以及为提取的帐户找到的所有电子邮件中合并的收件人数。</span><span class="sxs-lookup"><span data-stu-id="45710-142">This will process an **Azure Blob** and update a collection representing the email accounts and how many recipients there were combined across all emails found for the extracted accounts.</span></span>

    ```csharp
    private async Task ProcessBlobEmails(List<Models.EmailMetric> emailMetrics, BlobClient emailBlob)
    {
        using (var stream = new MemoryStream())
        {
            var response = await emailBlob.DownloadToAsync(stream);
            var pos = stream.Seek(0, SeekOrigin.Begin);

            using (var reader = new StreamReader(stream))
            {

                string line;
                while ((line = reader.ReadLine()) != null)
                {
                    var jsonObj = JObject.Parse(line);

                    // extract sender
                    var sender = jsonObj.SelectToken("Sender.EmailAddress.Address")?.ToString();
                    // No sender - skip this one
                    if (string.IsNullOrEmpty(sender)) continue;

                    // extract and count up recipients
                    var totalRecipients = 0;
                    totalRecipients += jsonObj.SelectToken("ToRecipients")?.Children().Count() ?? 0;
                    totalRecipients += jsonObj.SelectToken("CcRecipients")?.Children().Count() ?? 0;
                    totalRecipients += jsonObj.SelectToken("BccRecipients")?.Children().Count() ?? 0;

                    var emailMetric = new Models.EmailMetric();
                    emailMetric.Email = sender;
                    emailMetric.RecipientsToEmail = totalRecipients;

                    // if already have this sender...
                    var existingMetric = emailMetrics.FirstOrDefault(metric => metric.Email == emailMetric.Email);
                    if (existingMetric != null)
                    {
                        existingMetric.RecipientsToEmail += emailMetric.RecipientsToEmail;
                    }
                    else
                    {
                        emailMetrics.Add(emailMetric);
                    }
                }
            }
        }
    }
    ```

1. <span data-ttu-id="45710-143">将以下方法添加到 **EmailMetricsController** 类。</span><span class="sxs-lookup"><span data-stu-id="45710-143">Add the following method to the **EmailMetricsController** class.</span></span> <span data-ttu-id="45710-144">这将枚举指定帐户的指定Azure 存储中所有 blob，并将每个 blob 发送到上一步 `ProcessBlobEmails()` 中添加的方法。</span><span class="sxs-lookup"><span data-stu-id="45710-144">This will enumerate through all blobs in the specified **Azure Storage** account's specified container and send each one to `ProcessBlobEmails()` method added in the last step.</span></span>

    ```csharp
    private async Task<List<Models.EmailMetric>> ProcessBlobFiles()
    {
        var emailMetrics = new List<Models.EmailMetric>();
        var connectionString = ConfigurationManager.ConnectionStrings[connectionStringName];

        // Connect to the storage account
        var containerClient = new BlobContainerClient(connectionString.ConnectionString, emailBlobName);

        foreach (var blob in containerClient.GetBlobs())
        {
            if (blob.Properties.BlobType == BlobType.Block &&
                // Don't process blobs in the metadata folder
                !blob.Name.StartsWith("metadata/"))
            {
                var blobClient = containerClient.GetBlobClient(blob.Name);
                await ProcessBlobEmails(emailMetrics, blobClient);
            }
        }

        return emailMetrics;
    }
    ```

1. <span data-ttu-id="45710-145">将以下操作添加到 **EmailMetricsController，** 它将使用添加此类的方法处理电子邮件并将结果发送到视图。</span><span class="sxs-lookup"><span data-stu-id="45710-145">Add the following action to the **EmailMetricsController** that will use the methods added this class to process the emails and send the results to the view.</span></span>

    ```csharp
    [HttpPost, ActionName("ShowMetrics")]
    [ValidateAntiForgeryToken]
    public async Task<ActionResult> ShowMetrics()
    {
        var emailMetrics = await ProcessBlobFiles();

        return View(emailMetrics);
    }
    ```

## <a name="create-a-new-view-for-the-emailmetrics-index-action"></a><span data-ttu-id="45710-146">为 EmailMetrics 索引操作创建新视图</span><span class="sxs-lookup"><span data-stu-id="45710-146">Create a new view for the EmailMetrics index action</span></span>

1. <span data-ttu-id="45710-147">在"**解决方案资源管理器**"工具窗口中，右键单击"视图 **">"EmailMetrics"** 文件夹，然后选择"添加>**视图"。**</span><span class="sxs-lookup"><span data-stu-id="45710-147">In the  **Solution Explorer** tool window, right-click the **Views > EmailMetrics** folder and select **Add > View**.</span></span>

1. <span data-ttu-id="45710-148">在"**添加新基架项目**"对话框中，选择 **"MVC 5** 视图"，然后选择"添加 **"。**</span><span class="sxs-lookup"><span data-stu-id="45710-148">In the **Add New Scaffolded Item** dialog box, select **MVC 5 View**, then select **Add**.</span></span>

1. <span data-ttu-id="45710-149">在"**添加视图"** 对话框中，将"**视图** 名称"设置为 **"索引**"，将其余输入控件保留为默认值，然后选择"添加 **"。**</span><span class="sxs-lookup"><span data-stu-id="45710-149">In the **Add View** dialog, set the **View** name to **Index**, leave the remaining input controls to their default values, and select **Add**.</span></span>

    ![显示如何添加Visual Studio索引的新视图的屏幕快照。](images/data-connect-vs-add-view-index.png)

1. <span data-ttu-id="45710-151">将 EmailMetrics 中的新 **Views > _Index.cshtml >中的标记_** 更新为以下内容。</span><span class="sxs-lookup"><span data-stu-id="45710-151">Update the markup in the new **Views > EmailMetrics > _Index.cshtml_** to the following.</span></span> <span data-ttu-id="45710-152">这将添加一个表单，该表单具有一个按钮，该按钮将 HTTP POST 提交到上一步添加的自定义控制器操作。</span><span class="sxs-lookup"><span data-stu-id="45710-152">This will add a form with a single button that will submit an HTTP POST to the custom controller action added in the last step.</span></span>

    ```html
    @{
    ViewBag.Title = "Index";
    }

    <h2>Email Metrics</h2>
    ```

1. <span data-ttu-id="45710-153">此应用程序将查看提取到 **Azure Blob** 帐户存储电子邮件的电子邮件数据，并显示每个发件人的收件人总数。</span><span class="sxs-lookup"><span data-stu-id="45710-153">This application will look at the email data for emails extracted to the **Azure Blob Storage** account and display the total number of recipients from each sender.</span></span>

    ```html
    @using (Html.BeginForm("ShowMetrics", "EmailMetrics", FormMethod.Post))
    {
    @Html.AntiForgeryToken()
    <div>
        <button type="submit">View email metrics</button>
    </div>

    <div>
        <em>Please be patient as this can take a few moments to calculate depending on the size of the exported data...</em>
    </div>
    }
    ```

## <a name="create-a-new-view-for-the-emailmetrics-showmetrics-action"></a><span data-ttu-id="45710-154">为 EmailMetrics ShowMetrics 操作创建新视图</span><span class="sxs-lookup"><span data-stu-id="45710-154">Create a new view for the EmailMetrics ShowMetrics action</span></span>

1. <span data-ttu-id="45710-155">在"**解决方案资源管理器**"工具窗口中，右键单击"视图 **">"EmailMetrics"** 文件夹，然后选择"添加>**视图"。**</span><span class="sxs-lookup"><span data-stu-id="45710-155">In the **Solution Explorer** tool window, right-click the **Views > EmailMetrics** folder and select **Add > View**.</span></span>

1. <span data-ttu-id="45710-156">在"**添加视图"** 对话框中，设置以下值，将其余输入控件保留为默认值，然后选择"添加 **"。**</span><span class="sxs-lookup"><span data-stu-id="45710-156">In the **Add View** dialog, set the following values and leave the remaining input controls to their default values and select **Add**.</span></span>

    - <span data-ttu-id="45710-157">**视图名称**：ShowMetrics</span><span class="sxs-lookup"><span data-stu-id="45710-157">**View name**: ShowMetrics</span></span>
    - <span data-ttu-id="45710-158">**模板**：列表</span><span class="sxs-lookup"><span data-stu-id="45710-158">**Template**: List</span></span>
    - <span data-ttu-id="45710-159">**Model 类**：EmailMetric (EmailMetric.Models) </span><span class="sxs-lookup"><span data-stu-id="45710-159">**Model class**: EmailMetric (EmailMetric.Models)</span></span>

        ![显示如何添加Visual Studio ShowMetrics 的新视图的屏幕快照。](images/data-connect-vs-add-view-showmetrics.png)

    >[!TIP]
    > <span data-ttu-id="45710-161">如果你看不到下拉框中的 **EmailMetric** 模型，请生成解决方案。</span><span class="sxs-lookup"><span data-stu-id="45710-161">In case you can't see the **EmailMetric** model in the dropdown box, please build the solution.</span></span>

1. <span data-ttu-id="45710-162">将 **_ShowMetrics.cshtml_** 中新的 Views > EmailMetrics >中的标记更新为以下内容。</span><span class="sxs-lookup"><span data-stu-id="45710-162">Update the markup in the new **Views > EmailMetrics > _ShowMetrics.cshtml_** to the following.</span></span> <span data-ttu-id="45710-163">这将显示计算结果。</span><span class="sxs-lookup"><span data-stu-id="45710-163">This will display the results of the calculations.</span></span>

    ```html
    @model IEnumerable<EmailMetrics.Models.EmailMetric>

    @{
    ViewBag.Title = "ShowMetrics";
    }

    <h2>Email Metrics</h2>

    <table class="table">
    <tr>
        <th>Sender</th>
        <th>Number of Recipients</th>
    </tr>

    @foreach (var item in Model)
    {
    <tr>
        <td>@Html.DisplayFor(modelItem => item.Email)</td>
        <td>@Html.DisplayFor(modelItem => item.RecipientsToEmail)</td>
    </tr>
    }

    </table>
    ```

## <a name="update-the-navigation-to-have-a-way-to-get-to-the-new-controller"></a><span data-ttu-id="45710-164">更新导航以具有到达新控制器的方法</span><span class="sxs-lookup"><span data-stu-id="45710-164">Update the navigation to have a way to get to the new controller</span></span>

1. <span data-ttu-id="45710-165">在" **解决方案资源管理器** "工具窗口中，找到并打开文件 Views **> Shared > _Layout.cshtml_**。</span><span class="sxs-lookup"><span data-stu-id="45710-165">In the **Solution Explorer** tool window, locate and open the file **Views > Shared > _Layout.cshtml_**.</span></span>
1. <span data-ttu-id="45710-166">用以下代码替换内容。</span><span class="sxs-lookup"><span data-stu-id="45710-166">Replace the contents with the following code.</span></span>

    ```html
    <!-- new code -->
    <li>@Html.ActionLink("Email Metrics", "Index", "EmailMetrics")</li>
    ```

## <a name="test-the-application"></a><span data-ttu-id="45710-167">测试应用程序</span><span class="sxs-lookup"><span data-stu-id="45710-167">Test the application</span></span>

1. <span data-ttu-id="45710-168">In Visual Studio， select **Debug > Start Debugging**.</span><span class="sxs-lookup"><span data-stu-id="45710-168">In Visual Studio, select **Debug > Start Debugging**.</span></span>

1. <span data-ttu-id="45710-169">构建应用程序并加载到新的浏览器窗口中时，选择顶部导航栏中的"电子邮件指标"项。</span><span class="sxs-lookup"><span data-stu-id="45710-169">When the application is built and loads in a new browser window, select the **Email Metrics** item in the top navigation bar.</span></span>

1. <span data-ttu-id="45710-170">在" **电子邮件指标"** 页上，选择" **查看电子邮件指标"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="45710-170">On the **Email Metrics** page, select the **View email metrics** button.</span></span>

    ![显示"查看电子邮件 ASP.NET 按钮的内置 Web 应用程序界面屏幕截图。](images/data-connect-vs-select-view-metrics.png)

1. <span data-ttu-id="45710-172">加载页面时，你将看到在所有电子邮件中找到的电子邮件地址列表，其中包含在两者之间发送的所有收件人的总和，如下图测试电子邮件提取中的一个小示例集所示。</span><span class="sxs-lookup"><span data-stu-id="45710-172">When the page loads, you will see a list of emails addresses that were found among all emails with a sum of all the recipients sent between them, as shown from a small sample set in a test email extract in the following figure.</span></span>

    ![显示查看电子邮件 ASP.NET 结果的内置 Web 应用程序界面屏幕截图。](images/data-connect-vs-show-email-metrics.png)
