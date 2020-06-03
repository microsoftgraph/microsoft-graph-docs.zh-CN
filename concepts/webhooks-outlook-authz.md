---
title: 减少缺少的订阅和 Outlook 资源的更改通知（预览）
description: 由于用户密码重置等安全事件，Outlook 可能会暂停传递更改通知。 需要处理特殊的生命周期事件， `subscriptionRemoved` `missed` 以确保不中断的更改通知传递。
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 8b2174ea14dd7e3d6af7f0b4a447c4e5afa6fce1
ms.sourcegitcommit: 4fa554d92a684d7720db1bd96befb9dea8d6ba5f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/30/2020
ms.locfileid: "44429626"
---
# <a name="reduce-missing-subscriptions-and-change-notifications-for-outlook-resources-preview"></a><span data-ttu-id="479c4-104">减少缺少的订阅和 Outlook 资源的更改通知（预览）</span><span class="sxs-lookup"><span data-stu-id="479c4-104">Reduce missing subscriptions and change notifications for Outlook resources (preview)</span></span> 

<span data-ttu-id="479c4-105">订阅更改 Outlook 资源通知的应用程序可能会删除订阅，并错过一些更改通知。</span><span class="sxs-lookup"><span data-stu-id="479c4-105">Apps subscribing to change notifications for Outlook resources might get their subscriptions removed and miss some change notifications.</span></span> <span data-ttu-id="479c4-106">应用应实现逻辑以检测丢失和恢复丢失，并恢复连续更改通知流。</span><span class="sxs-lookup"><span data-stu-id="479c4-106">Apps should implement logic to detect and recover from the loss, and resume a continuous change notification flow.</span></span>

<span data-ttu-id="479c4-107">Outlook 中的某些事件可能导致订阅被删除。</span><span class="sxs-lookup"><span data-stu-id="479c4-107">Certain events in Outlook can cause a subscription to be removed.</span></span> <span data-ttu-id="479c4-108">这些事件包括：</span><span class="sxs-lookup"><span data-stu-id="479c4-108">These events include:</span></span>

- <span data-ttu-id="479c4-109">用户的密码已重置</span><span class="sxs-lookup"><span data-stu-id="479c4-109">User's password has been reset</span></span>
- <span data-ttu-id="479c4-110">用户的设备不合规</span><span class="sxs-lookup"><span data-stu-id="479c4-110">User's device is out of compliance</span></span>
-   <span data-ttu-id="479c4-111">用户的帐户已吊销</span><span class="sxs-lookup"><span data-stu-id="479c4-111">User's account has been revoked</span></span>

<span data-ttu-id="479c4-112">发生此类事件时，Outlook 将发送特殊生命周期通知 `subscriptionRemoved`。</span><span class="sxs-lookup"><span data-stu-id="479c4-112">When such an event happens, Outlook sends a special lifecycle notification, `subscriptionRemoved`.</span></span>

<span data-ttu-id="479c4-113">`missed`如果无法将更改通知传递给应用程序，Outlook 还会发送另一个生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="479c4-113">Outlook also sends another lifecycle notification, `missed`, if a change notification cannot be delivered to an app.</span></span>

<span data-ttu-id="479c4-114">为 Outlook 资源（如**邮件**和**事件**）订阅更改通知的应用程序应侦听 `subscriptionRemoved` 和 `missed` 发出以下信号并执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="479c4-114">An app subscribing to change notifications for Outlook resources, such as **message** and **event**, should listen to the `subscriptionRemoved` and `missed` signals and do the following:</span></span>

- <span data-ttu-id="479c4-115">在收到 `subscriptionRemoved` 生命周期通知后，应用应重新创建订阅，以便保持连续流。</span><span class="sxs-lookup"><span data-stu-id="479c4-115">Upon receiving a `subscriptionRemoved` lifecycle notification, the app should recreate the subscription in order to maintain a continuous flow.</span></span>
- <span data-ttu-id="479c4-116">在接收 `missed` 生命周期通知时，应用应使用 Microsoft Graph 重新同步资源数据。</span><span class="sxs-lookup"><span data-stu-id="479c4-116">On receiving a `missed` lifecycle notification, the app should resynchronize resource data using Microsoft Graph.</span></span>

