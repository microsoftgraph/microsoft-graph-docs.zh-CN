---
title: 订阅使用 Microsoft Graph 更改云打印 API 的通知
description: 了解如何使用 Microsoft Graph API 更改打印作业事件的通知。
author: jahsu
localization_priority: Priority
ms.prod: cloud-printing
ms.custom: scenarios:getting-started
ms.openlocfilehash: 0d4cbaabb6fc05df3d9a58d1ced467bee0b8ef04
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515728"
---
# <a name="subscribe-to-change-notifications-from-cloud-printing-apis-using-microsoft-graph"></a><span data-ttu-id="7b50a-103">订阅使用 Microsoft Graph 更改云打印 API 的通知</span><span class="sxs-lookup"><span data-stu-id="7b50a-103">Subscribe to change notifications from cloud printing APIs using Microsoft Graph</span></span>

<span data-ttu-id="7b50a-104">通用打印可帮助客户将其打印基础结构移动到云，是提供高级打印功能的合作伙伴解决方案强大生产力的一部分。</span><span class="sxs-lookup"><span data-stu-id="7b50a-104">Universal Print helps customers move their print infrastructure to the cloud, and is part of a robust ecosystem of partner solutions that offer advanced print functionality.</span></span> <span data-ttu-id="7b50a-105">当您使用 Microsoft Graph 中的云打印 API 与通用打印集成时，这些解决方案甚至会更加强大。</span><span class="sxs-lookup"><span data-stu-id="7b50a-105">These solutions can become even more powerful when you use the cloud printing APIs in Microsoft Graph to integrate with Universal Print.</span></span>

<span data-ttu-id="7b50a-106">许多合作伙伴解决方案需要将打印作业从用户的设备发送到打印机时实时处理，这意味着当打印作业可进行处理时，需要收到通知。</span><span class="sxs-lookup"><span data-stu-id="7b50a-106">Many partner solutions need to process print jobs in real time as they're sent from users' devices to printers, which means they need to be notified when print jobs are available for processing.</span></span> <span data-ttu-id="7b50a-107">通用打印为在云中移动作业时通知打印供应商解决方案提供的连接，以及可管理打印机和打印作业的 API。</span><span class="sxs-lookup"><span data-stu-id="7b50a-107">Universal Print provides hooks for print vendor solutions to be notified as jobs move through the cloud, and APIs that enable management of printers and print jobs.</span></span>

<span data-ttu-id="7b50a-108">本文介绍如何订阅各种打印作业事件的通知。</span><span class="sxs-lookup"><span data-stu-id="7b50a-108">This article describes how to subscribe to notifications for various print job events.</span></span>


## <a name="get-started-with-change-notifications"></a><span data-ttu-id="7b50a-109">更改通知入门</span><span class="sxs-lookup"><span data-stu-id="7b50a-109">Get started with change notifications</span></span>

