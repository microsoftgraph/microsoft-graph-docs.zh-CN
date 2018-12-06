---
title: 与 IBM QRadar SIEM 使用 Azure 监视器集成 Microsoft Graph 安全 API 通知
description: Microsoft Graph 安全提供程序可以通过单个的 REST 终结点。 此终结点可配置为支持连接到多个 SIEM 产品连接器的 Azure 监视器。 步骤 1 和 2 的本文中的说明引用所有 Azure 监视器连接器的支持通过事件集线器消耗。 本文介绍 QRadar SIEM 连接器的端到端集成。
ms.openlocfilehash: 107435c463116c002c86955559209d2dffd4d688
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091813"
---
# <a name="integrate-microsoft-graph-security-api-alerts-with-ibm-qradar-siem-using-azure-monitor"></a><span data-ttu-id="ad789-106">与 IBM QRadar SIEM 使用 Azure 监视器集成 Microsoft Graph 安全 API 通知</span><span class="sxs-lookup"><span data-stu-id="ad789-106">Integrate Microsoft Graph Security API alerts with IBM QRadar SIEM using Azure Monitor</span></span>

<span data-ttu-id="ad789-107">Microsoft Graph 安全提供程序可以通过单个的 REST 终结点。</span><span class="sxs-lookup"><span data-stu-id="ad789-107">The Microsoft Graph Security providers can be managed through a single REST endpoint.</span></span> <span data-ttu-id="ad789-108">到[Azure 监视器](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/)，支持连接到多个 SIEM 产品的连接器，可以配置此终结点。</span><span class="sxs-lookup"><span data-stu-id="ad789-108">This endpoint can be configured to [Azure Monitor](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/), which supports connectors to several SIEM products.</span></span> <span data-ttu-id="ad789-109">步骤 1 和 2 的本文中的说明引用所有 Azure 监视器连接器的支持通过事件集线器消耗。</span><span class="sxs-lookup"><span data-stu-id="ad789-109">The instructions in Steps 1 and 2 of this article refer to all Azure Monitor connectors that support consumption via event hubs.</span></span> <span data-ttu-id="ad789-110">本文介绍[QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem) SIEM 连接器的端到端集成。</span><span class="sxs-lookup"><span data-stu-id="ad789-110">This article describes the end-to-end integration of the [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem) SIEM connector.</span></span>

<span data-ttu-id="ad789-111">此集成过程包含下列步骤：</span><span class="sxs-lookup"><span data-stu-id="ad789-111">The integration process involves the following steps:</span></span>

