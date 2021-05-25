<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="927fc-101">下一步是使用 Azure 数据工厂创建管道，以使用 Microsoft 365 将数据从 Azure 存储 帐户提取Microsoft Graph 数据连接。</span><span class="sxs-lookup"><span data-stu-id="927fc-101">The next step is to use the Azure Data Factory to create a pipeline to extract the data from Microsoft 365 to the Azure Storage account using Microsoft Graph data connect.</span></span>

## <a name="create-an-azure-data-factory-pipeline"></a><span data-ttu-id="927fc-102">创建 Azure 数据工厂管道</span><span class="sxs-lookup"><span data-stu-id="927fc-102">Create an Azure Data Factory pipeline</span></span>

1. <span data-ttu-id="927fc-103">打开浏览器并转到 Azure [门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="927fc-103">Open a browser and go to your [Azure Portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="927fc-104">使用具有 Azure 和租户 **全局** 管理员权限Microsoft 365登录。</span><span class="sxs-lookup"><span data-stu-id="927fc-104">Sign in using an account with **Global administrator** rights to your Azure and Microsoft 365 tenants.</span></span>

1. <span data-ttu-id="927fc-105">在边栏导航上，选择 **"创建资源"。**</span><span class="sxs-lookup"><span data-stu-id="927fc-105">On the sidebar navigation, select **Create a resource**.</span></span>

1. <span data-ttu-id="927fc-106">找到"**数据工厂**"资源类型，然后使用以下值创建它，然后选择"创建 **"。**</span><span class="sxs-lookup"><span data-stu-id="927fc-106">Find the **Data Factory** resource type and use the following values to create it, then select **Create**.</span></span>

    1. <span data-ttu-id="927fc-107">**订阅**：选择 Azure 订阅</span><span class="sxs-lookup"><span data-stu-id="927fc-107">**Subscription**: select your Azure subscription</span></span>
    2. <span data-ttu-id="927fc-108">**资源组**：GraphDataConnect</span><span class="sxs-lookup"><span data-stu-id="927fc-108">**Resource group**: GraphDataConnect</span></span>
    3. <span data-ttu-id="927fc-109">**区域**：选取与你的区域相同的 Azure Microsoft 365区域</span><span class="sxs-lookup"><span data-stu-id="927fc-109">**Region**: pick an Azure region in the same region as your Microsoft 365 region</span></span>
    4. <span data-ttu-id="927fc-110">**名称**：dfM365toBlobStorage</span><span class="sxs-lookup"><span data-stu-id="927fc-110">**Name**: dfM365toBlobStorage</span></span>
    5. <span data-ttu-id="927fc-111">**版本**： V2</span><span class="sxs-lookup"><span data-stu-id="927fc-111">**Version**: V2</span></span>

        ![显示成功在 Azure 门户中新建 Azure 数据工厂服务的屏幕截图。](images/data-connect-adf-create.png)

    6. <span data-ttu-id="927fc-113">在 **"Git 配置"** 选项卡中，确保配置 Git 或选择选项"_稍后配置 Git"。_</span><span class="sxs-lookup"><span data-stu-id="927fc-113">In the **Git configuration** tab, make sure you either configure Git or select the option _Configure Git later_.</span></span>

1. <span data-ttu-id="927fc-114">创建 Azure 数据工厂资源后，选择"作者和 **监视器** "磁贴以启动 Azure 数据工厂全屏编辑器。</span><span class="sxs-lookup"><span data-stu-id="927fc-114">After the Azure Data Factory resource is created, select the **Author and Monitor** tile to launch the Azure Data Factory full screen editor.</span></span>

    ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图。](images/data-connect-adf-auth-and-mon.png)

1. <span data-ttu-id="927fc-117">通过从左侧 **导航\*\*\*\*中选择**"概述"，从"管理"体验切换到"管理"体验。</span><span class="sxs-lookup"><span data-stu-id="927fc-117">Switch from the **Overview** to the **Manage** experience by selecting it from the left-hand navigation.</span></span>

1. <span data-ttu-id="927fc-118">默认情况下，Azure 数据工厂将使用自动解析区域集成运行时。</span><span class="sxs-lookup"><span data-stu-id="927fc-118">By default, the Azure Data Factory will use an integration runtime that is auto-resolving the region.</span></span> <span data-ttu-id="927fc-119">由于连接要求源和目标以及集成运行时存在于同一 Microsoft 365 区域，因此建议您创建一个包含固定区域的新集成运行时。</span><span class="sxs-lookup"><span data-stu-id="927fc-119">Because Data Connect requires that your source and destination, and integration runtime to exist in the same Microsoft 365 region, we recommend that you create a new integration runtime with a fixed region.</span></span>

    1. <span data-ttu-id="927fc-120">选择 **"集成运行时**  >  **""新建"。**</span><span class="sxs-lookup"><span data-stu-id="927fc-120">Select **Integration runtimes** > **New**.</span></span>
    2. <span data-ttu-id="927fc-121">选择 **"Azure，自托管"，** 然后选择"继续 **"。**</span><span class="sxs-lookup"><span data-stu-id="927fc-121">Select **Azure, Self-Hosted** and select **Continue**.</span></span>
    3. <span data-ttu-id="927fc-122">选择 **"Azure** 用于网络环境"，然后选择"继续 **"。**</span><span class="sxs-lookup"><span data-stu-id="927fc-122">Select **Azure** for network environment and select **Continue**.</span></span>

        ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图。](images/data-connect-adf-network.png)

    4. <span data-ttu-id="927fc-125">使用以下详细信息在最终屏幕上完成表单，然后选择"创建 **"。**</span><span class="sxs-lookup"><span data-stu-id="927fc-125">Use the following details to complete the form on the final screen and then select **Create**.</span></span>

        - <span data-ttu-id="927fc-126">**名称**：集成运行时的名称</span><span class="sxs-lookup"><span data-stu-id="927fc-126">**Name**: name of your integration runtime</span></span>
        - <span data-ttu-id="927fc-127">**说明**：输入说明</span><span class="sxs-lookup"><span data-stu-id="927fc-127">**Description**: enter a description</span></span>
        - <span data-ttu-id="927fc-128">**区域**：选择与你的区域Microsoft 365区域</span><span class="sxs-lookup"><span data-stu-id="927fc-128">**Region**: select the region that matches your Microsoft 365 region</span></span>
        - <span data-ttu-id="927fc-129">**虚拟网络配置 (预览) ：** 已禁用</span><span class="sxs-lookup"><span data-stu-id="927fc-129">**Virtual network configuration (preview)**: Disabled</span></span>

