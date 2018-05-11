# <a name="integrate-security-api-alerts-with-your-siem-using-azure-monitor"></a><span data-ttu-id="bd1fd-101">使用 Azure Monitor 将安全 API 警报与 SIEM 集成</span><span class="sxs-lookup"><span data-stu-id="bd1fd-101">Integrate security API alerts with your SIEM using Azure Monitor</span></span>

<span data-ttu-id="bd1fd-102">Microsoft Graph 中的安全 API 提供了通过单个 REST 终结点来管理多个不同安全产品（称为“提供程序”）中安全警报的功能。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-102">The security API in Microsoft Graph provides the ability to manage security alerts from many different security products, known as providers, through a single REST endpoint.</span></span> <span data-ttu-id="bd1fd-103">某些组织可能已将 Azure 特定日志数据通过 Azure Monitor 引入 SIEM 解决方案。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-103">Some organizations might already ingest Azure specific log data through Azure Monitor into SIEM solutions.</span></span> <span data-ttu-id="bd1fd-104">为了便于集成，通过 REST API 获取的安全警报也可通过 Azure Monitor 获取。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-104">To facilitate ease of integration, the security alerts available through the REST API are also made available through Azure Monitor.</span></span> <span data-ttu-id="bd1fd-105">如果组织已使用 SIEM 解决方案配置了 Azure Monitor 集成，就可以将组织的安全警报轻松地添加到通过 Azure Monitor 获取的数据中。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-105">If your organization has already configured Azure Monitor integration with your SIEM solution, you can now easily add your organization’s security alerts to the data available through Azure Monitor.</span></span> <span data-ttu-id="bd1fd-106">本文将指导你完成启用此集成的步骤。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-106">This article will guide you through the steps to enable this integration.</span></span>