<span data-ttu-id="479c4-117">若要接收生命周期通知，可以使用已接收更改通知的现有**notificationUrl**终结点，也可以在单独的终结点中注册单独的**lifecycleNotificationUrl**以接收 `subscriptionRemoved` 和 `missed` 生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="479c4-117">To receive lifecycle notifications, you can use the existing **notificationUrl** endpoint that already receives change notifications, or you can register a separate **lifecycleNotificationUrl** to receive `subscriptionRemoved` and `missed` lifecycle notifications in a separate endpoint.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="479c4-118">创建订阅</span><span class="sxs-lookup"><span data-stu-id="479c4-118">Creating a subscription</span></span>

<span data-ttu-id="479c4-119">创建订阅时，可以使用**lifecycleNotificationUrl**属性指定单独的终结点。</span><span class="sxs-lookup"><span data-stu-id="479c4-119">When creating a subscription, you can specify a separate endpoint using the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="479c4-120">如果指定终结点，所有当前和未来类型的生命周期通知都将传递到那里。</span><span class="sxs-lookup"><span data-stu-id="479c4-120">If you specify the endpoint, all current and future types of lifecycle notifications will be delivered there.</span></span> <span data-ttu-id="479c4-121">否则， `subscriptionRemoved` `missed` 会将生命周期通知传递到现有的**notificationUrl**以供所有现有订阅。</span><span class="sxs-lookup"><span data-stu-id="479c4-121">Otherwise, `subscriptionRemoved` and `missed` lifecycle notifications will be delivered to the existing **notificationUrl** for all existing subscriptions.</span></span>

> <span data-ttu-id="479c4-122">**注意：** 只能使用 Microsoft Graph beta API 设置或读取 **lifecycleNotificationUrl** 属性。</span><span class="sxs-lookup"><span data-stu-id="479c4-122">**Note:** The **lifecycleNotificationUrl** property can only be set or read using Microsoft Graph beta APIs.</span></span> <span data-ttu-id="479c4-123">但是，使用 beta API 创建的订阅与使用 v1.0 创建的订阅存储在同一个生产环境中，因此除了使用 v1.0 API 创建的订阅外，还可以实现新 Outlook 流程。</span><span class="sxs-lookup"><span data-stu-id="479c4-123">However, subscriptions created using beta APIs are stored in the same production environment as those created using v1.0, so you can implement the new Outlook flow in addition to your subscriptions creating using v1.0 APIs.</span></span>

> <span data-ttu-id="479c4-124">通过 v1.0 API 创建的订阅将收到生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="479c4-124">Subscriptions created via the v1.0 APIs will receive lifecycle notifications.</span></span> 