1. <span data-ttu-id="927fc-130">从左侧 **导航中选择** "管理 **"** 体验切换到"作者"体验。</span><span class="sxs-lookup"><span data-stu-id="927fc-130">Switch from the **Manage** to the **Author** experience by selecting it from the left-hand navigation.</span></span>
1. <span data-ttu-id="927fc-131">通过选择加号图标，然后通过管道 创建新 **管道**。</span><span class="sxs-lookup"><span data-stu-id="927fc-131">Create a new pipeline by selecting the **plus** icon, then **pipeline**.</span></span>

    ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图。](images/data-connect-adf-pipeline-create.png)

    - <span data-ttu-id="927fc-134">将 **"复制数据"** 活动从 **"移动和转换"** 部分拖到设计图面上。</span><span class="sxs-lookup"><span data-stu-id="927fc-134">Drag the **Copy Data** activity from the **Move and Transform** section onto the design surface.</span></span>

        ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图。](images/data-connect-adf-pipeline-copy-data.png)

    - <span data-ttu-id="927fc-137">在设计器中选择活动。</span><span class="sxs-lookup"><span data-stu-id="927fc-137">Select the activity in the designer.</span></span>
    - <span data-ttu-id="927fc-138">选择" **常规"** 选项卡，并指定其名称和说明。</span><span class="sxs-lookup"><span data-stu-id="927fc-138">Select the **General** tab and give it a name and description.</span></span>

      - <span data-ttu-id="927fc-139">**名称**：CopyFromM365toBlobStorage</span><span class="sxs-lookup"><span data-stu-id="927fc-139">**Name**: CopyFromM365toBlobStorage</span></span>
      - <span data-ttu-id="927fc-140">**说明**：您需要的说明。</span><span class="sxs-lookup"><span data-stu-id="927fc-140">**Description**: A description you want.</span></span>

    - <span data-ttu-id="927fc-141">在设计器下面的活动编辑器窗格中，选择"源 **"** 选项卡，然后选择"新建 **"。**</span><span class="sxs-lookup"><span data-stu-id="927fc-141">In the activity editor pane below the designer, select the **Source** tab, then select **New**.</span></span>
    - <span data-ttu-id="927fc-142">找到数据集 **Office 365，** 选择它，然后选择"继续 **"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="927fc-142">Locate the dataset **Office 365**, select it and then select the **Continue** button.</span></span>

        ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图。](images/data-connect-adf-pipeline-dataset.png)

    - <span data-ttu-id="927fc-145">设计器将 **更新"源**"选项卡，Microsoft 365连接器设置。</span><span class="sxs-lookup"><span data-stu-id="927fc-145">The designer will update the **Source** tab with the Microsoft 365 connector settings.</span></span>
    - <span data-ttu-id="927fc-146">选择" **源** 数据集"字段旁边的" **打开"** 选项。</span><span class="sxs-lookup"><span data-stu-id="927fc-146">Select the **Open** option next to the **Source dataset** field.</span></span>
    - <span data-ttu-id="927fc-147">在表设置中，选择"连接 **"** 选项卡，然后选择"新建 **"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="927fc-147">In the table settings, select the **Connection** tab, then the **New** button.</span></span>
    - <span data-ttu-id="927fc-148">在出现的对话框中，分别在"服务主体 **ID"** 和"服务主体密钥"字段中输入之前创建的 Azure AD应用程序的应用程序 ID 和密码 **ID，** 然后选择"创建 **"。**</span><span class="sxs-lookup"><span data-stu-id="927fc-148">In the dialog that appears, enter the previously created Azure AD application's **Application ID** and **Secret ID** in the **Service principal ID** and **Service principal key** fields respectively, then select **Create**.</span></span>
    - <span data-ttu-id="927fc-149">通过"集成运行时"下拉列表选择 **之前在 连接中创建的集成** 运行时。</span><span class="sxs-lookup"><span data-stu-id="927fc-149">Select the integration runtime you previously created in the **Connect via integration runtime** dropdown.</span></span>

        ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图。](images/data-connect-adf-linked-service.png)

    - <span data-ttu-id="927fc-152">创建连接Microsoft 365，对于 **"表**"字段，选择"BasicDataSet_v0"。 **Message_v0**。</span><span class="sxs-lookup"><span data-stu-id="927fc-152">After creating the Microsoft 365 connection, for the **Table** field, select **BasicDataSet_v0.Message_v0**.</span></span>
    - <span data-ttu-id="927fc-153">从 **Office365Table** 切换到 **管道>源**。</span><span class="sxs-lookup"><span data-stu-id="927fc-153">Switch from **Office365Table** to **Pipeline > Source**.</span></span> <span data-ttu-id="927fc-154">对 Date 筛选器 **使用以下值**。</span><span class="sxs-lookup"><span data-stu-id="927fc-154">Use the following values for the **Date filter**.</span></span>

      - <span data-ttu-id="927fc-155">**列名称**：CreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="927fc-155">**Column name**: CreatedDateTime</span></span>
      - <span data-ttu-id="927fc-156">**UTC (开始时间) ：** 选择当前日期之前的某个时间</span><span class="sxs-lookup"><span data-stu-id="927fc-156">**Start time (UTC)**: select a date sometime prior to the current date</span></span>
      - <span data-ttu-id="927fc-157">**UTC (结束) ：** 选择当前日期</span><span class="sxs-lookup"><span data-stu-id="927fc-157">**End time (UTC)**: select the current date</span></span>
      - <span data-ttu-id="927fc-158">选择 **"输出列** "部分 _中的"导入架构_ "。</span><span class="sxs-lookup"><span data-stu-id="927fc-158">Select **Import schema** in the _Output columns_ section.</span></span>

    - <span data-ttu-id="927fc-159">选择管道 **选项卡中的** "复制数据活动"，然后选择" **接收"** 选项卡。</span><span class="sxs-lookup"><span data-stu-id="927fc-159">Select the **Copy data** activity in the pipeline tab, then select the **Sink** tab.</span></span>

      - <span data-ttu-id="927fc-160">选择"**新建"** 按钮，选择 **"Azure Blob 存储"，** 然后选择"继续 **"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="927fc-160">Select the **New** button, select **Azure Blob Storage**, and then select the **Continue** button.</span></span>
      - <span data-ttu-id="927fc-161">选择 **"** 二进制"作为数据的格式，然后选择"继续 **"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="927fc-161">Select **Binary** as the format for the data and then select the **Continue** button.</span></span>
      - <span data-ttu-id="927fc-162">为数据集指定名称 **M365JsonFile，** 如果尚未存在，则创建新的链接服务。</span><span class="sxs-lookup"><span data-stu-id="927fc-162">Give the dataset the name **M365JsonFile** and create new linked service if it does not exist already.</span></span>

    - <span data-ttu-id="927fc-163">在表中，选择"连接 **"** 选项卡，然后选择"新建 **"。**</span><span class="sxs-lookup"><span data-stu-id="927fc-163">In the table select the **Connection** tab, then select **New**.</span></span>
    - <span data-ttu-id="927fc-164">在对话框中设置以下值，然后选择"完成 **"。**</span><span class="sxs-lookup"><span data-stu-id="927fc-164">Set the following values in the dialog, then select **Finish**.</span></span>

        - <span data-ttu-id="927fc-165">**身份验证方法**：服务主体</span><span class="sxs-lookup"><span data-stu-id="927fc-165">**Authentication method**: Service principal</span></span>
        - <span data-ttu-id="927fc-166">**Azure 订阅**：全选</span><span class="sxs-lookup"><span data-stu-id="927fc-166">**Azure subscription**: Select all</span></span>
        - <span data-ttu-id="927fc-167">**存储帐户名称**： mgdcm365datastore</span><span class="sxs-lookup"><span data-stu-id="927fc-167">**Storage account name**: mgdcm365datastore</span></span>
          - <span data-ttu-id="927fc-168">这是本练习前面创建的存储帐户。</span><span class="sxs-lookup"><span data-stu-id="927fc-168">This is the storage account created earlier in this exercise.</span></span>
        - <span data-ttu-id="927fc-169">**租户**：输入 Azure 租户的 ID</span><span class="sxs-lookup"><span data-stu-id="927fc-169">**Tenant**: enter the ID of your Azure tenant</span></span>
        - <span data-ttu-id="927fc-170">**服务主体 ID：** 输入之前创建的 Azure AD 应用程序的 ID</span><span class="sxs-lookup"><span data-stu-id="927fc-170">**Service principal ID**: enter the ID of the Azure AD application you previously created</span></span>
        - <span data-ttu-id="927fc-171">**服务主体密钥**：输入你之前创建的 Azure AD 应用程序的哈希密钥</span><span class="sxs-lookup"><span data-stu-id="927fc-171">**Service principal key**: enter the hashed key of the Azure AD application you previously created</span></span>

    - <span data-ttu-id="927fc-172">在"文件 **路径"字段旁边**，选择"浏览 **"。**</span><span class="sxs-lookup"><span data-stu-id="927fc-172">Next to the **File path** field, select **Browse**.</span></span>
    - <span data-ttu-id="927fc-173">选择之前创建的存储容器的名称。</span><span class="sxs-lookup"><span data-stu-id="927fc-173">Select the name of the storage container you created previously.</span></span>

      ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图。](images/data-connect-adf-sa-fp-config.png)