<span data-ttu-id="bd1fd-107">Azure Monitor 支持各种供应商提供的多个不同的 SIEM 连接器。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-107">Azure Monitor supports several different SIEM connectors from various vendors.</span></span> <span data-ttu-id="bd1fd-108">有关 Azure Monitor 的 SIEM 工具和连接器的非详尽列表，请参阅文章[向事件中心发送监控数据](https://docs.microsoft.com/zh-CN/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub)。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-108">For a non-exhaustive list of SIEM tools with connectors for Azure Monitor data, see the article [Send monitoring data to an event hub](https://docs.microsoft.com/zh-CN/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub).</span></span> <span data-ttu-id="bd1fd-109">本文步骤 1 和步骤 2 中的说明都与通过事件中心支持使用的所有 Azure Monitor 连接器相关。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-109">The instructions in Step 1 and Step 2 of this article are relevant for all Azure Monitor connectors supporting consumption via event hub.</span></span> <span data-ttu-id="bd1fd-110">本文介绍了 Splunk SIEM 连接器的端到端配置。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-110">This article describes the end-to-end configuration for the Splunk SIEM connector.</span></span>

<span data-ttu-id="bd1fd-111">此集成过程包含下列步骤：</span><span class="sxs-lookup"><span data-stu-id="bd1fd-111">The integration process involves the following steps:</span></span>

1. [<span data-ttu-id="bd1fd-112">设置 Azure 事件中心以接收租户的安全警报</span><span class="sxs-lookup"><span data-stu-id="bd1fd-112">Set up Azure your event hub to receive security alerts for your tenant</span></span>](#step-1-set-up-an-event-hubs-namespace-in-azure-to-receive-security-alerts-for-your-tenant)
2. [<span data-ttu-id="bd1fd-113">配置 Azure Monitor 以将租户的安全警报发送至事件中心</span><span class="sxs-lookup"><span data-stu-id="bd1fd-113">Configure Azure Monitor to send security alerts from your tenant to the event hub</span></span>](#step-2-configure-azure-monitor-to-send-security-alerts-from-your-tenant-to-the-event-hub)
3. [<span data-ttu-id="bd1fd-114">下载和安装 Splunk 的 Azure Monitor 加载项，以允许 Splunk 使用安全警报</span><span class="sxs-lookup"><span data-stu-id="bd1fd-114">Download and install the Azure Monitor Add-on for Splunk which will allow Splunk to consume security alerts</span></span>](#step-3-download-and-install-the-azure-monitor-add-on-for-splunk-which-will-allow-splunk-to-consume-security-alerts)
4. [<span data-ttu-id="bd1fd-115">使用租户 Azure Active Directory 注册一个供 Splunk 从事件中心进行读取的应用程序</span><span class="sxs-lookup"><span data-stu-id="bd1fd-115">Register an application with your tenant Azure Active Directory which Splunk will use to read from the event hub</span></span>](#step-4-register-an-application-with-your-tenant-azure-active-directory-which-splunk-will-use-to-read-from-the-event-hub )
5. [<span data-ttu-id="bd1fd-116">创建 Azure Key Vault 以存储事件中心的访问密钥</span><span class="sxs-lookup"><span data-stu-id="bd1fd-116">Create an Azure Key vault to store the access key for the event hub</span></span>](#step-5-create-an-azure-key-vault-to-store-the-access-key-for-the-event-hub)
6. [<span data-ttu-id="bd1fd-117">配置 Splunk 数据输入以使用存储在事件中心的安全警报</span><span class="sxs-lookup"><span data-stu-id="bd1fd-117">Configure the Splunk data inputs to consume security alerts stored in the event hub</span></span>](#step-6-configure-the-splunk-data-inputs-to-consume-security-alerts-stored-in-the-event-hub)

<span data-ttu-id="bd1fd-118">完成这些步骤后，Splunk Enterprise 将使用获许可租户的所有 Microsoft Graph 集成安全产品的安全警报。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-118">After you complete these steps, your Splunk Enterprise will consume security alerts from all the Microsoft Graph integrated security products for which your tenant is licensed.</span></span> <span data-ttu-id="bd1fd-119">许可的任何新安全产品也将通过此连接发送警报（在同一架构且无需进一步集成）。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-119">Any new security products that you license will also send alerts through this connection, in the same schema with no further integration work needed.</span></span>

## <a name="step-1-set-up-an-event-hubs-namespace-in-azure-to-receive-security-alerts-for-your-tenant"></a><span data-ttu-id="bd1fd-120">步骤 1：在 Azure 中设置事件中心命名空间，以接收租户的安全警报。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-120">Step 1: Set up an Event Hubs namespace in Azure to receive security alerts for your tenant</span></span>

<span data-ttu-id="bd1fd-121">首先，需要创建 Microsoft Azure 事件中心命名空间和事件中心。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-121">To begin, you need to create a Microsoft Azure Event Hubs namespace and event hub.</span></span> <span data-ttu-id="bd1fd-122">此命名空间和事件中心是所有组织的安全警报的目标。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-122">This namespace and event hub is the destination for all your organization’s security alerts.</span></span> <span data-ttu-id="bd1fd-123">事件中心命名空间是共享同一访问策略的事件中心的逻辑分组。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-123">An Event Hubs namespace is a logical grouping of event hubs that share the same access policy.</span></span> <span data-ttu-id="bd1fd-124">请注意有关你创建的事件中心命名空间和事件中心的一些详细信息：</span><span class="sxs-lookup"><span data-stu-id="bd1fd-124">Note a few details about the Event Hubs namespace and event hubs that you create:</span></span>

- <span data-ttu-id="bd1fd-125">我们建议使用标准事件中心命名空间（尤其是当你通过这些相同的事件中心发送其他 Azure 监控数据时）。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-125">We recommend using a Standard Event Hubs namespace, particularly if you are sending other Azure monitoring data through these same event hubs.</span></span>
- <span data-ttu-id="bd1fd-126">通常情况下，一个吞吐量单位就已足够。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-126">Typically, only one throughput unit is necessary.</span></span> <span data-ttu-id="bd1fd-127">如果随着使用情况的增加而需要扩展吞吐量，则可在以后随时手动增加命名空间的吞吐量单位数或启用自动膨胀。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-127">If you need to scale up as your usage increases, you can always manually increase the number of throughput units for the namespace later or enable auto inflation.</span></span>
- <span data-ttu-id="bd1fd-128">吞吐量单位数可让你增加事件中心的吞吐量比例。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-128">The number of throughput units allows you to increase throughput scale for your event hubs.</span></span> <span data-ttu-id="bd1fd-129">分区数可让你跨多个使用者并行使用。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-129">The number of partitions allows you to parallelize consumption across many consumers.</span></span> <span data-ttu-id="bd1fd-130">单个分区可执行最多 20MBps，或大约每秒 20,000 封邮件。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-130">A single partition can do up to 20MBps, or approximately 20,000 messages per second.</span></span> <span data-ttu-id="bd1fd-131">分区是否支持从多个分区使用要取决于使用数据的工具。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-131">Depending on the tool consuming the data, it may or may not support consuming from multiple partitions.</span></span> <span data-ttu-id="bd1fd-132">如果不确定要设置的分区数，我们建议从设置四个分区开始。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-132">If you're not sure about the number of partitions to set, we recommend starting with four partitions.</span></span>
- <span data-ttu-id="bd1fd-133">我们建议将事件中心的消息保留设置为 7 天。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-133">We recommend that you set message retention on your event hub to 7 days.</span></span> <span data-ttu-id="bd1fd-134">在你使用的工具停用多天时，该设置可确保工具能够从上次停用的位置继续工作（针对最多 7 天的事件）。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-134">If your consuming tool goes down for more than a day, this ensures that the tool can pick up where it left off (for events up to 7 days old).</span></span>
- <span data-ttu-id="bd1fd-135">我们建议为事件中心使用默认的使用者组。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-135">We recommend using the default consumer group for your event hub.</span></span> <span data-ttu-id="bd1fd-136">无需创建其他使用者组或使用单独的使用者组，除非你计划用两个不同的工具使用来自同一事件中心的同一数据。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-136">You don't need to create other consumer groups or use a separate consumer group unless you plan to have two different tools consume the same data from the same event hub.</span></span>
- <span data-ttu-id="bd1fd-137">通常情况下，对于使用事件中心数据的计算机，必须打开端口 5671 和 5672。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-137">Typically, port 5671 and 5672 must be opened on the machine consuming data from the event hub.</span></span>

<span data-ttu-id="bd1fd-138">另请参阅 [Azure 事件中心常见问题解答](https://docs.microsoft.com/zh-CN/azure/event-hubs/event-hubs-faq)。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-138">Also see the [Azure Event Hubs FAQ](https://docs.microsoft.com/zh-CN/azure/event-hubs/event-hubs-faq).</span></span>

1. <span data-ttu-id="bd1fd-139">登录到 [Azure 门户](https://portal.azure.com/)，并选择屏幕左上角的“创建资源”****。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-139">Log on to the [Azure portal](https://portal.azure.com/) and choose **Create a resource** at the top left of the screen.</span></span>

    ![创建资源图像](../concepts/images/create-resource.png)

2. <span data-ttu-id="bd1fd-141">选择“物联网”****，并选择“事件中心”****。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-141">Select **Internet of Things** and choose **Event Hubs**.</span></span>

    ![事件中心图像](../concepts/images/event-hubs.png)

3. <span data-ttu-id="bd1fd-143">在“创建命名空间”**** 中，输入命名空间名称。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-143">In **Create namespace**, enter a namespace name.</span></span> <span data-ttu-id="bd1fd-144">确保命名空间名称可用后，选择定价层（基本或标准）。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-144">After making sure the namespace name is available, choose the pricing tier (Basic or Standard).</span></span> <span data-ttu-id="bd1fd-145">此外，选择 Azure 订阅、资源组以及创建资源的位置。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-145">Also, choose an Azure subscription, resource group, and location in which to create the resource.</span></span> <span data-ttu-id="bd1fd-146">选择“创建”**** 以创建命名空间。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-146">Choose **Create** to create the namespace.</span></span> <span data-ttu-id="bd1fd-147">你可能需要等待几分钟的时间，以使系统完全预配资源。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-147">You might have to wait a few minutes for the system to fully provision the resources.</span></span>

    ![创建命名空间图像](../concepts/images/create-namespace.png)

## <a name="step-2-configure-azure-monitor-to-send-security-alerts-from-your-tenant-to-the-event-hub"></a><span data-ttu-id="bd1fd-149">步骤 2：配置 Azure Monitor 以将租户的安全警报发送至事件中心</span><span class="sxs-lookup"><span data-stu-id="bd1fd-149">Step 2: Configure Azure Monitor to send security alerts from your tenant to the event hub</span></span>

<span data-ttu-id="bd1fd-150">通过 Azure Monitor 为整个 Azure Active Directory (Azure AD) 租户启用组织安全警报的流式处理操作已执行一次。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-150">Enabling the streaming of your organization’s security alerts through Azure Monitor is done one time for your entire Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="bd1fd-151">所有安全 API 许可和启用的产品都将开始向 Azure Monitor 发送安全警报，流式处理数据以使用应用程序。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-151">All security API licensed and enabled products will begin sending security alerts to Azure Monitor, streaming data to consuming applications.</span></span> <span data-ttu-id="bd1fd-152">由组织许可和部署的任何其他启用了安全 API 的产品都将通过此相同的 Azure Monitor 配置自动流式处理安全警报。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-152">Any additional security API-enabled products licensed and deployed by your organization will automatically stream security alerts through this same Azure Monitor configuration.</span></span> <span data-ttu-id="bd1fd-153">无需在组织中进行进一步集成。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-153">No further integration work is needed from the organization.</span></span>

<span data-ttu-id="bd1fd-154">安全警报是具有很多特权的数据，通常只能由组织内的安全响应人员和全局管理员查看。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-154">Security alerts are highly privileged data typically viewable only by security response personnel and global administrators within an organization.</span></span> <span data-ttu-id="bd1fd-155">为此，在 SIEM 系统中配置租户安全警报集成所需的步骤将需要使用 Azure AD 全局管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-155">For this reason, the steps required to configure the integration of a tenant’s security alerts with SIEM systems require an Azure AD Global Administrator account.</span></span> <span data-ttu-id="bd1fd-156">此帐户在设置过程中只需使用一次，用以请求将组织的安全警报发送到 Azure Monitor。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-156">This account is only needed one time, during setup, to request your organization’s security alerts be sent to Azure Monitor.</span></span>

> <span data-ttu-id="bd1fd-157">**注意：**目前，Azure Monitor 诊断设置边栏选项卡不允许配置租户级资源。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-157">**Note:** At this time, the Azure Monitor Diagnostic settings blade does not allow configuration of tenant-level resources.</span></span> <span data-ttu-id="bd1fd-158">因为安全 API 警报是租户级资源，所以必须使用 Azure 资源管理器 API 为组织的安全警报配置 Azure Monitor。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-158">Because  security API alerts is a tenant-level resource, you have to use the Azure Resource Manager API to configure Azure Monitor for your organization’s security alerts.</span></span>


1. <span data-ttu-id="bd1fd-159">若要使用 Azure 资源管理器 API 配置 Azure Monitor，请获取 [ARMClient](https://github.com/projectkudu/ARMClient) 工具。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-159">To configure Azure Monitor using the Azure Resource Manager API, obtain the [ARMClient](https://github.com/projectkudu/ARMClient) tool.</span></span> <span data-ttu-id="bd1fd-160">此工具将用于将 REST API 调用从命令行发送到 Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-160">This tool will be used to send REST API calls to the Azure portal from a command line.</span></span>

2. <span data-ttu-id="bd1fd-161">准备诊断设置请求 JSON 文件，如下所示：</span><span class="sxs-lookup"><span data-stu-id="bd1fd-161">Prepare a diagnostic setting request JSON file like the following:</span></span>

    ``` json
    {
      "location": "",
      "properties": {
        "name": "securityApiAlerts",
        "serviceBusRuleId": "/subscriptions/SUBSCRIPTION_ID/resourceGroups/RESOURCE_GROUP/providers/Microsoft.EventHub/namespaces/EVENT_HUB_NAMESPACE/authorizationrules/RootManageSharedAccessKey",
        "logs": [
          {
            "category": "Alert",
            "enabled": true,
            "retentionPolicy": {
              "enabled": true,
              "days": 7
            }
          }
        ]
      }
    }
    ```

    <span data-ttu-id="bd1fd-162">将 JSON 文件中的值替换为以下值：</span><span class="sxs-lookup"><span data-stu-id="bd1fd-162">Replace the values in the JSON file as follows:</span></span>

     <span data-ttu-id="bd1fd-163">**SUBSCRIPTION_ID** 是托管资源组和事件中心命名空间的 Azure 订阅的订阅 ID，你将在此处发送组织的安全警报。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-163">**SUBSCRIPTION_ID** is the Subscription ID of the Azure subscription hosting the resource group and event hub namespace where you will be sending security alerts from your organization.</span></span>
     
     <span data-ttu-id="bd1fd-164">**RESOURCE_GROUP** 是包含事件中心命名空间的资源组，你将在此处发送组织的安全警报。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-164">**RESOURCE_GROUP** is the resource group containing the event hub namespace where you will be sending security alerts from your organization.</span></span>
     
     <span data-ttu-id="bd1fd-165">**EVENT_HUB_NAMESPACE** 是事件中心命名空间，你将在此处发送组织的安全警报。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-165">**EVENT_HUB_NAMESPACE** is the event hub namespace where you will be sending security alerts from your organization.</span></span>
     
     <span data-ttu-id="bd1fd-166">**“天”：**7 是你想要在事件中心保留消息的天数。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-166">**“days”:** 7 is the number of days you want to retain messages in your event hub.</span></span>

3. <span data-ttu-id="bd1fd-167">以 JSON 格式将文件另存到你将从中调用 ARMClient.exe 的目录。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-167">Save the file as JSON to the directory where you will invoke ARMClient.exe.</span></span> <span data-ttu-id="bd1fd-168">例如，将文件命名为 **AzMonConfig.json**。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-168">For example, name the file **AzMonConfig.json.**</span></span>

4. <span data-ttu-id="bd1fd-169">运行以下命令以登录到 ARMClient 工具。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-169">Run the following command to sigh in to the ARMClient tool.</span></span> <span data-ttu-id="bd1fd-170">你需要使用全局管理员帐户凭据。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-170">You will need to be using Global Administrator account credentials.</span></span>

    ``` shell
    ARMClient.exe login
    ```

5. <span data-ttu-id="bd1fd-171">运行以下命令以将 Azure Monitor 配置为向事件中心命名空间发送安全警报。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-171">Run the following command to configure Azure Monitor to send security alerts to your event hub namespace.</span></span> <span data-ttu-id="bd1fd-172">这将自动预配命名空间内的事件中心，并启动流入事件中心的安全警报的流。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-172">This will automatically provision an event hub within the namespace and start the flow of security alerts into the event hub.</span></span> <span data-ttu-id="bd1fd-173">确保设置名称（在此示例中是 **securityApiAlerts**）匹配在 JSON 文件中为“名称”**** 字段指定的设置名称。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-173">Ensure that the setting name (in this example, **securityApiAlerts**) matches the setting name you specified in the JSON file for the **name** field.</span></span>

    ``` shell
    ARMClient.exe put https://management.azure.com/providers/Microsoft.SecurityGraph/diagnosticSettings/securityApiAlerts?api-version=2017-04-01-preview  @".\AzMonConfig.json"
    ```

6. <span data-ttu-id="bd1fd-174">若要验证是否正确应用了设置，运行此命令并验证输出匹配 JSON 文件设置。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-174">To verify the settings were applied correctly, run this command and verify that the output matches your JSON file settings.</span></span>

    ``` shell
    ARMClient.exe get https://management.azure.com/providers/Microsoft.SecurityGraph/diagnosticSettings/securityApiAlerts?api-version=2017-04-01-preview
    ```
7. <span data-ttu-id="bd1fd-175">退出 ARMClient 工具。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-175">Exit the ARMClient tool.</span></span> <span data-ttu-id="bd1fd-176">现在，你已完成将租户安全警报发送到事件中心的 Azure Monitor 的配置。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-176">You have now completed the configuration of Azure Monitor to send security alerts from your tenant to event hub.</span></span>

## <a name="step-3-download-and-install-the-azure-monitor-add-on-for-splunk-which-will-allow-splunk-to-consume-security-alerts"></a><span data-ttu-id="bd1fd-177">步骤 3：下载和安装 Splunk 的 Azure Monitor 加载项，以允许 Splunk 使用安全警报</span><span class="sxs-lookup"><span data-stu-id="bd1fd-177">Step 3: Download and install the Azure Monitor Add-on for Splunk which will allow Splunk to consume security alerts</span></span>

1. <span data-ttu-id="bd1fd-178">下载 **Splunk Enterprise** 或使用现有 Splunk Enterprise 安装。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-178">Download **Splunk Enterprise** or use an existing Splunk Enterprise installation.</span></span>
2. <span data-ttu-id="bd1fd-179">下载并安装 [Splunk 的 Azure Monitor 加载项](https://github.com/Microsoft/AzureMonitorAddonForSplunk)。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-179">Download and install the [Azure Monitor Add-on for Splunk](https://github.com/Microsoft/AzureMonitorAddonForSplunk).</span></span> <span data-ttu-id="bd1fd-180">有关详细的安装说明，请参阅[安装](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Installation)。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-180">For detailed installation instructions, see [Installation](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Installation).</span></span>
3. <span data-ttu-id="bd1fd-181">还需要额外的一步，因为 Splunk 的 Azure Monitor 加载项是在 Azure Monitor 集成中有可用安全 API 警报前创建的。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-181">One additional step is necessary because the Azure Monitor Add-on for Splunk was created before security API alerts were available in Azure Monitor integration.</span></span> <span data-ttu-id="bd1fd-182">需要对这两个 Splunk 配置文件进行更改，以能够让 Splunk 理解 Azure Monitor 的安全 API 所使用的新日志类别，以及为组织的安全警报所配置的事件中心名称。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-182">Two Splunk configuration files need to be changed to allow Splunk to understand the new log category used by the security API for Azure Monitor, and the name of the event hub that you configured for your organization’s security alerts.</span></span>

    <span data-ttu-id="bd1fd-183">a.</span><span class="sxs-lookup"><span data-stu-id="bd1fd-183">a.</span></span>  <span data-ttu-id="bd1fd-184">从 Splunk 安装目录中的路径 **\etc\apps\TA-Azure_Monitor\bin\app** 中打开文件 **logCategories.json**。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-184">Open the file **logCategories.json** from the path                 **\etc\apps\TA-Azure_Monitor\bin\app** within your Splunk installation directory.</span></span>
   <span data-ttu-id="bd1fd-185">将以下行追加到标准日志类别的列表：</span><span class="sxs-lookup"><span data-stu-id="bd1fd-185">Append the following line to the list of standard log categories:</span></span>  
    `“MICROSOFT.SECURITYGRAPH/ALERT”: “_json”`  
    <span data-ttu-id="bd1fd-186">这将向 Splunk 的 Azure Monitor 加载项说明日志类型将被视为 JSON。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-186">This tells the Azure Monitor Addon for Splunk the log type is to be treated as JSON.</span></span>

    <span data-ttu-id="bd1fd-187">b.</span><span class="sxs-lookup"><span data-stu-id="bd1fd-187">b.</span></span> <span data-ttu-id="bd1fd-188">从 Splunk 安装目录中的路径 **\etc\apps\TA-Azure_Monitor\bin\app** 中打开文件 **hubs.json**。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-188">Open the file **hubs.json** from the path **\etc\apps\TA-Azure_Monitor\bin\app** within your Splunk installation directory.</span></span>  
    <span data-ttu-id="bd1fd-189">将以下行追加到标准事件中心的列表：</span><span class="sxs-lookup"><span data-stu-id="bd1fd-189">Append the following line to the list of standard event hubs:</span></span>  
    `“insights-logs-alert”: “tenantId”`  
    <span data-ttu-id="bd1fd-190">这将向 Splunk 的 Azure Monitor 加载项说明事件中心的名称，并指示资源 ID 为 Azure AD 租户 ID，因为这些安全警报是租户级资源。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-190">This tells the Azure Monitor Add-on for Splunk the name of the event hub and indicates that the resource ID is the Azure AD tenant ID because these security alerts are a tenant-level resource.</span></span> <span data-ttu-id="bd1fd-191">如果在之前的预配过程中为事件中心选择了自定义名称，请确保在此处更改事件中心名称（见解日志警报）。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-191">Be sure to change the event hub name (insights-logs-alert) here if you chose a custom name for your event hub during provisioning earlier.</span></span>

4. <span data-ttu-id="bd1fd-192">如加载项安装说明中所述，需要在 Splunk Web 中的“管理应用”页面上通过执行禁用/启用循环，才可使加载项正常工作。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-192">As indicated in the Add-on installation instructions, the add-on will work by doing a disable/enable cycle on the Manage Apps page in Splunk Web.</span></span> <span data-ttu-id="bd1fd-193">或者，可以重启 Splunk。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-193">Or, you can restart Splunk.</span></span>

## <a name="step-4-register-an-application-with-your-tenant-azure-active-directory-which-splunk-will-use-to-read-from-the-event-hub"></a><span data-ttu-id="bd1fd-194">步骤 4：使用租户 Azure Active Directory 注册一个供 Splunk 从事件中心进行读取的应用程序</span><span class="sxs-lookup"><span data-stu-id="bd1fd-194">Step 4: Register an application with your tenant Azure Active Directory which Splunk will use to read from the event hub</span></span>

<span data-ttu-id="bd1fd-195">Splunk 需要组织的 Azure Active Directory 中的应用程序注册，以获取从事件中心读取安全警报所需的权限和密码。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-195">Splunk needs an application registration in your organization’s Azure Active Directory to obtain the permissions and secrets it needs to read the security alerts from the event hub.</span></span> <span data-ttu-id="bd1fd-196">域中的任何标准用户帐户都可以注册应用。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-196">Any standard user account in the domain can register an app.</span></span> 

1. <span data-ttu-id="bd1fd-197">在 Azure 门户中，转到“应用注册”****，然后选择“新应用程序注册”****。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-197">In the Azure portal, go to **App Registrations** and select **New application registration**.</span></span>

    ![应用注册图像](../concepts/images/app-registration.png)

2. <span data-ttu-id="bd1fd-199">为应用程序选择一个名称，为类型选择 **Web 应用/API**，为登录 URL 选择 **`http://localhost`**。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-199">Select a name for your application, choose **Web app / API** for the type, and **`http://localhost`** for the sign-on URL.</span></span> <span data-ttu-id="bd1fd-200">然后选择“创建”****。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-200">Then select **Create**.</span></span>

    ![Web API 配置](../concepts/images/app-web-config.png)

3. <span data-ttu-id="bd1fd-202">应用程序创建后，复制“应用程序 ID”**** 并将其保存，以供在以后配置 Splunk 数据输入时使用。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-202">After the application is created, copy the **Application ID** and save for later use configuring the Splunk data inputs.</span></span> <span data-ttu-id="bd1fd-203">然后，转到应用程序设置并选择“密钥”****。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-203">Then go to the application settings and choose **Keys**.</span></span>

    ![Web 应用 ID](../concepts/images/app-id.png)

    <span data-ttu-id="bd1fd-205">这将允许你生成新密钥，称为“应用程序密码”。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-205">This will allow you to generate a new key, known as an Application Secret.</span></span> <span data-ttu-id="bd1fd-206">新密钥生成后，复制“应用程序密码”**** 并将其保存，以供在以后配置 Splunk 数据输入时使用。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-206">After it's generated, copy the **Application Secret** and save for later use configuring the Splunk data inputs.</span></span>

4. <span data-ttu-id="bd1fd-207">在包含组织安全警报的事件中心的 Azure 订阅中授予应用程序****“读取器”角色。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-207">Grant the application the role of **Reader** in the Azure subscription containing the event hub with your organization’s security alerts.</span></span>

    ![添加 Azure 子类](../concepts/images/add-azure-sub.png)

    <span data-ttu-id="bd1fd-209">选择你的订阅，然后选择“访问控制 (IAM)”****。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-209">Select your subscription, choose **Access control (IAM)**.</span></span> <span data-ttu-id="bd1fd-210">选择“添加”**** 以添加权限。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-210">Select **Add** to add permissions.</span></span> <span data-ttu-id="bd1fd-211">选择应用程序并为其选择“读取器”**** 的“角色”****。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-211">Select your application and choose the **Role** of **Reader** for your application.</span></span>

    ![添加读取器权限](../concepts/images/add-reader-perms.png)

    <span data-ttu-id="bd1fd-213">选择“保存”****，以将授予应用程序的权限添加到订阅。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-213">Select **Save** to add the permissions granted to your application to the subscription.</span></span>

## <a name="step-5-create-an-azure-key-vault-to-store-the-access-key-for-the-event-hub"></a><span data-ttu-id="bd1fd-214">步骤 5：创建 Azure Key Vault 以存储事件中心的访问密钥</span><span class="sxs-lookup"><span data-stu-id="bd1fd-214">Step 5: Create an Azure Key vault to store the access key for the event hub</span></span>

<span data-ttu-id="bd1fd-215">Azure Key Vault 用于存储应用程序在运行时所使用的标识、密码和证书等机密。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-215">Azure key vaults are used to store secrets such as identities, passwords, and certificates for use at runtime by applications.</span></span> <span data-ttu-id="bd1fd-216">在此步骤中，你将创建一个 Azure Key Vault，以存储 Splunk 从包含组织安全警报的 Azure 事件中心连接和读取所需的密码。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-216">In this step you will create an Azure key vault to store the secrets needed for Splunk to connect and read from the Azure event hubs containing your organization’s security alerts.</span></span>

1. <span data-ttu-id="bd1fd-217">在 Azure 门户中，转到“密钥保管库”**** 并选择“添加”****。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-217">In the Azure portal, go to **Key vaults** and select **Add**.</span></span>

    ![添加密钥保管库](../concepts/images/add-key-vaults.png)

2. <span data-ttu-id="bd1fd-219">创建新密钥保管库后，选择“访问策略”****，为刚在步骤 4 中注册的应用程序添加新访问策略。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-219">When creating the new key vault, select **Access policies** to add a new access policy for the application you just registered in Step 4.</span></span> <span data-ttu-id="bd1fd-220">向应用程序授予“获取”**** 密码权限。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-220">Grant the **Get** secret permissions to your application.</span></span> <span data-ttu-id="bd1fd-221">这将允许 Splunk（充当注册的应用程序）访问存储在此 Azure Key Vault 中的密钥（密码）。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-221">This will allow Splunk, acting as the registered application, to access the keys (secrets) stored in this Azure key vault.</span></span>

    ![添加访问策略](../concepts/images/add-access-policies.png)

    <span data-ttu-id="bd1fd-223">选择“创建”****，以完成新 Azure Key Vault 的创建过程。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-223">Select **Create** to complete the creation of your new Azure key vault.</span></span>

3. <span data-ttu-id="bd1fd-224">在密钥保管库中生成新密码，以将访问密钥存储到事件中心命名空间。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-224">Generate a new secret in your key vault to store the access key to your event hub namespace.</span></span> <span data-ttu-id="bd1fd-225">首先，将访问密钥捕捉到事件中心命名空间，方法是打开事件中心命名空间并选择“共享的访问策略”****。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-225">First, grab the access key to your event hub namespace by opening your event hub namespace and selecting **Shared access policies**.</span></span> <span data-ttu-id="bd1fd-226">从列表中选择 **RootManageSharedAccessKey** 策略并从中复制“主键”****。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-226">Select the **RootManageSharedAccessKey** policy from the list and copy the **Primary Key** from the list.</span></span>

    ![添加共享的访问策略](../concepts/images/get-shared-policies.png)

4. <span data-ttu-id="bd1fd-228">打开密钥保管库并选择“密码”****。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-228">Open your key vault and select **Secrets**.</span></span> <span data-ttu-id="bd1fd-229">选择“生成/导入”****，以将新密码添加到密钥保管库。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-229">Choose **Generate/Import** to add a new secret to the key vault.</span></span> <span data-ttu-id="bd1fd-230">粘贴事件中心命名空间 **RootManageSharedAccessKey** 中的“主键”****。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-230">Paste in the **Primary key** from the event hub namespace **RootManageSharedAccessKey**.</span></span>

    ![生成新密码](../concepts/images/generate-new-secret.png)

5. <span data-ttu-id="bd1fd-232">创建后，选择该密码并复制密码的“机密版本”****。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-232">After it's created, select the secret and copy the **Secret Version** of the secret.</span></span> <span data-ttu-id="bd1fd-233">稍后将在步骤 6 中使用它来配置 Splunk 数据输入。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-233">This will be used later in Step 6 to configure Splunk data inputs.</span></span>

    ![机密版本](../concepts/images/secret-version.png)

## <a name="step-6-configure-the-splunk-data-inputs-to-consume-security-alerts-stored-in-the-event-hub"></a><span data-ttu-id="bd1fd-235">步骤 6：配置 Splunk 数据输入以使用存储在事件中心的安全警报</span><span class="sxs-lookup"><span data-stu-id="bd1fd-235">Step 6: Configure the Splunk data inputs to consume security alerts stored in the event hub</span></span>

<span data-ttu-id="bd1fd-236">完成设置过程的最后一步是配置 Splunk 数据输入，以利用事件中心、应用程序和在上一步骤中创建的密码。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-236">The last step to complete the setup process is to configure Splunk data inputs to utilize the event hub, application, and secrets you created in previous steps.</span></span>

1. <span data-ttu-id="bd1fd-237">按照[配置 Splunk](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Configuration-of-Splunk) 主题中的说明进行操作，打开和配置 Azure Monitor 加载项的 Splunk 数据输入。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-237">Follow the instructions in the [Configuration of Splunk](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Configuration-of-Splunk) topic to open and configure Splunk data inputs for the Azure Monitor Add-on.</span></span> <span data-ttu-id="bd1fd-238">转到“设置”**** 和“数据输入”****。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-238">Go to **Settings** and **Data Inputs**.</span></span> <span data-ttu-id="bd1fd-239">选择“Azure Monitor 诊断日志”****。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-239">Choose **Azure Monitor Diagnostic Logs**.</span></span>
2. <span data-ttu-id="bd1fd-240">选择“新建”****，并使用在上一步骤中获取的值来输入所有必填的字段。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-240">Select **New** and input all the required fields using the values obtained in the previous steps.</span></span> <span data-ttu-id="bd1fd-241">下图显示使用本文前面示例中值的所有必填的字段。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-241">The following image shows all the required fields using the values from the previous examples in this article.</span></span>

    ![Azure Monitor 字段](../concepts/images/azure-monitor-fields.png)

3. <span data-ttu-id="bd1fd-243">选择“下一步”****，开始搜索从 Azure Monitor 中引入的组织安全警报。</span><span class="sxs-lookup"><span data-stu-id="bd1fd-243">Select **Next** and begin searching your organization’s security alerts ingested from Azure Monitor.</span></span>