<span data-ttu-id="7b50a-110">必须先在 Azure [中注册应用程序，](/azure/active-directory/develop/howto-create-service-principal-portal#register-an-application-with-azure-ad-and-create-a-service-principal) Azure Active Directory （Azure AD） 租户中预配应用程序，才能利用通过 Microsoft Graph 更改通知。</span><span class="sxs-lookup"><span data-stu-id="7b50a-110">Before you can take advantage of change notifications via Microsoft Graph, you must [register your application in Azure](/azure/active-directory/develop/howto-create-service-principal-portal#register-an-application-with-azure-ad-and-create-a-service-principal) and provision your application in the customers Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="7b50a-111">确保应用程序已启用所需的权限范围，如本文稍后所述。</span><span class="sxs-lookup"><span data-stu-id="7b50a-111">Make sure that the application has the required permission scopes enabled, as described later in this article.</span></span>


### <a name="notifications-and-subscriptions"></a><span data-ttu-id="7b50a-112">通知和订阅</span><span class="sxs-lookup"><span data-stu-id="7b50a-112">Notifications and subscriptions</span></span>

<span data-ttu-id="7b50a-113">通用打印当前支持两种打印作业相关方案的通知：</span><span class="sxs-lookup"><span data-stu-id="7b50a-113">Universal Print currently supports notifications for two scenarios related to print jobs:</span></span>

* <span data-ttu-id="7b50a-114">PrintTask 被触发（作业启动）：应用程序可以在其 printTask（hook） 触发时订阅以接收通知。</span><span class="sxs-lookup"><span data-stu-id="7b50a-114">PrintTask is triggered (JobStarted): An application can subscribe to receive notifications when their printTask(hook) is triggered.</span></span>
<span data-ttu-id="7b50a-115">若要详细了解如何触发任务，请参阅扩展通用 [以支持将打印内容拉取](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-115">For details about how to trigger a task, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span> <span data-ttu-id="7b50a-116">目前，仅能为作业启动事件触发 printTask。</span><span class="sxs-lookup"><span data-stu-id="7b50a-116">Currently, a printTask can be triggered only for a JobStarted event.</span></span> <span data-ttu-id="7b50a-117">成功创建打印作业、上传有效负载并开始作业处理后，将发生作业启动事件。</span><span class="sxs-lookup"><span data-stu-id="7b50a-117">A JobStarted event is raised when a print job has been successfully created, its payload has been uploaded, and job processing has started.</span></span>  

* <span data-ttu-id="7b50a-118">作业可保存：作业启动后，第三方打印应用程序或通用打印可能会执行某些处理（例如将 XPS 有效负载转换为 PDF，用于 PDF 打印机）。</span><span class="sxs-lookup"><span data-stu-id="7b50a-118">JobFetchable: After the job has started, third-party print applications or Universal Print might do some processing (like converting XPS payload to PDF for a PDF printer).</span></span> <span data-ttu-id="7b50a-119">处理完成后，如果有效负载已准备好由打印机下载，则针对相应的打印作业将发生 JobFable 事件。</span><span class="sxs-lookup"><span data-stu-id="7b50a-119">After processing is complete and the payload is ready to be downloaded by a printer, a JobFetchable event is raised for the corresponding print job.</span></span>

>[!NOTE]
><span data-ttu-id="7b50a-120">为收听 JobFableable 事件更改通知， **printTaskDefinition** 更改通知。</span><span class="sxs-lookup"><span data-stu-id="7b50a-120">For listening to the change notifications for JobFetchable event, a **printTaskDefinition** resource is not required.</span></span>

### <a name="create-an-application-to-listen-to-notifications"></a><span data-ttu-id="7b50a-121">创建可收听通知的应用程序</span><span class="sxs-lookup"><span data-stu-id="7b50a-121">Create an application to listen to notifications</span></span>

<span data-ttu-id="7b50a-122">若要了解如何收听 Microsoft Graph 通知，请参阅 [通过 Microsoft Graph](https://docs.microsoft.com/learn/modules/msgraph-changenotifications-trackchanges/) 使用更改通知和修订 [设置用户数据更改通知 - 代码示例](/graph/webhooks#code-samples)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-122">For information about how to listen for Microsoft Graph notifications, see [Use change notifications and track changes with Microsoft Graph](https://docs.microsoft.com/learn/modules/msgraph-changenotifications-trackchanges/) and [Set up notifications for changes in user data – Code Samples](/graph/webhooks#code-samples).</span></span>


### <a name="scopes"></a><span data-ttu-id="7b50a-123">Scopes</span><span class="sxs-lookup"><span data-stu-id="7b50a-123">Scopes</span></span>

<span data-ttu-id="7b50a-124">若要订阅打印作业通知，应用程序必须具有在客户的 Azure AD 租户中批准的下列权限范围：</span><span class="sxs-lookup"><span data-stu-id="7b50a-124">To subscribe to notifications for print jobs, applications must have the following permission scopes approved in the customer’s Azure AD tenant:</span></span> 

* <span data-ttu-id="7b50a-125">对于 printTask 触发（作业启动）事件，"获取任务定义 [中列出的权限](/graph/api/printtaskdefinition-get?view=graph-rest-beta&tabs=http%22%20%5Cl%20%22permissions%22%20%5C)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-125">For printTask triggered (JobStarted) event, the permissions listed in [Get taskDefinition](/graph/api/printtaskdefinition-get?view=graph-rest-beta&tabs=http%22%20%5Cl%20%22permissions%22%20%5C).</span></span> 

* <span data-ttu-id="7b50a-126">对于 JobFable 事件，"创建订阅" [中列出的](/graph/api/subscription-post-subscriptions?view=graph-rest-beta&tabs=http)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-126">For JobFetchable event, the permissions listed in [Create subscription](/graph/api/subscription-post-subscriptions?view=graph-rest-beta&tabs=http).</span></span>

<span data-ttu-id="7b50a-127">应用程序必须 [Microsoft Graph API 请求标头中生成](/graph/auth-v2-service?context=graph%2Fapi%2Fbeta&view=graph-rest-beta) Azure AD 安全令牌。</span><span class="sxs-lookup"><span data-stu-id="7b50a-127">Applications must [generate and use the Azure AD security token](/graph/auth-v2-service?context=graph%2Fapi%2Fbeta&view=graph-rest-beta) in the Microsoft Graph API request header.</span></span> <span data-ttu-id="7b50a-128">安全令牌包含按管理员批准的客户 Azure AD 租户范围内声明声明。</span><span class="sxs-lookup"><span data-stu-id="7b50a-128">The security token contains the claims as per the scopes approved for the customer’s Azure AD tenant by its administrator.</span></span>  


## <a name="create-subscription-printtask-triggered-jobstarted-event"></a><span data-ttu-id="7b50a-129">创建订阅：printTask 触发（作业启动）事件</span><span class="sxs-lookup"><span data-stu-id="7b50a-129">Create subscription: printTask triggered (JobStarted) event</span></span> 

<span data-ttu-id="7b50a-130">某些应用程序监视传入作业的打印队列，希望在队列中具有有效作业时收到通知。</span><span class="sxs-lookup"><span data-stu-id="7b50a-130">Some applications monitor print queues for incoming jobs and want to be notified as soon as there is a valid job in the queue.</span></span> <span data-ttu-id="7b50a-131">收到通知后，他们可以收集相关的作业元数据，甚至可以在打印作业中执行修改，包括中止作业或相应地修改作业属性后将作业从当前打印队列重定向到另一个队列。</span><span class="sxs-lookup"><span data-stu-id="7b50a-131">After theyt're notified, they can collect the relevant job metadata or even perform modifications in the print job – including aborting the job or redirecting the job from the current print queue to another queue after modifying the job attributes accordingly.</span></span> 

<span data-ttu-id="7b50a-132">在创建打印任务 **-** 事件的通知之前，请确保应用程序创建了以下应用程序：</span><span class="sxs-lookup"><span data-stu-id="7b50a-132">Before creating a notification for a **printTask**-triggered event, ensure that application has created the following:</span></span> 

- <span data-ttu-id="7b50a-133">一[Azure AD](/graph/api/print-post-taskdefinitions?view=graph-rest-beta&tabs=http) printTaskDefinition 应用程序。</span><span class="sxs-lookup"><span data-stu-id="7b50a-133">A [printTaskDefinition](/graph/api/print-post-taskdefinitions?view=graph-rest-beta&tabs=http) for the customer’s Azure AD tenant.</span></span> <span data-ttu-id="7b50a-134">单个任务定义可在同一 Azure AD 租户中的一个或多个打印机关联。</span><span class="sxs-lookup"><span data-stu-id="7b50a-134">A single task definition can be associated with one or more printers within the same Azure AD tenant.</span></span> 

- <span data-ttu-id="7b50a-135">针对 [开始新打印作业时，合作伙伴希望接收其通知的每个打印机队列的](/graph/api/printer-post-tasktriggers?view=graph-rest-beta&tabs=http) "PrintTaskTri你邮件"标签。</span><span class="sxs-lookup"><span data-stu-id="7b50a-135">A [printTaskTrigger](/graph/api/printer-post-tasktriggers?view=graph-rest-beta&tabs=http) for each of the printer queues for which the partner wants to receive a notification when a new print job starts.</span></span> <span data-ttu-id="7b50a-136">**printTaskDefinition** 需要绑定到 **PrintTaskDefinition**。</span><span class="sxs-lookup"><span data-stu-id="7b50a-136">The **printTaskTrigger** needs to be bound to the **printTaskDefinition**.</span></span> 

>[!NOTE]
><span data-ttu-id="7b50a-137">一个打印机只能与一个 **printTaskTriition** 和一个 **printTaskTriition** 只能与一 **printTaskDefinition**。</span><span class="sxs-lookup"><span data-stu-id="7b50a-137">One printer can be associated with only one **printTaskTrigger** and one **printTaskTrigger** can be associated with only one **printTaskDefinition**.</span></span> <span data-ttu-id="7b50a-138">但是，一 **printTaskDefinition** 可以具有一 **一个或多个 printTaskTriitions** 与其关联。</span><span class="sxs-lookup"><span data-stu-id="7b50a-138">However, one **printTaskDefinition** can have one or more **printTaskTriggers** associated with it.</span></span> 

<span data-ttu-id="7b50a-139">使用客户的 Azure A [D 租户 **printTaskDefinition**，该应用程序可以使用 printTaskDefinition](/graph/api/subscription-post-subscriptions?view=graph-rest-beta&tabs=http)为 printTask 触发（作业启动）事件创建订阅。</span><span class="sxs-lookup"><span data-stu-id="7b50a-139">With the **printTaskDefinition** that exists for customer’s Azure AD tenant, the application can [create a subscription for a printTask triggered (JobStarted) event using the printTaskDefinition](/graph/api/subscription-post-subscriptions?view=graph-rest-beta&tabs=http).</span></span> <span data-ttu-id="7b50a-140">创建订阅时：</span><span class="sxs-lookup"><span data-stu-id="7b50a-140">While creating the subscription:</span></span>  

* <span data-ttu-id="7b50a-141">`resource` 字段需要设置为 `print/taskDefinitions/{printTaskDefinition ID}/tasks`。</span><span class="sxs-lookup"><span data-stu-id="7b50a-141">The `resource` field needs to be set as `print/taskDefinitions/{printTaskDefinition ID}/tasks`.</span></span> 
* <span data-ttu-id="7b50a-142">`changeType` 字段需要设置为 `created`。</span><span class="sxs-lookup"><span data-stu-id="7b50a-142">The `changeType` field needs to be set as `created`.</span></span> 
* <span data-ttu-id="7b50a-143">" `expirationDateTime` "字段需要小于 [最大到期日期](/graph/api/resources/subscription?view=graph-rest-beta#maximum-length-of-subscription-per-resource-type)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-143">The `expirationDateTime` field needs to be less than the [maximum expiration time](/graph/api/resources/subscription?view=graph-rest-beta#maximum-length-of-subscription-per-resource-type).</span></span> 

<span data-ttu-id="7b50a-144">如需了解更多详情，请参阅 [openTypeExtension 资源类型](/graph/api/resources/subscription?view=graph-rest-beta#properties)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-144">For more details, see [Subscription resource type properties](/graph/api/resources/subscription?view=graph-rest-beta#properties).</span></span>

<span data-ttu-id="7b50a-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7b50a-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription"
}--> 
```http
POST https://graph.microsoft.com/beta/subscriptions 
Content-Type: application/json
{ 
    "changeType":"created", 
    "resource":"print/taskDefinitions/{printTaskDefinition ID}/tasks", 
    "clientState":"secret", 
    "notificationUrl":"{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "expirationDateTime":"2020-01-30T22:42:09Z" 
} 
```

### <a name="response"></a><span data-ttu-id="7b50a-146">响应</span><span class="sxs-lookup"><span data-stu-id="7b50a-146">Response</span></span>

<span data-ttu-id="7b50a-147">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="7b50a-147">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
{ 
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity", 
    "id": "{Subscription ID}", 
    "resource": "print/taskDefinitions/{printTaskDefinition ID}/tasks", 
    "applicationId": "{application ID}", 
    "changeType": "created", 
    "clientState": "secret", 
    "notificationUrl": "{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "notificationQueryOptions": null, 
    "lifecycleNotificationUrl": null, 
    "expirationDateTime": "2020-12-30T22:42:09Z", 
    "creatorId": "{Creator ID}", 
    "includeResourceData": null, 
    "latestSupportedTlsVersion": "v1_2", 
    "encryptionCertificate": null, 
    "encryptionCertificateId": null 
}
```


## <a name="create-subscription-jobfetchable-event"></a><span data-ttu-id="7b50a-148">创建订阅：作业可创建事件</span><span class="sxs-lookup"><span data-stu-id="7b50a-148">Create subscription: JobFetchable event</span></span> 
<span data-ttu-id="7b50a-149">一些云应用程序需要准备好后从通用打印中下载打印作业。</span><span class="sxs-lookup"><span data-stu-id="7b50a-149">Some cloud applications need to download print jobs from Universal Print when they are ready.</span></span> <span data-ttu-id="7b50a-150">由于在云中运行的这些应用程序不在客户的防火墙后面，因此可在下载打印作业时使用 Microsoft Graph 更改通知。</span><span class="sxs-lookup"><span data-stu-id="7b50a-150">Because these applications running in the cloud are not behind the customer's firewall, they can use Microsoft Graph change notifications to be notified when a print job is ready to be downloaded.</span></span>

>[!NOTE]
><span data-ttu-id="7b50a-151">打印作业进入作业可打印状态时不可修改。</span><span class="sxs-lookup"><span data-stu-id="7b50a-151">Print jobs can't be modified when they enter the JobFetchable state.</span></span>
<span data-ttu-id="7b50a-152">需要针对每个打印机队列创建可作业通知。</span><span class="sxs-lookup"><span data-stu-id="7b50a-152">A JobFetchable notification needs to be created for each printer queue.</span></span> <span data-ttu-id="7b50a-153">创建订阅时：</span><span class="sxs-lookup"><span data-stu-id="7b50a-153">While creating the subscription:</span></span>
* <span data-ttu-id="7b50a-154">" `resource` "字段需要设置为"print/printer/{printer id}/jobs"。</span><span class="sxs-lookup"><span data-stu-id="7b50a-154">The `resource` field needs to be set as 'print/printers/{printer id}/jobs'.</span></span> 
* <span data-ttu-id="7b50a-155">`changeType` 字段需要设置为 `updated`。</span><span class="sxs-lookup"><span data-stu-id="7b50a-155">The `changeType` field needs to be set as `updated`.</span></span> 
* <span data-ttu-id="7b50a-156">`notificationQueryOptions` 字段需要设置为 `$filter = isFetchable eq true`。</span><span class="sxs-lookup"><span data-stu-id="7b50a-156">The `notificationQueryOptions` field needs to be set as `$filter = isFetchable eq true`.</span></span> 
* <span data-ttu-id="7b50a-157">" `expirationDateTime` "字段需要小于 [最大到期日期](/graph/api/resources/subscription?view=graph-rest-beta#maximum-length-of-subscription-per-resource-type)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-157">The `expirationDateTime` field needs to be less than the [maximum expiration time](/graph/api/resources/subscription?view=graph-rest-beta#maximum-length-of-subscription-per-resource-type).</span></span> 

<span data-ttu-id="7b50a-158">如需了解更多详情，请参阅 [openTypeExtension 资源类型](/graph/api/resources/subscription?view=graph-rest-beta#properties)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-158">For more details, see [Subscription resource type properties](/graph/api/resources/subscription?view=graph-rest-beta#properties).</span></span>

<span data-ttu-id="7b50a-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7b50a-159">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription"
}--> 
```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
    "changeType":"updated",
    "resource":"print/printers/{printer id}/jobs",
    "notificationQueryOptions": "$filter = isFetchable eq true", 
    "notificationUrl":"{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}",
    "expirationDateTime":"2020-12-30T22:42:09Z",
    "clientState":"mysecret"
} 
```

### <a name="response"></a><span data-ttu-id="7b50a-160">响应</span><span class="sxs-lookup"><span data-stu-id="7b50a-160">Response</span></span>

<span data-ttu-id="7b50a-161">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="7b50a-161">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
{ 
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity", 
    "id": "{Subscription ID}", 
    "resource": "print/printers/{printer ID}/jobs", 
    "applicationId": "{Application ID}", 
    "changeType": "updated", 
    "clientState": "mysecret", 
    "notificationUrl": "{URL for receiving the event – e.g. https://webhookappexample.azurewebsites.net/api/notifications}", 
    "notificationQueryOptions": "$filter = isFetchable eq true", 
    "lifecycleNotificationUrl": null, 
    "expirationDateTime": "2020-12-30T22:42:09Z", 
    "creatorId": "{Creator ID}", 
    "includeResourceData": null, 
    "latestSupportedTlsVersion": "v1_2", 
    "encryptionCertificate": null, 
    "encryptionCertificateId": null
}
```


## <a name="renewing-a-notification-subscription"></a><span data-ttu-id="7b50a-162">续订通知订阅</span><span class="sxs-lookup"><span data-stu-id="7b50a-162">Renewing a notification subscription</span></span>

<span data-ttu-id="7b50a-163">Microsoft Graph 对到期时间有限制。</span><span class="sxs-lookup"><span data-stu-id="7b50a-163">Microsoft Graph has a limit on the expiration time.</span></span> <span data-ttu-id="7b50a-164">有关详细信息，请参阅 [的到期日期](/graph/api/resources/subscription?view=graph-rest-beta#maximum-length-of-subscription-per-resource-type)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-164">For details, see [maximum expiration time](/graph/api/resources/subscription?view=graph-rest-beta#maximum-length-of-subscription-per-resource-type).</span></span> <span data-ttu-id="7b50a-165">若要继续接收通知，需使用更新订阅 API 更新 [定期续订](/graph/api/subscription-update?view=graph-rest-beta&tabs=http)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-165">To continue receiving notifications, the subscription needs to be renewed periodically by using the [Update subscription API](/graph/api/subscription-update?view=graph-rest-beta&tabs=http).</span></span> 

## <a name="other-operations-on-notification-subscriptions"></a><span data-ttu-id="7b50a-166">通知订阅的其他操作</span><span class="sxs-lookup"><span data-stu-id="7b50a-166">Other operations on notification subscriptions</span></span> 

<span data-ttu-id="7b50a-167">应用程序 [获取](/graph/api/subscription-get?view=graph-rest-beta&tabs=http) 的详细信息，或者 [删除](/graph/api/subscription-delete?view=graph-rest-beta&tabs=http) 订阅。</span><span class="sxs-lookup"><span data-stu-id="7b50a-167">Applications can [get](/graph/api/subscription-get?view=graph-rest-beta&tabs=http) details of the subscription or can [delete](/graph/api/subscription-delete?view=graph-rest-beta&tabs=http) a subscription when required.</span></span> <span data-ttu-id="7b50a-168">有关详细信息，请参阅 [Microsoft Graph API 通过更改通知](/graph/api/resources/webhooks?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-168">For details, see [Use the Microsoft Graph API to get change notifications](/graph/api/resources/webhooks?view=graph-rest-beta).</span></span>


## <a name="faqs"></a><span data-ttu-id="7b50a-169">常见问题</span><span class="sxs-lookup"><span data-stu-id="7b50a-169">FAQs</span></span>
### <a name="how-does-microsoft-graph-validate-notification-urls"></a><span data-ttu-id="7b50a-170">Microsoft Graph 如何验证通知 URL？</span><span class="sxs-lookup"><span data-stu-id="7b50a-170">How does Microsoft Graph validate notification URLs?</span></span>
<span data-ttu-id="7b50a-171">Microsoft Graph 将验证创建订阅前订阅请求的 **notificationurl** 属性中提供的通知终结点。</span><span class="sxs-lookup"><span data-stu-id="7b50a-171">Microsoft Graph validates the notification endpoint provided in the **notificationUrl** property of the subscription request before creating the subscription.</span></span>
<span data-ttu-id="7b50a-172">有关详细信息，请参阅 [终结点验证](/graph/webhooks#notification-endpoint-validation)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-172">For details, see [Notification endpoint validation](/graph/webhooks#notification-endpoint-validation).</span></span>

### <a name="what-are-applications-expected-to-do-after-receiving-a-change-notification"></a><span data-ttu-id="7b50a-173">收到更改通知后，应用程序应执行哪些操作？</span><span class="sxs-lookup"><span data-stu-id="7b50a-173">What are applications expected to do after receiving a change notification?</span></span>
<span data-ttu-id="7b50a-174">应用程序应处理和确认他们收到的每个更改通知。</span><span class="sxs-lookup"><span data-stu-id="7b50a-174">Applications should process and acknowledge every change notification they receive.</span></span> <span data-ttu-id="7b50a-175">有关详细信息，请参阅 [更改通知](/graph/webhooks#processing-the-change-notification)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-175">For details, see [Processing the change notification](/graph/webhooks#processing-the-change-notification).</span></span>

### <a name="how-can-i-get-a-list-of-active-subscriptions"></a><span data-ttu-id="7b50a-176">如何获取活动订阅列表？</span><span class="sxs-lookup"><span data-stu-id="7b50a-176">How can I get a list of active subscriptions?</span></span>
<span data-ttu-id="7b50a-177">若要详细了解如何检索 Web 网站订阅列表，请参阅 [订阅](/graph/api/subscription-list?view=graph-rest-beta&tabs=http)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-177">For details about how to retrieve a list of webhook subscriptions, see [List subscriptions](/graph/api/subscription-list?view=graph-rest-beta&tabs=http).</span></span>


## <a name="see-also"></a><span data-ttu-id="7b50a-178">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7b50a-178">See also</span></span>

- <span data-ttu-id="7b50a-179">若要深入了解 Microsoft Graph 中的云打印 API，请参阅 [云打印 API 概述](/graph/universal-print-concept-overview)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-179">To learn more about the cloud printing API in Microsoft Graph, see [Universal Print cloud printing API overview](/graph/universal-print-concept-overview).</span></span> 
- <span data-ttu-id="7b50a-180">有关 Microsoft Graph 中的云打印 API 的建议或反馈，请访问 [通用打印技术社区](https://aka.ms/community/UniversalPrint)。</span><span class="sxs-lookup"><span data-stu-id="7b50a-180">For suggestions or feedback about the cloud printing API in Microsoft Graph, visit the [Universal Print tech community](https://aka.ms/community/UniversalPrint).</span></span>