1. <span data-ttu-id="927fc-176">创建管道后，选择设计器 **顶部的** "全部验证"按钮。</span><span class="sxs-lookup"><span data-stu-id="927fc-176">With the pipeline created, select the **Validate All** button at the top of the designer.</span></span>

1. <span data-ttu-id="927fc-177">在验证 (并修复在) 发现的所有问题后，选择设计器顶部的"全部发布"按钮。 </span><span class="sxs-lookup"><span data-stu-id="927fc-177">After validating (and fixing any issues that were found), select the **Publish All** button at the top of the designer.</span></span>

## <a name="run-the-azure-data-factory-pipeline"></a><span data-ttu-id="927fc-178">运行 Azure 数据工厂管道</span><span class="sxs-lookup"><span data-stu-id="927fc-178">Run the Azure Data Factory Pipeline</span></span>

<span data-ttu-id="927fc-179">创建管道后，现在可以运行它了。</span><span class="sxs-lookup"><span data-stu-id="927fc-179">With the pipeline created, now it is time to run it.</span></span>

> [!NOTE]
> <span data-ttu-id="927fc-180">可能需要几分钟时间才能显示同意请求，并且整个过程 (开始、请求同意以及批准完成管道运行) 同意后，需要 40 分钟以上的时间。</span><span class="sxs-lookup"><span data-stu-id="927fc-180">It can take several minutes for the consent request to appear and it is not uncommon for the entire process (start, requesting consent and after approving the consent completing the pipeline run) to take over 40 minutes.</span></span>