### <a name="subscription-request-example"></a><span data-ttu-id="479c4-125">订阅请求示例</span><span class="sxs-lookup"><span data-stu-id="479c4-125">Subscription request example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/users/{id}/messages",
  "expirationDateTime": "2019-03-20T11:00:00.0000000Z",
  "clientState": "<secretClientState>"
}
```
 
> <span data-ttu-id="479c4-126">**重要提示：** 对两个通知 URL 使用相同的主机名。</span><span class="sxs-lookup"><span data-stu-id="479c4-126">**Important:** Use the same hostname for both notifications URLs.</span></span> 

> <span data-ttu-id="479c4-127">**注意：** 您需要验证这两个终结点，如[管理订阅](webhooks.md#managing-subscriptions)中所述。</span><span class="sxs-lookup"><span data-stu-id="479c4-127">**Note:** You need to validate both endpoints as described in [Managing subscriptions](webhooks.md#managing-subscriptions).</span></span>
<span data-ttu-id="479c4-128">如果选择对两个终结点使用相同的 URL，将收到并响应两个验证请求。</span><span class="sxs-lookup"><span data-stu-id="479c4-128">If you choose to use the same URL for both endpoints you will receive and respond to two validation requests.</span></span>

> <span data-ttu-id="479c4-129">**注意：** 无法更新 (`PATCH`) 现有订阅以添加 **lifecycleNotificationUrl** 属性。</span><span class="sxs-lookup"><span data-stu-id="479c4-129">**Note:** You cannot update (`PATCH`) the existing subscriptions to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="479c4-130">应删除此类现有订阅，创建新订阅并指定 **lifecycleNotificationUrl** 属性。</span><span class="sxs-lookup"><span data-stu-id="479c4-130">You should remove such existing subscriptions, and create new subscriptions and specify the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="479c4-131">不带**lifecycleNotificationUrl**属性的现有订阅将 `subscriptionRemoved` `missed` 通过**notificationUrl**接收和生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="479c4-131">Existing subscriptions without **lifecycleNotificationUrl** property will receive the `subscriptionRemoved` and `missed` lifecycle notifications via the **notificationUrl**.</span></span> 

## <a name="responding-to-subscriptionremoved-notifications"></a><span data-ttu-id="479c4-132">响应 subscriptionRemoved 通知</span><span class="sxs-lookup"><span data-stu-id="479c4-132">Responding to subscriptionRemoved notifications</span></span>

<span data-ttu-id="479c4-133">`subscriptionRemoved`如果要继续接收更改通知，则生命周期通知会通知您已删除订阅且应重新创建订阅。</span><span class="sxs-lookup"><span data-stu-id="479c4-133">The `subscriptionRemoved` lifecycle notification informs you that a subscription has been removed and should be recreated, if you want to continue receiving change notifications.</span></span> 

<span data-ttu-id="479c4-134">您可以创建长期订阅（3天），更改通知将开始在**notificationUrl**中流动。</span><span class="sxs-lookup"><span data-stu-id="479c4-134">You can create a long-lived subscription (3 days), and change notifications will start flowing to the **notificationUrl**.</span></span> <span data-ttu-id="479c4-135">但是，资源数据的访问条件可能会随时间变化。</span><span class="sxs-lookup"><span data-stu-id="479c4-135">However, the conditions of access to the resource data might change over time.</span></span> <span data-ttu-id="479c4-136">例如，Outlook 服务中的事件可能会发生，需要应用程序对于用户重新进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="479c4-136">For example, an event in the Outlook service might occur that requires the app to re-authenticate the user.</span></span> <span data-ttu-id="479c4-137">在此类情况下，流程如下所示：</span><span class="sxs-lookup"><span data-stu-id="479c4-137">In such a case, the flow is as follows:</span></span>

1. <span data-ttu-id="479c4-138">Outlook 检测到需要从 Microsoft Graph 删除订阅。</span><span class="sxs-lookup"><span data-stu-id="479c4-138">Outlook detects that a subscription needs to be removed from Microsoft Graph.</span></span>
    
    <span data-ttu-id="479c4-139">这些事件没有固定的节奏。</span><span class="sxs-lookup"><span data-stu-id="479c4-139">There is no set cadence for these events.</span></span> <span data-ttu-id="479c4-140">对于某些资源，它们可能经常发生，而对于其他资源，几乎永远不会发生。</span><span class="sxs-lookup"><span data-stu-id="479c4-140">They might occur frequently for some resources, and almost never for others.</span></span>

2. <span data-ttu-id="479c4-141">Microsoft Graph 将 `subscriptionRemoved` 生命周期通知发送到**lifecycleNotificationUrl** （如果已指定）或**notificationUrl**。</span><span class="sxs-lookup"><span data-stu-id="479c4-141">Microsoft Graph sends a `subscriptionRemoved` lifecycle notification to the **lifecycleNotificationUrl** (if specified), or the **notificationUrl**.</span></span>  

3. <span data-ttu-id="479c4-142">您可以通过为同一资源创建新的订阅来响应此生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="479c4-142">You can respond to this lifecycle notification by creating a new subscription for the same resource.</span></span> <span data-ttu-id="479c4-143">为此，你需要提供有效的访问令牌；在某些情况下，这意味着应用程序需要重新验证用户以获取新的有效访问令牌。</span><span class="sxs-lookup"><span data-stu-id="479c4-143">To do this, you need to present a valid access token; in some cases this means the app needs to re-authenticate the user to obtain a new valid access token.</span></span>

4. <span data-ttu-id="479c4-144">如果您已成功创建新的订阅，更改通知将重新开始流动。</span><span class="sxs-lookup"><span data-stu-id="479c4-144">If you successfully create a new subscription, change notifications will start flowing again.</span></span> <span data-ttu-id="479c4-145">但是，如果失败（例如，应用程序无法获取有效的访问令牌），则不会发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="479c4-145">However, if you fail (for example, the app can't obtain a valid access token), change notifications will not be sent.</span></span>

5. <span data-ttu-id="479c4-146">创建新订阅后，可以同步资源数据以标识任何缺失的更改。</span><span class="sxs-lookup"><span data-stu-id="479c4-146">After creating the new subscription, you can sync the resource data to identify any missing changes.</span></span>

### <a name="subscriptionremoved-notification-example"></a><span data-ttu-id="479c4-147">subscriptionRemoved 通知示例</span><span class="sxs-lookup"><span data-stu-id="479c4-147">subscriptionRemoved notification example</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2019-03-20T11:00:00.0000000Z",
      "tenantId": "<tenant_guid>",
      "clientState":"<secretClientState>",
      "lifecycleEvent": "subscriptionRemoved"
    }
  ]
}
```