1. <span data-ttu-id="ad789-112">[Azure 事件集线器接收租户的安全警告设置](#step-1-set-up-an-event-hubs-namespace-in-azure-to-receive-security-alerts-for-your-tenant)。</span><span class="sxs-lookup"><span data-stu-id="ad789-112">[Set up Azure event hub to receive security alerts for your tenant](#step-1-set-up-an-event-hubs-namespace-in-azure-to-receive-security-alerts-for-your-tenant).</span></span>
2. <span data-ttu-id="ad789-113">[配置 Azure 监视器发送从到事件集线器租户的安全警告](#step-2-configure-azure-monitor-to-send-security-alerts-from-your-tenant-to-the-event-hub)。</span><span class="sxs-lookup"><span data-stu-id="ad789-113">[Configure Azure Monitor to send security alerts from your tenant to the event hub](#step-2-configure-azure-monitor-to-send-security-alerts-from-your-tenant-to-the-event-hub).</span></span>
3. <span data-ttu-id="ad789-114">[下载并安装 QRadar 以使用安全警告](#step-3-download-and-install-the-qradar-to-consume-security-alerts)。</span><span class="sxs-lookup"><span data-stu-id="ad789-114">[Download and install the QRadar to consume security alerts](#step-3-download-and-install-the-qradar-to-consume-security-alerts).</span></span>

<span data-ttu-id="ad789-115">完成这些步骤后，您 IBM QRadar 将使用安全警报所有 Microsoft Graph 集成安全产品为其授权您的租户。</span><span class="sxs-lookup"><span data-stu-id="ad789-115">After you complete these steps, your IBM QRadar will consume security alerts from all the Microsoft Graph integrated security products for which your tenant is licensed.</span></span> <span data-ttu-id="ad789-116">许可的任何新安全产品也将通过此连接发送警报（在同一架构且无需进一步集成）。</span><span class="sxs-lookup"><span data-stu-id="ad789-116">Any new security products that you license will also send alerts through this connection, in the same schema with no further integration work needed.</span></span>

## <a name="step-1-set-up-an-event-hubs-namespace-in-azure-to-receive-security-alerts-for-your-tenant"></a><span data-ttu-id="ad789-117">步骤 1：在 Azure 中设置事件中心命名空间，以接收租户的安全警报。</span><span class="sxs-lookup"><span data-stu-id="ad789-117">Step 1: Set up an Event Hubs namespace in Azure to receive security alerts for your tenant</span></span>

<span data-ttu-id="ad789-118">若要开始，您需要创建[Microsoft Azure 事件集线器](https://docs.microsoft.com/en-us/azure/event-hubs/)命名空间和事件集线器。</span><span class="sxs-lookup"><span data-stu-id="ad789-118">To begin, you need to create a [Microsoft Azure Event Hubs](https://docs.microsoft.com/en-us/azure/event-hubs/) namespace and event hub.</span></span> <span data-ttu-id="ad789-119">此命名空间和事件中心是所有组织的安全警报的目标。</span><span class="sxs-lookup"><span data-stu-id="ad789-119">This namespace and event hub is the destination for all your organization’s security alerts.</span></span> <span data-ttu-id="ad789-120">事件中心命名空间是共享同一访问策略的事件中心的逻辑分组。</span><span class="sxs-lookup"><span data-stu-id="ad789-120">An Event Hubs namespace is a logical grouping of event hubs that share the same access policy.</span></span> <span data-ttu-id="ad789-121">请注意有关你创建的事件中心命名空间和事件中心的一些详细信息：</span><span class="sxs-lookup"><span data-stu-id="ad789-121">Note a few details about the Event Hubs namespace and event hubs that you create:</span></span>

- <span data-ttu-id="ad789-122">我们建议使用标准事件中心命名空间（尤其是当你通过这些相同的事件中心发送其他 Azure 监控数据时）。</span><span class="sxs-lookup"><span data-stu-id="ad789-122">We recommend using a Standard Event Hubs namespace, particularly if you are sending other Azure monitoring data through these same event hubs.</span></span>
- <span data-ttu-id="ad789-123">通常情况下，一个吞吐量单位就已足够。</span><span class="sxs-lookup"><span data-stu-id="ad789-123">Typically, only one throughput unit is necessary.</span></span> <span data-ttu-id="ad789-124">如果随着使用情况的增加而需要扩展吞吐量，则可在以后随时手动增加命名空间的吞吐量单位数或启用自动膨胀。</span><span class="sxs-lookup"><span data-stu-id="ad789-124">If you need to scale up as your usage increases, you can always manually increase the number of throughput units for the namespace later or enable auto inflation.</span></span>
- <span data-ttu-id="ad789-125">吞吐量单位数可让你增加事件中心的吞吐量比例。</span><span class="sxs-lookup"><span data-stu-id="ad789-125">The number of throughput units allows you to increase throughput scale for your event hubs.</span></span> <span data-ttu-id="ad789-126">分区数可让你跨多个使用者并行使用。</span><span class="sxs-lookup"><span data-stu-id="ad789-126">The number of partitions allows you to parallelize consumption across many consumers.</span></span> <span data-ttu-id="ad789-127">单个分区可执行最多 20MBps，或大约每秒 20,000 封邮件。</span><span class="sxs-lookup"><span data-stu-id="ad789-127">A single partition can do up to 20MBps, or approximately 20,000 messages per second.</span></span> <span data-ttu-id="ad789-128">分区是否支持从多个分区使用要取决于使用数据的工具。</span><span class="sxs-lookup"><span data-stu-id="ad789-128">Depending on the tool consuming the data, it may or may not support consuming from multiple partitions.</span></span> <span data-ttu-id="ad789-129">如果不确定要设置的分区数，我们建议从设置四个分区开始。</span><span class="sxs-lookup"><span data-stu-id="ad789-129">If you're not sure about the number of partitions to set, we recommend starting with four partitions.</span></span>
- <span data-ttu-id="ad789-130">我们建议将事件中心的消息保留设置为 7 天。</span><span class="sxs-lookup"><span data-stu-id="ad789-130">We recommend that you set message retention on your event hub to 7 days.</span></span> <span data-ttu-id="ad789-131">在你使用的工具停用多天时，该设置可确保工具能够从上次停用的位置继续工作（针对最多 7 天的事件）。</span><span class="sxs-lookup"><span data-stu-id="ad789-131">If your consuming tool goes down for more than a day, this ensures that the tool can pick up where it left off (for events up to 7 days old).</span></span>
- <span data-ttu-id="ad789-132">我们建议为事件中心使用默认的使用者组。</span><span class="sxs-lookup"><span data-stu-id="ad789-132">We recommend using the default consumer group for your event hub.</span></span> <span data-ttu-id="ad789-133">无需创建其他使用者组或使用单独的使用者组，除非你计划用两个不同的工具使用来自同一事件中心的同一数据。</span><span class="sxs-lookup"><span data-stu-id="ad789-133">You don't need to create other consumer groups or use a separate consumer group unless you plan to have two different tools consume the same data from the same event hub.</span></span>
- <span data-ttu-id="ad789-134">通常情况下，对于使用事件中心数据的计算机，必须打开端口 5671 和 5672。</span><span class="sxs-lookup"><span data-stu-id="ad789-134">Typically, port 5671 and 5672 must be opened on the machine consuming data from the event hub.</span></span>

<span data-ttu-id="ad789-135">另请参阅 [Azure 事件中心常见问题解答](https://docs.microsoft.com/en-us/azure/event-hubs/event-hubs-faq)。</span><span class="sxs-lookup"><span data-stu-id="ad789-135">Also see the [Azure Event Hubs FAQ](https://docs.microsoft.com/en-us/azure/event-hubs/event-hubs-faq).</span></span>

1. <span data-ttu-id="ad789-136">登录到 [Azure 门户](https://portal.azure.com/)，并选择屏幕左上角的“创建资源”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="ad789-136">Log on to the [Azure portal](https://portal.azure.com/) and choose **Create a resource** at the top left of the screen.</span></span>

    ![创建资源图像](images/create-resource.png)

2. <span data-ttu-id="ad789-138">选择“物联网”\*\*\*\*，并选择“事件中心”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="ad789-138">Select **Internet of Things** and choose **Event Hubs**.</span></span>

    ![事件中心图像](images/event-hubs.png)

3. <span data-ttu-id="ad789-140">在“创建命名空间”\*\*\*\* 中，输入命名空间名称。</span><span class="sxs-lookup"><span data-stu-id="ad789-140">In **Create namespace**, enter a namespace name.</span></span> <span data-ttu-id="ad789-141">确保命名空间名称可用后，选择定价层（基本或标准）。</span><span class="sxs-lookup"><span data-stu-id="ad789-141">After making sure the namespace name is available, choose the pricing tier (Basic or Standard).</span></span> <span data-ttu-id="ad789-142">此外，选择 Azure 订阅、资源组以及创建资源的位置。</span><span class="sxs-lookup"><span data-stu-id="ad789-142">Also, choose an Azure subscription, resource group, and location in which to create the resource.</span></span> <span data-ttu-id="ad789-143">选择“创建”\*\*\*\* 以创建命名空间。</span><span class="sxs-lookup"><span data-stu-id="ad789-143">Choose **Create** to create the namespace.</span></span> <span data-ttu-id="ad789-144">你可能需要等待几分钟的时间，以使系统完全预配资源。</span><span class="sxs-lookup"><span data-stu-id="ad789-144">You might have to wait a few minutes for the system to fully provision the resources.</span></span>

    ![创建命名空间图像](images/create-namespace.png)

## <a name="step-2-configure-azure-monitor-to-send-security-alerts-from-your-tenant-to-the-event-hub"></a><span data-ttu-id="ad789-146">步骤 2：配置 Azure Monitor 以将租户的安全警报发送至事件中心</span><span class="sxs-lookup"><span data-stu-id="ad789-146">Step 2: Configure Azure Monitor to send security alerts from your tenant to the event hub</span></span>

<span data-ttu-id="ad789-147">通过 Azure Monitor 为整个 Azure Active Directory (Azure AD) 租户启用组织安全警报的流式处理操作已执行一次。</span><span class="sxs-lookup"><span data-stu-id="ad789-147">Enabling the streaming of your organization’s security alerts through Azure Monitor is done one time for your entire Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="ad789-148">所有 Microsoft Graph 安全 API 都授权和启用的产品将开始发送到 Azure 监视器，流式传输到使用应用程序的数据的安全警告。</span><span class="sxs-lookup"><span data-stu-id="ad789-148">All Microsoft Graph Security API licensed and enabled products will begin sending security alerts to Azure Monitor, streaming data to consuming applications.</span></span> <span data-ttu-id="ad789-149">任何其他 Microsoft Graph 安全 API 启用产品授权和部署您的组织将自动 stream 通过相同的 Azure 监视器配置的安全警告。</span><span class="sxs-lookup"><span data-stu-id="ad789-149">Any additional Microsoft Graph Security API-enabled products licensed and deployed by your organization will automatically stream security alerts through this same Azure Monitor configuration.</span></span> <span data-ttu-id="ad789-150">无需在组织中进行进一步集成。</span><span class="sxs-lookup"><span data-stu-id="ad789-150">No further integration work is needed from the organization.</span></span>

<span data-ttu-id="ad789-151">安全警报是具有很多特权的数据，通常只能由组织内的安全响应人员和全局管理员查看。</span><span class="sxs-lookup"><span data-stu-id="ad789-151">Security alerts are highly privileged data typically viewable only by security response personnel and global administrators within an organization.</span></span> <span data-ttu-id="ad789-152">为此，在 SIEM 系统中配置租户安全警报集成所需的步骤将需要使用 Azure AD 全局管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="ad789-152">For this reason, the steps required to configure the integration of a tenant’s security alerts with SIEM systems require an Azure AD Global Administrator account.</span></span> <span data-ttu-id="ad789-153">此帐户在设置过程中只需使用一次，用以请求将组织的安全警报发送到 Azure Monitor。</span><span class="sxs-lookup"><span data-stu-id="ad789-153">This account is only needed one time, during setup, to request your organization’s security alerts be sent to Azure Monitor.</span></span>

> <span data-ttu-id="ad789-154">**注意：** 目前，Azure 监视器诊断设置刀片不支持配置租户级别的资源。</span><span class="sxs-lookup"><span data-stu-id="ad789-154">**Note:** Currently, the Azure Monitor Diagnostic settings blade does not support configuration of tenant-level resources.</span></span> <span data-ttu-id="ad789-155">Microsoft Graph 安全 API 通知是要求使用 Azure 资源管理器 API 配置要支持的组织的安全警告消耗的 Azure 监视器的租户级资源。</span><span class="sxs-lookup"><span data-stu-id="ad789-155">Microsoft Graph Security API alerts are a tenant-level resource, which requires using the Azure Resource Manager API to configure Azure Monitor to support consumption of your organization’s security alerts.</span></span>

1. <span data-ttu-id="ad789-156">在您 Azure 订阅中 （可以在"所有服务"下，找到），为资源提供程序注册"microsoft.insights"（Azure 监视器）。</span><span class="sxs-lookup"><span data-stu-id="ad789-156">In your Azure subscription (can be found under "All services"), register "microsoft.insights" (Azure Monitor) as a resource provider.</span></span>  
 > <span data-ttu-id="ad789-157">**注意：** 原样"Microsoft.SecurityGraph"租户级资源上面所述，并为您的 Azure 订阅中的资源提供程序注册"Microsoft.SecurityGraph"(Microsoft Graph 安全 API)。</span><span class="sxs-lookup"><span data-stu-id="ad789-157">**Note:** Do not register "Microsoft.SecurityGraph" (Microsoft Graph Security API) as a resource provider in your Azure subscription, as “Microsoft.SecurityGraph” is a tenant-level resource as explained above.</span></span> <span data-ttu-id="ad789-158">租户级配置将是下面 #6 的一部分。</span><span class="sxs-lookup"><span data-stu-id="ad789-158">Tenant level configuration will be part of #6 below.</span></span>

2. <span data-ttu-id="ad789-159">若要使用 Azure 资源管理器 API 配置 Azure Monitor，请获取 [ARMClient](https://github.com/projectkudu/ARMClient) 工具。</span><span class="sxs-lookup"><span data-stu-id="ad789-159">To configure Azure Monitor using the Azure Resource Manager API, obtain the [ARMClient](https://github.com/projectkudu/ARMClient) tool.</span></span> <span data-ttu-id="ad789-160">此工具将用于将 REST API 调用从命令行发送到 Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="ad789-160">This tool will be used to send REST API calls to the Azure portal from a command line.</span></span>

3. <span data-ttu-id="ad789-161">准备诊断设置请求 JSON 文件，如下所示：</span><span class="sxs-lookup"><span data-stu-id="ad789-161">Prepare a diagnostic setting request JSON file like the following:</span></span>

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

  <span data-ttu-id="ad789-162">将 JSON 文件中的值替换为以下值：</span><span class="sxs-lookup"><span data-stu-id="ad789-162">Replace the values in the JSON file as follows:</span></span>

  * <span data-ttu-id="ad789-163">**SUBSCRIPTION_ID** 是托管资源组和事件中心命名空间的 Azure 订阅的订阅 ID，你将在此处发送组织的安全警报。</span><span class="sxs-lookup"><span data-stu-id="ad789-163">**SUBSCRIPTION_ID** is the Subscription ID of the Azure subscription hosting the resource group and event hub namespace where you will be sending security alerts from your organization.</span></span>
  * <span data-ttu-id="ad789-164">**RESOURCE_GROUP** 是包含事件中心命名空间的资源组，你将在此处发送组织的安全警报。</span><span class="sxs-lookup"><span data-stu-id="ad789-164">**RESOURCE_GROUP** is the resource group containing the event hub namespace where you will be sending security alerts from your organization.</span></span>
  * <span data-ttu-id="ad789-165">**EVENT_HUB_NAMESPACE** 是事件中心命名空间，你将在此处发送组织的安全警报。</span><span class="sxs-lookup"><span data-stu-id="ad789-165">**EVENT_HUB_NAMESPACE** is the event hub namespace where you will be sending security alerts from your organization.</span></span>
  * <span data-ttu-id="ad789-166">**"天":** 是您想要保留事件中心中的邮件的天数。</span><span class="sxs-lookup"><span data-stu-id="ad789-166">**“days”:** is the number of days you want to retain messages in your event hub.</span></span>
  
&nbsp;

4. <span data-ttu-id="ad789-167">以 JSON 格式将文件另存到你将从中调用 ARMClient.exe 的目录。</span><span class="sxs-lookup"><span data-stu-id="ad789-167">Save the file as JSON to the directory where you will invoke ARMClient.exe.</span></span> <span data-ttu-id="ad789-168">例如，将文件命名为 **AzMonConfig.json**。</span><span class="sxs-lookup"><span data-stu-id="ad789-168">For example, name the file **AzMonConfig.json.**</span></span>

5. <span data-ttu-id="ad789-169">运行以下命令以登录到 ARMClient 工具。</span><span class="sxs-lookup"><span data-stu-id="ad789-169">Run the following command to sigh in to the ARMClient tool.</span></span> <span data-ttu-id="ad789-170">你需要使用全局管理员帐户凭据。</span><span class="sxs-lookup"><span data-stu-id="ad789-170">You will need to be using Global Administrator account credentials.</span></span>

    ``` shell
    ARMClient.exe login
    ```

6. <span data-ttu-id="ad789-171">运行以下命令以将 Azure Monitor 配置为向事件中心命名空间发送安全警报。</span><span class="sxs-lookup"><span data-stu-id="ad789-171">Run the following command to configure Azure Monitor to send security alerts to your event hub namespace.</span></span> <span data-ttu-id="ad789-172">这将自动预配命名空间内的事件中心，并启动流入事件中心的安全警报的流。</span><span class="sxs-lookup"><span data-stu-id="ad789-172">This will automatically provision an event hub within the namespace and start the flow of security alerts into the event hub.</span></span> <span data-ttu-id="ad789-173">确保设置名称（在此示例中是 **securityApiAlerts**）匹配在 JSON 文件中为“名称”\*\*\*\* 字段指定的设置名称。</span><span class="sxs-lookup"><span data-stu-id="ad789-173">Ensure that the setting name (in this example, **securityApiAlerts**) matches the setting name you specified in the JSON file for the **name** field.</span></span>

    ``` shell
    ARMClient.exe put https://management.azure.com/providers/Microsoft.SecurityGraph/diagnosticSettings/securityApiAlerts?api-version=2017-04-01-preview  @".\AzMonConfig.json"
    ```

7. <span data-ttu-id="ad789-174">若要验证是否正确应用了设置，运行此命令并验证输出匹配 JSON 文件设置。</span><span class="sxs-lookup"><span data-stu-id="ad789-174">To verify the settings were applied correctly, run this command and verify that the output matches your JSON file settings.</span></span>

    ``` shell
    ARMClient.exe get https://management.azure.com/providers/Microsoft.SecurityGraph/diagnosticSettings/securityApiAlerts?api-version=2017-04-01-preview
    ```

8. <span data-ttu-id="ad789-175">退出 ARMClient 工具。</span><span class="sxs-lookup"><span data-stu-id="ad789-175">Exit the ARMClient tool.</span></span> <span data-ttu-id="ad789-176">现在，你已完成将租户安全警报发送到事件中心的 Azure Monitor 的配置。</span><span class="sxs-lookup"><span data-stu-id="ad789-176">You have now completed the configuration of Azure Monitor to send security alerts from your tenant to event hub.</span></span>

## <a name="step-3-download-and-install-the-qradar-to-consume-security-alerts"></a><span data-ttu-id="ad789-177">步骤 3： 下载并安装 QRadar 以使用安全警告</span><span class="sxs-lookup"><span data-stu-id="ad789-177">Step 3: Download and install the QRadar to consume security alerts</span></span>

1. <span data-ttu-id="ad789-178">下载并安装[IBM QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem)。</span><span class="sxs-lookup"><span data-stu-id="ad789-178">Download and install [IBM QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem).</span></span> <span data-ttu-id="ad789-179">**7.2.8 修补程序 7 或更高版本，则需要**从 Microsoft Azure 事件集线器读取事件。</span><span class="sxs-lookup"><span data-stu-id="ad789-179">**Version 7.2.8 with Patch 7 or higher is required** to read events from a Microsoft Azure Event Hub.</span></span>
2. <span data-ttu-id="ad789-180">按照[配置 Microsoft Azure 事件集线器与 IBM QRadar 通信](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/t_dsm_guide_microsoft_azure_enable_event_hubs.html)配置事件集线器中的步骤。</span><span class="sxs-lookup"><span data-stu-id="ad789-180">Follow the steps in [Configuring Microsoft Azure Event Hubs to communicate with IBM QRadar](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/t_dsm_guide_microsoft_azure_enable_event_hubs.html) to configure your event hub.</span></span>
3. <span data-ttu-id="ad789-181">最后，按照[配置 QRadar 以收集中使用的 Microsoft Azure 事件集线器协议的 Microsoft Azure 事件集线器事件](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/t_logsource_microsoft_azure_event_hubs.html)开始显示安全警报中的步骤。</span><span class="sxs-lookup"><span data-stu-id="ad789-181">Finally, follow the steps in [Configuring QRadar to collect events from Microsoft Azure Event Hubs by using the Microsoft Azure Event Hubs protocol](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/t_logsource_microsoft_azure_event_hubs.html) to begin surfacing security alerts.</span></span>
  
 > <span data-ttu-id="ad789-182">**注意：** 与 IBM QRadar Microsoft Azure 集成支持[Microsoft Azure DSM 规范](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/c_dsm_guide_microsoft_azure_DSM_specs.html)中列出的事件。</span><span class="sxs-lookup"><span data-stu-id="ad789-182">**Note:** Microsoft Azure integration with IBM QRadar supports the events listed in [Microsoft Azure DSM specifications](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/c_dsm_guide_microsoft_azure_DSM_specs.html).</span></span> <span data-ttu-id="ad789-183">我们当前正在与 IBM QRadar 添加完整 Microsoft Graph 安全 API 通知的支持。</span><span class="sxs-lookup"><span data-stu-id="ad789-183">We are currently working with IBM QRadar to add complete support for Microsoft Graph Security API alerts.</span></span> <span data-ttu-id="ad789-184">目前，您将能够接收的 Microsoft 安全图形 API 警报和查看它们在 IBM QRadar 控制台。</span><span class="sxs-lookup"><span data-stu-id="ad789-184">Currently, you will be able to receive the Microsoft Security Graph API alerts and view them in your IBM QRadar console.</span></span> <span data-ttu-id="ad789-185">您可以使用[DSM 编辑器](https://www.ibm.com/support/knowledgecenter/SS42VS_7.2.8/com.ibm.qradar.doc/c_qradar_adm_dsm_ed_overview.html)启用分析 Microsoft 安全图形 API 通知。</span><span class="sxs-lookup"><span data-stu-id="ad789-185">You can use [DSM editor](https://www.ibm.com/support/knowledgecenter/SS42VS_7.2.8/com.ibm.qradar.doc/c_qradar_adm_dsm_ed_overview.html) to enable parsing Microsoft Security Graph API alerts.</span></span>  