1. <span data-ttu-id="927fc-181">在 Azure 数据工厂设计器中，打开管道后，选择"添加触发器 **>"现在触发"。**</span><span class="sxs-lookup"><span data-stu-id="927fc-181">In the Azure Data Factory designer, with the pipeline open, select **Add trigger > Trigger Now**.</span></span>

    ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图，显示如何在管道中激活触发器。](images/data-connect-adf-run-trigger.png)

1. <span data-ttu-id="927fc-183">启动作业后，从边栏菜单中选择"监视器"以查看当前正在运行的作业。</span><span class="sxs-lookup"><span data-stu-id="927fc-183">After starting the job, from the sidebar menu, select **Monitor** to view current running jobs.</span></span>

1. <span data-ttu-id="927fc-184">在左侧导航栏上，找到" **管道运行** "选项卡并选择它。</span><span class="sxs-lookup"><span data-stu-id="927fc-184">On the left-side navigation bar, locate the **Pipeline runs** tab and select it.</span></span> <span data-ttu-id="927fc-185">选择管道 **名称列下的** 管道以查看活动 **运行**。</span><span class="sxs-lookup"><span data-stu-id="927fc-185">Select the pipeline under the **Pipeline name** column to view the **Activity runs**.</span></span> <span data-ttu-id="927fc-186">此管道将显示为 _"正在进行"。_</span><span class="sxs-lookup"><span data-stu-id="927fc-186">This pipeline will show as _In progress_.</span></span>

    ![Screenshot showing the Azure portal UI for Data Factory， it is showing the pipeline runs list.](images/data-connect-adf-pipeline-runs.png)

