---
title: 设置用户数据更改的通知
description: Microsoft Graph API 使用 Webhook 机制将更改通知传递到客户端。客户端是用于配置自身的 URL 以接收更改通知的 Web 服务。客户端应用使用更改通知在更改时更新其状态。
author: davidmu1
ms.prod: non-product-specific
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: fda7792cab92391aba441ec62004ffb604f3ac3c
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469442"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="1c3e2-105">设置用户数据更改的通知</span><span class="sxs-lookup"><span data-stu-id="1c3e2-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="1c3e2-p102">Microsoft Graph API 使用 Webhook 机制将更改通知传递到客户端。客户端是用于配置自身的 URL 以接收更改通知的 Web 服务。客户端应用使用更改通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-p102">The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients. A client is a web service that configures its own URL to receive change notifications. Client apps use change notifications to update their state upon changes.</span></span>

<span data-ttu-id="1c3e2-109">Microsoft Graph 接受订阅请求之后，将更改通知推送到订阅中指定的 URL。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-109">After Microsoft Graph accepts the subscription request, it pushes change notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="1c3e2-110">然后应用根据其业务逻辑执行操作。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="1c3e2-111">例如，它提取更多数据、更新缓存和视图等。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-111">For example, it fetches more data, updates its cache and views, and so on.</span></span>


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [<span data-ttu-id="1c3e2-112">教程：在 Microsoft Graph 中使用变更通知和变更跟踪</span><span class="sxs-lookup"><span data-stu-id="1c3e2-112">Tutorial: Use Change Notifications and Track Changes with Microsoft Graph</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)

<span data-ttu-id="1c3e2-113">默认情况下，更改通知不包含资源数据，`id` 除外。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-113">By default, change notifications do not contain resource data, other than the `id`.</span></span> <span data-ttu-id="1c3e2-114">如果应用需要资源数据，则可以调用 Microsoft Graph API 以获取完整资源。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-114">If the app requires resource data, it can make calls to Microsoft Graph APIs to get the full resource.</span></span> <span data-ttu-id="1c3e2-115">本文使用 **用户** 资源作为使用更改通知的示例。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-115">This article uses the **user** resource as an example for working with change notifications.</span></span>