<span data-ttu-id="479c4-148">有关此类型通知的一些注意事项：</span><span class="sxs-lookup"><span data-stu-id="479c4-148">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="479c4-149">`"lifecycleEvent": "subscriptionRemoved"` 字段将此通知指定为与订阅删除相关。</span><span class="sxs-lookup"><span data-stu-id="479c4-149">The `"lifecycleEvent": "subscriptionRemoved"` field designates this notification as related to subscription removal.</span></span> <span data-ttu-id="479c4-150">其他类型的生命周期通知也是可能的，将来会引入新的通知。</span><span class="sxs-lookup"><span data-stu-id="479c4-150">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="479c4-151">生命周期通知不包含有关特定资源的任何信息，因为它与资源更改无关，而是订阅状态更改。</span><span class="sxs-lookup"><span data-stu-id="479c4-151">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="479c4-152">与更改通知类似，生命周期通知可以一起分批（在**值**数组中），每个都有可能不同的**lifecycleEvent**值。</span><span class="sxs-lookup"><span data-stu-id="479c4-152">Similar to change notifications, lifecycle notifications can be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="479c4-153">相应地处理批次中的每个生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="479c4-153">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="479c4-154">**注意：** 有关在传递更改通知时发送的数据的完整说明，请参阅[changeNotificationCollection](/graph/api/resources/changenotificationcollection)。</span><span class="sxs-lookup"><span data-stu-id="479c4-154">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="479c4-155">要采取的操作</span><span class="sxs-lookup"><span data-stu-id="479c4-155">Actions to take</span></span>