1. <span data-ttu-id="927fc-188">进入"活动运行 **"** 视图后，转到位于页面底部的"活动运行"部分。</span><span class="sxs-lookup"><span data-stu-id="927fc-188">After you are in the **Activity runs** view, go to the _Activity runs_ section, which is located in the bottom side of the page.</span></span>

1. <span data-ttu-id="927fc-189">将鼠标悬停在 **活动名称上方** ，然后选择 googles 选项。</span><span class="sxs-lookup"><span data-stu-id="927fc-189">Hover over the **Activity name** and select the googles option.</span></span> <span data-ttu-id="927fc-190">此时将打开" **详细信息"** 选项卡。</span><span class="sxs-lookup"><span data-stu-id="927fc-190">This will bring up the **Details** tab.</span></span>

    ![显示数据工厂活动运行的 Azure 门户 UI 的屏幕截图，用户选择活动名称中的 google 以打开详细信息选项卡。](images/data-connect-adf-pipeline-details.png)

1. <span data-ttu-id="927fc-192">在 **"详细信息** "屏幕中，查找管道活动的状态，如下图所示。</span><span class="sxs-lookup"><span data-stu-id="927fc-192">In the **Details** screen, look for the status of the pipeline activity as highlighted in the following image.</span></span> <span data-ttu-id="927fc-193">在这种情况下，你可以看到它的状态为 **RequestingConsent**。</span><span class="sxs-lookup"><span data-stu-id="927fc-193">In this case you can see it is in a state of **RequestingConsent**.</span></span>

    ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图，其中请求的加载状态设置为"RequestingConsent"。](images/data-connect-adf-wait-for-approval.png)

1. <span data-ttu-id="927fc-195">此时，活动运行在内部暂停，直到有人通过管理中心或 PowerShell Microsoft 365批准同意请求。</span><span class="sxs-lookup"><span data-stu-id="927fc-195">At this point, the activity run is internally paused until someone manually approves the consent request via the Microsoft 365 admin center or via PowerShell.</span></span>