<span data-ttu-id="1c3e2-116">应用还可订阅包含资源数据的更改通知，避免执行其他 API 调用来访问数据。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-116">An app can also subscribe to change notifications that include resource data, to avoid having to make additional API calls to access the data.</span></span> <span data-ttu-id="1c3e2-117">此类应用将需要实现额外的代码来处理此类通知的要求，具体而言：响应订阅生命周期通知，验证通知的真实性，以及解密资源数据。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-117">Such apps will need to implement extra code to handle the requirements of such notifications, specifically: responding to subscription lifecycle notifications, validating the authenticity of notifications, and decrypting the resource data.</span></span> <span data-ttu-id="1c3e2-118">有关如何使用这些通知的详细信息，请参阅[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-118">For details about how to work with these notifications, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

## <a name="supported-resources"></a><span data-ttu-id="1c3e2-119">支持的资源</span><span class="sxs-lookup"><span data-stu-id="1c3e2-119">Supported resources</span></span>

<span data-ttu-id="1c3e2-120">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="1c3e2-120">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="1c3e2-121">云打印 [打印机][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-121">Cloud printing [printer][]</span></span>
- <span data-ttu-id="1c3e2-122">云打印 [printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-122">Cloud printing [printTaskDefinition][]</span></span>
- <span data-ttu-id="1c3e2-123">用户个人 OneDrive 上 _任何_ [driveItem][] 文件夹层次结构内的内容</span><span class="sxs-lookup"><span data-stu-id="1c3e2-123">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="1c3e2-124">OneDrive for Business 上 [driveItem][] _根文件夹_ 层次结构内的内容</span><span class="sxs-lookup"><span data-stu-id="1c3e2-124">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="1c3e2-125">[组][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-125">[group][]</span></span>
- <span data-ttu-id="1c3e2-126">Microsoft 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-126">Microsoft 365 group [conversation][]</span></span>
- <span data-ttu-id="1c3e2-127">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-127">Outlook [event][]</span></span>
- <span data-ttu-id="1c3e2-128">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-128">Outlook [message][]</span></span>
- <span data-ttu-id="1c3e2-129">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-129">Outlook personal [contact][]</span></span>
- <span data-ttu-id="1c3e2-130">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-130">Security [alert][]</span></span>
- <span data-ttu-id="1c3e2-131">SharePoint [列表][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-131">SharePoint [list][]</span></span>
- <span data-ttu-id="1c3e2-132">Teams [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-132">Teams [callRecord][]</span></span>
- <span data-ttu-id="1c3e2-133">Teams [chatMessage][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-133">Teams [chatMessage][]</span></span>
- <span data-ttu-id="1c3e2-134">Teams [状态][]（预览版）</span><span class="sxs-lookup"><span data-stu-id="1c3e2-134">Teams [presence][] (preview)</span></span>
- <span data-ttu-id="1c3e2-135">[todoTask][]（预览版）</span><span class="sxs-lookup"><span data-stu-id="1c3e2-135">[todoTask][] (preview)</span></span>
- <span data-ttu-id="1c3e2-136">[用户][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-136">[user][]</span></span>

<span data-ttu-id="1c3e2-137">可以创建对特定 Outlook 文件夹的订阅，例如收件箱：`me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="1c3e2-137">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="1c3e2-138">或以下顶级资源的订阅：`/me/messages`、`/me/contacts`、`/me/events`、`users`、`groups`、`/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="1c3e2-138">Or to a top-level resource: `/me/messages`, `/me/contacts`, `/me/events`, `users`, `groups`, `/communications/callRecords`</span></span>

<span data-ttu-id="1c3e2-139">或以下特定资源实例的订阅：`users/{id}`、`groups/{id}`、`groups/{id}/conversations`、`sites/{site-id}/lists/{list-id}`、`/communications/presences/{id}`</span><span class="sxs-lookup"><span data-stu-id="1c3e2-139">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`, `sites/{site-id}/lists/{list-id}`, `/communications/presences/{id}`</span></span>

<span data-ttu-id="1c3e2-140">或用户个人 OneDrive 中任何文件夹的订阅：`/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="1c3e2-140">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="1c3e2-141">或 SharePoint/OneDrive for Business 驱动器根文件夹的订阅：`/drive/root`</span><span class="sxs-lookup"><span data-stu-id="1c3e2-141">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="1c3e2-142">或对新[安全性 API](security-concept-overview.md) 警报的订阅：`/security/alerts?$filter=status eq 'newAlert'`、`/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span><span class="sxs-lookup"><span data-stu-id="1c3e2-142">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span></span>

<span data-ttu-id="1c3e2-143">或对用户的待办事项列表中的任务的订阅：`/me/todo/lists/{todoTaskListId}/tasks`</span><span class="sxs-lookup"><span data-stu-id="1c3e2-143">Or to the tasks in a user's To Do list: `/me/todo/lists/{todoTaskListId}/tasks`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="1c3e2-144">Azure AD 资源限制</span><span class="sxs-lookup"><span data-stu-id="1c3e2-144">Azure AD resource limitations</span></span>

<span data-ttu-id="1c3e2-145">基于 Azure AD 的资源（用户、组）采用了某些限制，超出限制时将会产生错误：</span><span class="sxs-lookup"><span data-stu-id="1c3e2-145">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="1c3e2-146">**请注意**：这些限制不适用于来自 Azure AD 以外的服务的资源。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-146">**Note**: These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="1c3e2-147">例如，应用可以创建许多更多的 `message` 或 `event` 资源订阅，这些订阅受到 Microsoft Graph 中的 Exchange Online 服务支持。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-147">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="1c3e2-148">最大订阅配额：</span><span class="sxs-lookup"><span data-stu-id="1c3e2-148">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="1c3e2-149">每个应用（适用于所有组合租户）：50,000 总订阅</span><span class="sxs-lookup"><span data-stu-id="1c3e2-149">Per app (for all tenants combined): 50,000 total subscriptions</span></span>
  - <span data-ttu-id="1c3e2-150">每个租户（适用于所有组合的应用）：总计 1000 个所有应用订阅</span><span class="sxs-lookup"><span data-stu-id="1c3e2-150">Per tenant (for all applications combined): 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="1c3e2-151">每个应用和租户组合：总订阅数 100</span><span class="sxs-lookup"><span data-stu-id="1c3e2-151">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="1c3e2-152">超出限制时，尝试创建订阅将导致[错误响应](errors.md) - `403 Forbidden`。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-152">When any limit is exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="1c3e2-153">`message` 属性将说明已超出什么限制。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-153">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="1c3e2-154">不支持 Azure AD B2C 租户。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-154">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="1c3e2-155">个人 Microsoft 帐户不支持用户实体的更改通知。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-155">Change notification for user entities are not supported for personal Microsoft accounts.</span></span>

- <span data-ttu-id="1c3e2-156">用户和租订阅存在一个[已知问题](known-issues.md#change-notifications)。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-156">A [known issue](known-issues.md#change-notifications) exists with user and group subscriptions.</span></span>

### <a name="outlook-resource-limitations"></a><span data-ttu-id="1c3e2-157">Outlook 资源限制</span><span class="sxs-lookup"><span data-stu-id="1c3e2-157">Outlook resource limitations</span></span>

<span data-ttu-id="1c3e2-158">订阅 Outlook 资源（如 **邮件**、**事件** 或 **联系人**）时，如果选择使用资源路径中的 *用户主体名称* UPN，则在 UPN 包含撇号的情况下，订阅请求可能会失败。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-158">When subscribing to Outlook resources such as **messages**, **events** or **contacts**, if you choose to use the *user principal name* UPN in the resource path, the subscription request might fail if the UPN contains an apostrophe.</span></span> <span data-ttu-id="1c3e2-159">请考虑使用 GUID 用户 ID 而不是 UPN，以避免遇到此问题。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-159">Consider using GUID user IDs instead of UPNs to avoid running into this problem.</span></span> <span data-ttu-id="1c3e2-160">例如，请勿使用资源路径：</span><span class="sxs-lookup"><span data-stu-id="1c3e2-160">For example, instead of using resource path:</span></span>

`/users/sh.o'neal@contoso.com/messages`

<span data-ttu-id="1c3e2-161">请使用：</span><span class="sxs-lookup"><span data-stu-id="1c3e2-161">Use:</span></span>

`/users/{guid-user-id}/messages`

<span data-ttu-id="1c3e2-162">对于所有应用程序，每个邮箱最多允许 1000 个活动订阅。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-162">A maximum of 1000 active subscriptions per mailbox for all applications is allowed.</span></span>

### <a name="teams-resource-limitations"></a><span data-ttu-id="1c3e2-163">Teams 资源限制</span><span class="sxs-lookup"><span data-stu-id="1c3e2-163">Teams resource limitations</span></span>

<span data-ttu-id="1c3e2-164">每个 Teams 资源都有不同的订阅配额。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-164">Each Teams resource has different subscription quotas.</span></span>

- <span data-ttu-id="1c3e2-165">对于 **callRecords** 的订阅：</span><span class="sxs-lookup"><span data-stu-id="1c3e2-165">For subscriptions to **callRecords**:</span></span>
  - <span data-ttu-id="1c3e2-166">每个组织：总共 100 个订阅</span><span class="sxs-lookup"><span data-stu-id="1c3e2-166">Per organization: 100 total subscriptions</span></span>

- <span data-ttu-id="1c3e2-167">对于 **chatMessages**（频道或聊天）的订阅：</span><span class="sxs-lookup"><span data-stu-id="1c3e2-167">For subscriptions to **chatMessages** (channels or chats):</span></span>
  - <span data-ttu-id="1c3e2-168">每个应用和频道或聊天组合：1 个订阅</span><span class="sxs-lookup"><span data-stu-id="1c3e2-168">Per app and channel or chat combination: 1 subscription</span></span>
  - <span data-ttu-id="1c3e2-169">每个组织：总共 10,000 个订阅</span><span class="sxs-lookup"><span data-stu-id="1c3e2-169">Per organization: 10,000 total subscriptions</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="1c3e2-170">订阅生命周期</span><span class="sxs-lookup"><span data-stu-id="1c3e2-170">Subscription lifetime</span></span>

<span data-ttu-id="1c3e2-171">订阅的生命周期有限。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-171">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="1c3e2-172">应用需要在订阅到期前续订订阅。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-172">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="1c3e2-173">否则，需要新建订阅。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-173">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="1c3e2-174">有关最长有效期的列表，请参阅[每个资源类型的最长订阅有效期](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type)。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-174">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="1c3e2-175">应用还可以随时取消订阅，以停止接收更改通知。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-175">Apps can also unsubscribe at any time to stop getting change notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="1c3e2-176">管理订阅</span><span class="sxs-lookup"><span data-stu-id="1c3e2-176">Managing subscriptions</span></span>

<span data-ttu-id="1c3e2-177">客户端可以创建订阅、续订订阅和删除订阅。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-177">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="1c3e2-178">创建订阅</span><span class="sxs-lookup"><span data-stu-id="1c3e2-178">Creating a subscription</span></span>

<span data-ttu-id="1c3e2-179">创建订阅是开始接收资源更改通知的第一步。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-179">Creating a subscription is the first step to start receiving change notifications for a resource.</span></span> <span data-ttu-id="1c3e2-180">订阅流程如下所示：</span><span class="sxs-lookup"><span data-stu-id="1c3e2-180">The subscription process is as follows:</span></span>

1. <span data-ttu-id="1c3e2-181">客户端发送特定资源的订阅 (POST) 请求。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-181">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="1c3e2-182">Microsoft Graph 验证请求。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-182">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="1c3e2-183">如果请求有效，Microsoft Graph 将验证令牌发送到通知 URL。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-183">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="1c3e2-184">如果该请求无效，Microsoft Graph 将发送包含代码和详细信息的错误响应。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-184">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="1c3e2-185">客户端将验证令牌发送回 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-185">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="1c3e2-186">Microsoft Graph 将响应发送回客户端。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-186">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="1c3e2-187">客户端必须存储订阅 ID 以便将更改通知与订阅关联。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-187">The client must store the subscription ID to correlate change notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="1c3e2-188">订阅请求示例</span><span class="sxs-lookup"><span data-stu-id="1c3e2-188">Subscription request example</span></span>

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

<span data-ttu-id="1c3e2-189">`changeType`、`notificationUrl`、`resource` 和 `expirationDateTime` 属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-189">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="1c3e2-190">如需属性定义和值，请参阅[订阅资源类型](/graph/api/resources/subscription?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-190">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="1c3e2-191">`resource` 属性指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-191">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="1c3e2-192">例如，可以创建特定邮件文件夹的订阅：`me/mailFolders('inbox')/messages`，或代表由管理员同意的用户：`users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-192">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="1c3e2-193">虽然不需要 `clientState`，但必须包括它才能符合我们建议的更改通知处理过程。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-193">Although `clientState` is not required, you must include it to comply with our recommended change notification handling process.</span></span> <span data-ttu-id="1c3e2-194">通过设置此属性后，可以确认收到的更改通知来自 Microsoft Graph 服务。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-194">Setting this property will allow you to confirm that change notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="1c3e2-195">因此，该属性的值应保密，并且只有你的应用程序和 Microsoft Graph 服务知道。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-195">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="1c3e2-196">如果成功，Microsoft Graph 将在正文中返回 `201 Created` 代码和 [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) 对象。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-196">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

> <span data-ttu-id="1c3e2-197">**注意：** 传递通知时，**notificationURL** 属性中包含的任何查询字符串参数都将包含在 HTTP POST 请求中。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-197">**Note:** Any query string parameter included in the **notificationUrl** property will be included in the HTTP POST request when notifications are being delivered.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="1c3e2-198">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="1c3e2-198">Notification endpoint validation</span></span>

<span data-ttu-id="1c3e2-199">Microsoft Graph 在创建订阅之前验证订阅请求的 `notificationUrl` 属性中提供的通知终结点。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-199">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="1c3e2-200">验证流程如下所示：</span><span class="sxs-lookup"><span data-stu-id="1c3e2-200">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="1c3e2-201">Microsoft Graph 对验证令牌进行编码，并将其包含在通知 URL 的 POST 请求中：</span><span class="sxs-lookup"><span data-stu-id="1c3e2-201">Microsoft Graph encodes a validation token and includes it in a POST request to the notification URL:</span></span>

    ``` http
    Content-Type: text/plain; charset=utf-8
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

1. <span data-ttu-id="1c3e2-202">客户端必须对上一步中提供的 `validationToken`查询参数进行正确的URL解码，并转义任何 HTML / JavaScript。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-202">The client must properly URL decode the `validationToken` query parameter provided in the preceding step, and escape any HTML/JavaScript.</span></span>

   <span data-ttu-id="1c3e2-203">转义是一种很好的做法，因为恶意参与者可将通知终结点用于跨网站脚本类型的攻击。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-203">Escaping is a good practice because malicious actors can use the notification endpoint for cross-site scripting type of attacks.</span></span>

   <span data-ttu-id="1c3e2-204">通常，将验证令牌值视为不透明，因为令牌格式通常可以更改，恕不另行通知。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-204">In general, treat the validation token value as opaque, as the token format can generally change without notice.</span></span> <span data-ttu-id="1c3e2-205">Microsoft Graph 从不发送任何包含 HTML 或 JavaScript 代码的值。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-205">Microsoft Graph never sends any value containing HTML or JavaScript code.</span></span>

1. <span data-ttu-id="1c3e2-206">客户端必须在第 1 步的 10 秒内提供具有以下特性的响应：</span><span class="sxs-lookup"><span data-stu-id="1c3e2-206">The client must provide a response with the following characteristics within 10 seconds of step 1:</span></span>

    - <span data-ttu-id="1c3e2-207">`HTTP 200 OK` 状态代码。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-207">A status code of `HTTP 200 OK`.</span></span>
    - <span data-ttu-id="1c3e2-208">`text/plain` 的内容类型。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-208">A content type of `text/plain`.</span></span>
    - <span data-ttu-id="1c3e2-209">包含 _已解码URL_ 验证令牌的正文。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-209">A body that includes the _URL decoded_ validation token.</span></span> <span data-ttu-id="1c3e2-210">只需将 `validationToken`查询参数中发送的相同字符串反射回来即可。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-210">Simply reflect back the same string that was sent in the `validationToken` query parameter.</span></span>

    <span data-ttu-id="1c3e2-211">在响应中提供验证令牌之后，客户端应放弃验证令牌。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-211">The client should discard the validation token after providing it in the response.</span></span>

    > <span data-ttu-id="1c3e2-212">**重要提示：** 如果客户端返回已编码的验证令牌，验证将失败。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-212">**Important:** If the client returns an encoded validation token, the validation will fail.</span></span>

<span data-ttu-id="1c3e2-213">另外，可以使用 [Microsoft Graph Postman Collection](use-postman.md) 来确认终结点能否正确实现验证请求。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-213">Additionally, you can use the [Microsoft Graph Postman collection](use-postman.md) to confirm that your endpoint properly implements the validation request.</span></span> <span data-ttu-id="1c3e2-214">“杂项”文件夹中的“订阅验证”请求提供了单元测试，可验证终结点提供的响应。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-214">The **Subscription Validation** request in the **Misc** folder provides unit tests that validate the response provided by your endpoint.</span></span>  

![验证响应测试结果](images/change-notifications/validation-request-tests-results.png)

### <a name="renewing-a-subscription"></a><span data-ttu-id="1c3e2-216">续订订阅</span><span class="sxs-lookup"><span data-stu-id="1c3e2-216">Renewing a subscription</span></span>

<span data-ttu-id="1c3e2-217">客户端可以续订特定过期日期的订阅，自请求时间起长达三天。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-217">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="1c3e2-218">`expirationDateTime` 属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-218">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="1c3e2-219">订阅续订示例</span><span class="sxs-lookup"><span data-stu-id="1c3e2-219">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="1c3e2-220">如果成功，Microsoft Graph 将在正文中返回 `200 OK` 代码和 [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) 对象。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-220">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="1c3e2-221">subscription 对象包括新的 `expirationDateTime` 值。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-221">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="1c3e2-222">删除订阅</span><span class="sxs-lookup"><span data-stu-id="1c3e2-222">Deleting a subscription</span></span>

<span data-ttu-id="1c3e2-223">客户端可以通过使用其 ID 删除订阅来停止接收更改通知。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-223">The client can stop receiving change notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="1c3e2-224">如果成功，Microsoft Graph 将返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-224">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="change-notifications"></a><span data-ttu-id="1c3e2-225">更改通知</span><span class="sxs-lookup"><span data-stu-id="1c3e2-225">Change notifications</span></span>

<span data-ttu-id="1c3e2-226">通过客户端订阅对资源的更改，只要资源发生更改，Microsoft Graph 就会向通知 URL 发送一个 `POST` 请求。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-226">With a client subscribing to changes to a resource, Microsoft Graph sends a `POST` request to the notification URL whenever the resource changes.</span></span> <span data-ttu-id="1c3e2-227">仅对订阅中指定类型的更改（例如 `created`）发送通知。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-227">It sends notifications only for changes of the type that's specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="1c3e2-228">**注意：** 如果客户端拥有监视相同资源并使用相同通知 URL 的多个订阅，则 Microsoft Graph 可以发送与不同订阅对应的多个更改通知，每个都显示相应的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-228">**Note:** If a client has multiple subscriptions that monitor the same resource and use the same notification URL, Microsoft Graph can send multiple change notifications that correspond to different subscriptions, each showing the corresponding subscription ID.</span></span> <span data-ttu-id="1c3e2-229">无法保证 `POST` 请求中的所有更改通知都属于单个订阅。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-229">There is no guarantee that all change notifications in the `POST` request belong to a single subscription.</span></span>

### <a name="change-notification-example"></a><span data-ttu-id="1c3e2-230">更改通知示例</span><span class="sxs-lookup"><span data-stu-id="1c3e2-230">Change notification example</span></span>

<span data-ttu-id="1c3e2-231">本节显示创建邮件的通知示例。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-231">This section shows an example of a notification for a message creation.</span></span> <span data-ttu-id="1c3e2-232">用户收到电子邮件时，Microsoft Graph 将发送更改通知，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-232">When the user receives an email, Microsoft Graph sends a change notification as shown in the following example.</span></span>
<span data-ttu-id="1c3e2-233">请注意，此通知位于 `value` 字段中表示的集合中。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-233">Note that the notification is in a collection represented in the `value` field.</span></span> <span data-ttu-id="1c3e2-234">有关通知负载的详细信息，请参见 [changeNotificationCollection](/graph/api/resources/changenotificationcollection)。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-234">See [changeNotificationCollection](/graph/api/resources/changenotificationcollection) for details of the notification payload.</span></span> 

<span data-ttu-id="1c3e2-235">发生许多更改时，Microsoft Graph 可能会在同一 `POST` 请求中发送对应于不同订阅的多个通知。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-235">When many changes occur, Microsoft Graph may send multiple notifications that correspond to different subscriptions in the same `POST` request.</span></span>

```json
{
  "value": [
    {
      "id": "lsgTZMr9KwAAA",
      "subscriptionId":"{subscription_guid}",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@{tenant_guid}/messages/{long_id_string}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
      "resourceData":
      {
        "@odata.type":"#Microsoft.Graph.Message",
        "@odata.id":"Users/{user_guid}@{tenant_guid}/Messages/{long_id_string}",
        "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
        "id":"{long_id_string}"
      }
    }
  ]
}
```

### <a name="processing-the-change-notification"></a><span data-ttu-id="1c3e2-236">处理更改通知</span><span class="sxs-lookup"><span data-stu-id="1c3e2-236">Processing the change notification</span></span>

<span data-ttu-id="1c3e2-237">进程应处理收到的每个更改通知。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-237">Your process should process every change notification it receives.</span></span> <span data-ttu-id="1c3e2-238">应用程序必须至少执行以下任务来处理更改通知：</span><span class="sxs-lookup"><span data-stu-id="1c3e2-238">The following are the minimum tasks that your app must perform to process a change notification:</span></span>

1. <span data-ttu-id="1c3e2-239">将响应中的 `202 - Accepted` 状态代码发送到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-239">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="1c3e2-240">如果 Microsoft Graph 未收到 2xx 类代码，它将在大约 4 小时的一段时间内尝试多次发布更改通知，之后，更改通知将被删除，且不会发送。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-240">If Microsoft Graph doesn't receive a 2xx class code, it will try to publishing the change notification a number of times, for a period of about 4 hours; after that, the change notification will be dropped and won't be delivered.</span></span>

    > <span data-ttu-id="1c3e2-241">**注意：** 收到更改通知后立即发送 `202 - Accepted` 状态代码，甚至在验证其真实性之前。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-241">**Note:** Send a `202 - Accepted` status code as soon as you receive the change notification, even before validating its authenticity.</span></span> <span data-ttu-id="1c3e2-242">只是确认接收更改通知，防止不必要的重试。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-242">You are simply acknowledging the receipt of the change notification and preventing unnecessary retries.</span></span> <span data-ttu-id="1c3e2-243">当前超时是 30 秒，但将来可能会减少，以优化服务性能。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-243">The current timeout is 30 seconds, but it might be reduced in the future to optimize service performance.</span></span> <span data-ttu-id="1c3e2-244">在 10 分钟内，对于 Microsoft Graph 中超过 10% 的请求，如果通知 URL 未在 30 秒内回复，以下所有通知将被延迟并重试 4 小时。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-244">If the notification URL doesn't reply within 30 seconds for more than 10% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be delayed and retried for a period of 4 hours.</span></span> <span data-ttu-id="1c3e2-245">在 10 分钟内，对于 Microsoft Graph 中超过 20% 的请求，如果通知 URL 未在 30 秒内回复，以下所有通知将被删除。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-245">If a notification URL doesn't reply within 30 seconds for more than 20% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be dropped.</span></span>

1. <span data-ttu-id="1c3e2-246">验证 `clientState` 属性。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-246">Validate the `clientState` property.</span></span> <span data-ttu-id="1c3e2-247">它必须与最初使用订阅创建请求提交的值匹配。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-247">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="1c3e2-248">**注意：** 如果不符合这个条件，无需将其视为有效更改通知。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-248">**Note:** If this isn't true, you should not consider this a valid change notification.</span></span> <span data-ttu-id="1c3e2-249">更改通知可能不是来自 Microsoft Graph，并且可能是由未授权操作者发送的。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-249">It is possible that the change notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="1c3e2-250">还应调查更改通知来自何处并采取适当的措施。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-250">You should also investigate where the change notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="1c3e2-251">基于业务逻辑更新应用程序。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-251">Update your application based on your business logic.</span></span>

<span data-ttu-id="1c3e2-252">对请求中的其他更改通知重复该过程。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-252">Repeat for other change notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="1c3e2-253">代码示例</span><span class="sxs-lookup"><span data-stu-id="1c3e2-253">Code samples</span></span>

<span data-ttu-id="1c3e2-254">可在 GitHub 上获取以下代码示例。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-254">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="1c3e2-255">Microsoft Graph 培训模块 - 在 Microsoft Graph 中使用变更通知和变更跟踪</span><span class="sxs-lookup"><span data-stu-id="1c3e2-255">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="1c3e2-256">面向 Node.js 的 Microsoft Graph Webhooks 示例</span><span class="sxs-lookup"><span data-stu-id="1c3e2-256">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/microsoftgraph/nodejs-webhooks-rest-sample)
- [<span data-ttu-id="1c3e2-257">适用于 ASP.NET Core 的 Microsoft Graph Webhook 示例</span><span class="sxs-lookup"><span data-stu-id="1c3e2-257">Microsoft Graph Webhooks Sample for ASP.NET Core</span></span>](https://github.com/microsoftgraph/aspnetcore-webhooks-sample)
- [<span data-ttu-id="1c3e2-258">面向 Java Spring 的 Microsoft Graph Webhooks 示例</span><span class="sxs-lookup"><span data-stu-id="1c3e2-258">Microsoft Graph Webhooks Sample for Java Spring</span></span>](https://github.com/microsoftgraph/java-spring-webhooks-sample)

## <a name="firewall-configuration"></a><span data-ttu-id="1c3e2-259">防火墙配置</span><span class="sxs-lookup"><span data-stu-id="1c3e2-259">Firewall configuration</span></span>

<span data-ttu-id="1c3e2-260">可选择性地配置防火墙，以保护通知 URL，仅允许来自 Microsoft Graph 的入站连接。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-260">You can optionally configure the firewall that protects your notification URL to allow inbound connections only from Microsoft Graph.</span></span> <span data-ttu-id="1c3e2-261">这使你可以进一步降低发送到通知 URL 的无效更改通知的风险。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-261">This allows you to reduce further exposure to invalid change notifications that are sent to your notification URL.</span></span> <span data-ttu-id="1c3e2-262">这些无效更改通知可能会试图触发已实施的自定义逻辑。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-262">These invalid change notifications can be trying to trigger the custom logic that you implemented.</span></span> <span data-ttu-id="1c3e2-263">有关 Microsoft Graph 用于传递更改通知的 IP 地址的完整列表，请参阅 [Microsoft 365 的其他终结点](/office365/enterprise/additional-office365-ip-addresses-and-urls)。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-263">For a complete list of IP addresses used by Microsoft Graph to deliver change notifications, see [additional endpoints for Microsoft 365](/office365/enterprise/additional-office365-ip-addresses-and-urls).</span></span>

> <span data-ttu-id="1c3e2-264">**注意：** 用于传递更改通知的已列出 IP 地址可以随时更新，恕不另行通知。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-264">**Note:** The listed IP addresses that are used to deliver change notifications can be updated at any time without notice.</span></span>

## <a name="latency"></a><span data-ttu-id="1c3e2-265">延迟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-265">Latency</span></span>

<span data-ttu-id="1c3e2-266">下表列出了服务中发生的事件与传递更改通知之间的预计延迟时间。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-266">The following table lists the latency to expect between an event happening in the service and the delivery of the change notification.</span></span>

| <span data-ttu-id="1c3e2-267">资源</span><span class="sxs-lookup"><span data-stu-id="1c3e2-267">Resource</span></span> | <span data-ttu-id="1c3e2-268">平均延迟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-268">Average latency</span></span> | <span data-ttu-id="1c3e2-269">最大延迟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-269">Maximum latency</span></span> |
|:-----|:-----|:-----|
|<span data-ttu-id="1c3e2-270">[警报][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-270">[alert][]</span></span> | <span data-ttu-id="1c3e2-271">少于 3 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-271">Less than 3 minutes</span></span> | <span data-ttu-id="1c3e2-272">5 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-272">5 minutes</span></span> |
|<span data-ttu-id="1c3e2-273">[callRecord][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-273">[callRecord][]</span></span> | <span data-ttu-id="1c3e2-274">少于 15 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-274">Less than 15 minutes</span></span> | <span data-ttu-id="1c3e2-275">60 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-275">60 minutes</span></span> |
|<span data-ttu-id="1c3e2-276">[chatMessage][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-276">[chatMessage][]</span></span> | <span data-ttu-id="1c3e2-277">少于 10 秒</span><span class="sxs-lookup"><span data-stu-id="1c3e2-277">Less than 10 seconds</span></span> | <span data-ttu-id="1c3e2-278">1 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-278">1 minute</span></span> |
|<span data-ttu-id="1c3e2-279">[联系人][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-279">[contact][]</span></span> | <span data-ttu-id="1c3e2-280">未知</span><span class="sxs-lookup"><span data-stu-id="1c3e2-280">Unknown</span></span> | <span data-ttu-id="1c3e2-281">未知</span><span class="sxs-lookup"><span data-stu-id="1c3e2-281">Unknown</span></span> |
|<span data-ttu-id="1c3e2-282">[对话][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-282">[conversation][]</span></span> | <span data-ttu-id="1c3e2-283">未知</span><span class="sxs-lookup"><span data-stu-id="1c3e2-283">Unknown</span></span> | <span data-ttu-id="1c3e2-284">未知</span><span class="sxs-lookup"><span data-stu-id="1c3e2-284">Unknown</span></span> |
|<span data-ttu-id="1c3e2-285">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-285">[driveItem][]</span></span> | <span data-ttu-id="1c3e2-286">小于 1 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-286">Less than 1 minute</span></span> | <span data-ttu-id="1c3e2-287">5 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-287">5 minutes</span></span> |
|<span data-ttu-id="1c3e2-288">[事件][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-288">[event][]</span></span> | <span data-ttu-id="1c3e2-289">未知</span><span class="sxs-lookup"><span data-stu-id="1c3e2-289">Unknown</span></span> | <span data-ttu-id="1c3e2-290">未知</span><span class="sxs-lookup"><span data-stu-id="1c3e2-290">Unknown</span></span> |
|<span data-ttu-id="1c3e2-291">[组][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-291">[group][]</span></span> | <span data-ttu-id="1c3e2-292">少于 2 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-292">Less than 2 minutes</span></span> | <span data-ttu-id="1c3e2-293">15 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-293">15 minutes</span></span> |
|<span data-ttu-id="1c3e2-294">[列表][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-294">[list][]</span></span> | <span data-ttu-id="1c3e2-295">小于 1 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-295">Less than 1 minute</span></span> | <span data-ttu-id="1c3e2-296">5 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-296">5 minutes</span></span> |
|<span data-ttu-id="1c3e2-297">[邮件][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-297">[message][]</span></span> | <span data-ttu-id="1c3e2-298">未知</span><span class="sxs-lookup"><span data-stu-id="1c3e2-298">Unknown</span></span> | <span data-ttu-id="1c3e2-299">未知</span><span class="sxs-lookup"><span data-stu-id="1c3e2-299">Unknown</span></span> |
|<span data-ttu-id="1c3e2-300">[状态][]（预览版）</span><span class="sxs-lookup"><span data-stu-id="1c3e2-300">[presence][] (preview)</span></span> | <span data-ttu-id="1c3e2-301">少于 10 秒</span><span class="sxs-lookup"><span data-stu-id="1c3e2-301">Less than 10 seconds</span></span> | <span data-ttu-id="1c3e2-302">1 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-302">1 minute</span></span> |
|<span data-ttu-id="1c3e2-303">[打印机][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-303">[printer][]</span></span> | <span data-ttu-id="1c3e2-304">小于 1 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-304">Less than 1 minute</span></span> | <span data-ttu-id="1c3e2-305">5 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-305">5 minutes</span></span> |
|<span data-ttu-id="1c3e2-306">[printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-306">[printTaskDefinition][]</span></span> | <span data-ttu-id="1c3e2-307">小于 1 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-307">Less than 1 minute</span></span> | <span data-ttu-id="1c3e2-308">5 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-308">5 minutes</span></span> |
|<span data-ttu-id="1c3e2-309">[todoTask][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-309">[todoTask][]</span></span> | <span data-ttu-id="1c3e2-310">少于 2 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-310">Less than 2 minutes</span></span> | <span data-ttu-id="1c3e2-311">15 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-311">15 minutes</span></span> |
|<span data-ttu-id="1c3e2-312">[用户][]</span><span class="sxs-lookup"><span data-stu-id="1c3e2-312">[user][]</span></span> | <span data-ttu-id="1c3e2-313">少于 2 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-313">Less than 2 minutes</span></span> | <span data-ttu-id="1c3e2-314">15 分钟</span><span class="sxs-lookup"><span data-stu-id="1c3e2-314">15 minutes</span></span> |

><span data-ttu-id="1c3e2-315">**注意**：为 **alert** 资源提供的延迟仅在创建 alert 后才适用。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-315">**Note:** The latency provided for the **alert** resource is only applicable after the alert itself has been created.</span></span> <span data-ttu-id="1c3e2-316">它不包括规则从数据创建警报所需的时间。</span><span class="sxs-lookup"><span data-stu-id="1c3e2-316">It does not include the time it takes for a rule to create an alert from the data.</span></span>

## <a name="see-also"></a><span data-ttu-id="1c3e2-317">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1c3e2-317">See also</span></span>

- [<span data-ttu-id="1c3e2-318">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="1c3e2-318">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="1c3e2-319">获取订阅</span><span class="sxs-lookup"><span data-stu-id="1c3e2-319">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="1c3e2-320">创建订阅</span><span class="sxs-lookup"><span data-stu-id="1c3e2-320">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- <span data-ttu-id="1c3e2-321">[changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta) 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c3e2-321">[changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta) resource type</span></span>
- <span data-ttu-id="1c3e2-322">[changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta) 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c3e2-322">[changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta) resource type</span></span>
- [<span data-ttu-id="1c3e2-323">更改通知和更改跟踪教程</span><span class="sxs-lookup"><span data-stu-id="1c3e2-323">Change notifications and change tracking tutorial</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)
- [<span data-ttu-id="1c3e2-324">生命周期通知</span><span class="sxs-lookup"><span data-stu-id="1c3e2-324">Lifecycle notifications</span></span>](./webhooks-lifecycle.md)

[联系人]: /graph/api/resources/contact?view=graph-rest-1.0
[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[对话]: /graph/api/resources/conversation?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[driveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[事件]: /graph/api/resources/event?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[组]: /graph/api/resources/group?view=graph-rest-1.0
[group]: /graph/api/resources/group?view=graph-rest-1.0
[邮件]: /graph/api/resources/message?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[用户]: /graph/api/resources/user?view=graph-rest-1.0
[user]: /graph/api/resources/user?view=graph-rest-1.0
[警报]: /graph/api/resources/alert?view=graph-rest-1.0
[alert]: /graph/api/resources/alert?view=graph-rest-1.0
[callRecord]: /graph/api/resources/callrecords-callrecord?view=graph-rest-1.0
[状态]: /graph/api/resources/presence
[presence]: /graph/api/resources/presence
[chatMessage]: /graph/api/resources/chatmessage
[列表]: /graph/api/resources/list
[list]: /graph/api/resources/list
[打印机]: /graph/api/resources/printer
[printer]: /graph/api/resources/printer
[printTaskDefinition]: /graph/api/resources/printtaskdefinition
[todoTask]: /graph/api/resources/todotask