1. <span data-ttu-id="479c4-156">通过使用对 POST 呼叫做出响应来[确认](webhooks.md#change-notifications)收到生命周期通知 `202 - Accepted` 。</span><span class="sxs-lookup"><span data-stu-id="479c4-156">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="479c4-157">[验证](webhooks.md#change-notifications)生命周期通知的真实性。</span><span class="sxs-lookup"><span data-stu-id="479c4-157">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="479c4-158">确保应用程序具有执行下一步操作的有效访问令牌。</span><span class="sxs-lookup"><span data-stu-id="479c4-158">Ensure that the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="479c4-159">**注意：** 如果使用其中一个[身份验证库](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)，他们将通过重复使用有效的缓存令牌或获取新令牌，其中包括要求用户（使用新密码）再次登录来处理此问题。</span><span class="sxs-lookup"><span data-stu-id="479c4-159">**Note:** If you're using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to sign in again (with a new password).</span></span> <span data-ttu-id="479c4-160">请注意，获取新令牌可能会失败，因为访问条件可能已更改，并且可能不再允许调用者访问资源数据。</span><span class="sxs-lookup"><span data-stu-id="479c4-160">Note that obtaining a new token might fail, because the conditions of access might have changed, and the caller might no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="479c4-161">使用[此处](webhooks.md#subscription-request-example)描述的标准流程创建新订阅。</span><span class="sxs-lookup"><span data-stu-id="479c4-161">Create a new subscription using the standard process described [here](webhooks.md#subscription-request-example).</span></span>

  > <span data-ttu-id="479c4-162">**注意：** 此操作可能会失败，因为系统执行的授权检查可能会拒绝应用程序或用户访问资源。</span><span class="sxs-lookup"><span data-stu-id="479c4-162">**Note:** This action might fail, because the authorization checks performed by the system might deny the app or the user access to the resource.</span></span> <span data-ttu-id="479c4-163">应用程序可能需要从用户处获取新的访问令牌以成功重新授权订阅。</span><span class="sxs-lookup"><span data-stu-id="479c4-163">It might be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> <span data-ttu-id="479c4-164">以后可以随时重试这些操作，例如，当访问条件发生变化时。</span><span class="sxs-lookup"><span data-stu-id="479c4-164">You can retry these actions later, at any time; for example, when the conditions of access have changed.</span></span> <span data-ttu-id="479c4-165">从发送生命周期通知到应用程序成功重新创建订阅的时间段中的任何资源更改将丢失。</span><span class="sxs-lookup"><span data-stu-id="479c4-165">Any resource changes in the time period from when the lifecycle notification was sent, to when the app recreates the subscription successfully, will be lost.</span></span> <span data-ttu-id="479c4-166">该应用程序需要自己获取这些更改。</span><span class="sxs-lookup"><span data-stu-id="479c4-166">The app will need to fetch those changes on its own.</span></span>

5. <span data-ttu-id="479c4-167">创建新订阅后，从上次已知的已知资源数据中同步收到此资源的更改通知;例如：`GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span><span class="sxs-lookup"><span data-stu-id="479c4-167">After creating the new subscription, sync any missing resource data from the last known time you received a change notification for this resource; for example: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span></span>

## <a name="responding-to-missed-notifications"></a><span data-ttu-id="479c4-168">响应错过的通知</span><span class="sxs-lookup"><span data-stu-id="479c4-168">Responding to missed notifications</span></span>

<span data-ttu-id="479c4-169">这些信号通知您可能尚未传递某些更改通知。</span><span class="sxs-lookup"><span data-stu-id="479c4-169">These signals inform you that some change notifications might not have been delivered.</span></span> <span data-ttu-id="479c4-170">你应决定是否忽略或处理这些信号。</span><span class="sxs-lookup"><span data-stu-id="479c4-170">You should decide if you ignore or handle these signals.</span></span>

### <a name="notification-example"></a><span data-ttu-id="479c4-171">通知示例</span><span class="sxs-lookup"><span data-stu-id="479c4-171">Notification example</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2019-03-20T11:00:00.0000000Z",
      "tenantId": "<tenant_guid>",
      "clientState":"<secretClientState>",
      "lifecycleEvent": "missed"
    }
  ]
}
```

<span data-ttu-id="479c4-172">有关此类型通知的一些注意事项：</span><span class="sxs-lookup"><span data-stu-id="479c4-172">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="479c4-173">该 `"lifecycleEvent": "missed"` 字段将此字段指定为关于错过的更改通知的信号。</span><span class="sxs-lookup"><span data-stu-id="479c4-173">The `"lifecycleEvent": "missed"` field designates this as a signal about missed change notifications.</span></span> <span data-ttu-id="479c4-174">其他类型的生命周期通知也是可能的，将来会引入新的通知。</span><span class="sxs-lookup"><span data-stu-id="479c4-174">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="479c4-175">生命周期通知不包含有关特定资源的任何信息，因为它与资源更改无关，而是订阅状态更改。</span><span class="sxs-lookup"><span data-stu-id="479c4-175">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="479c4-176">与更改通知类似，生命周期通知可能会一起分批（在**值**数组中），每个都有可能不同的**lifecycleEvent**值。</span><span class="sxs-lookup"><span data-stu-id="479c4-176">Similar to change notifications, lifecycle notifications might be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="479c4-177">相应地处理批次中的每个生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="479c4-177">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="479c4-178">**注意：** 有关在传递更改通知时发送的数据的完整说明，请参阅[changeNotificationCollection](/graph/api/resources/changenotificationcollection)。</span><span class="sxs-lookup"><span data-stu-id="479c4-178">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="479c4-179">要采取的操作</span><span class="sxs-lookup"><span data-stu-id="479c4-179">Actions to take</span></span>

1. <span data-ttu-id="479c4-180">通过使用对 POST 呼叫做出响应来[确认](webhooks.md#change-notifications)收到生命周期通知 `202 - Accepted` 。</span><span class="sxs-lookup"><span data-stu-id="479c4-180">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
    - <span data-ttu-id="479c4-181">如果忽略这些信号，则无需执行其他任何操作。</span><span class="sxs-lookup"><span data-stu-id="479c4-181">If you ignore these signals, do nothing else.</span></span> <span data-ttu-id="479c4-182">或者：</span><span class="sxs-lookup"><span data-stu-id="479c4-182">Otherwise:</span></span>
2. <span data-ttu-id="479c4-183">[验证](webhooks.md#change-notifications)生命周期通知的真实性。</span><span class="sxs-lookup"><span data-stu-id="479c4-183">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="479c4-184">执行资源的完整数据重新同步，以标识未作为通知发送的更改。</span><span class="sxs-lookup"><span data-stu-id="479c4-184">Perform a full data resync of the resource to identify the changes that were not delivered as notifications.</span></span> 


## <a name="future-proof-the-code-handling-lifecycle-notifications"></a><span data-ttu-id="479c4-185">前瞻性的代码处理生命周期通知</span><span class="sxs-lookup"><span data-stu-id="479c4-185">Future-proof the code handling lifecycle notifications</span></span>

<span data-ttu-id="479c4-186">将来，Microsoft Graph 将添加更多类型的订阅生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="479c4-186">In the future, Microsoft Graph will add more types of subscription lifecycle notifications.</span></span> <span data-ttu-id="479c4-187">它们将被发布到相同的终结点：**lifecycleNotificationUrl**，但是它们在 **lifecycleEvent** 下将具有不同的值，并且可能包含稍微不同的模式和属性，这些模式和属性特定于将为其发布的方案。</span><span class="sxs-lookup"><span data-stu-id="479c4-187">They will be posted to the same endpoint: **lifecycleNotificationUrl**, but they will have a different value under **lifecycleEvent** and might contain a slightly different schema and properties, specific to the scenario for which they will be issued.</span></span>

<span data-ttu-id="479c4-188">你应该以前瞻性的方式实现代码，以便在 Microsoft Graph 引入新类型的生命周期通知时不会中断。</span><span class="sxs-lookup"><span data-stu-id="479c4-188">You should implement your code in a future-proof way so it does not break when Microsoft Graph introduces new types of lifecycle notifications.</span></span> <span data-ttu-id="479c4-189">建议使用以下方法：</span><span class="sxs-lookup"><span data-stu-id="479c4-189">We recommend the following approach:</span></span>

1. <span data-ttu-id="479c4-190">使用**lifecycleEvent**属性，将每个生命周期通知显式标识为您支持的事件。</span><span class="sxs-lookup"><span data-stu-id="479c4-190">Explicitly identify each lifecycle notification as an event that you support, using the **lifecycleEvent** property.</span></span> <span data-ttu-id="479c4-191">例如，查找 `"lifecycleEvent": "subscriptionRemoved"` 属性标识特定事件并处理它。</span><span class="sxs-lookup"><span data-stu-id="479c4-191">For example, look for the `"lifecycleEvent": "subscriptionRemoved"` property to identify a specific event, and handle it.</span></span>

2. <span data-ttu-id="479c4-192">监视新 scenarions 的生命周期通知通知。</span><span class="sxs-lookup"><span data-stu-id="479c4-192">Watch for announcements of lifecycle notifications for new scenarions.</span></span> <span data-ttu-id="479c4-193">将来可能会有更多类型的生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="479c4-193">There might be more types of lifecycle notifications in the future.</span></span>

3. <span data-ttu-id="479c4-194">在您的应用程序中，忽略应用程序不识别的任何生命周期通知，并将其记录出来以获得意识。</span><span class="sxs-lookup"><span data-stu-id="479c4-194">In your app, ignore any lifecycle notification that the app does not recognize, and log them to gain awareness.</span></span>

4. <span data-ttu-id="479c4-195">你可以自行决定查找新生命周期通知的相关文档，并根据需要实施对它们的支持。</span><span class="sxs-lookup"><span data-stu-id="479c4-195">At your discretion, look up the related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="see-also"></a><span data-ttu-id="479c4-196">另请参阅</span><span class="sxs-lookup"><span data-stu-id="479c4-196">See also</span></span>

- [<span data-ttu-id="479c4-197">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="479c4-197">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="479c4-198">获取订阅</span><span class="sxs-lookup"><span data-stu-id="479c4-198">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="479c4-199">创建订阅</span><span class="sxs-lookup"><span data-stu-id="479c4-199">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="479c4-200">删除订阅</span><span class="sxs-lookup"><span data-stu-id="479c4-200">Delete subscription</span></span>](/graph/api/subscription-delete?view=graph-rest-1.0)
- [<span data-ttu-id="479c4-201">更新订阅</span><span class="sxs-lookup"><span data-stu-id="479c4-201">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
