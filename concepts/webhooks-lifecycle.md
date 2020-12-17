---
title: 减少缺失订阅和更改通知
description: 订阅更改通知的应用可能会删除其订阅并错过一些更改通知。 应用程序应实现逻辑以进行检测并恢复丢失的内容，以及恢复连续更改通知流程。
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: bf870eecce08d61b6ad80ce774ed2b97af3ce3b2
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921688"
---
# <a name="reduce-missing-subscriptions-and-change-notifications"></a><span data-ttu-id="e2ac5-104">减少缺失订阅和更改通知</span><span class="sxs-lookup"><span data-stu-id="e2ac5-104">Reduce missing subscriptions and change notifications</span></span>

<span data-ttu-id="e2ac5-105">订阅更改通知的应用可能会删除其订阅并错过一些更改通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-105">Apps subscribing to change notifications might get their subscriptions removed and miss some change notifications.</span></span> <span data-ttu-id="e2ac5-106">应用程序应实现逻辑以进行检测并恢复丢失的内容，以及恢复连续更改通知流程。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-106">Apps should implement logic to detect and recover from the loss, and resume a continuous change notification flow.</span></span>

<span data-ttu-id="e2ac5-107">某些事件可能导致订阅被删除。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-107">Certain events can cause a subscription to be removed.</span></span> <span data-ttu-id="e2ac5-108">这些事件包括：</span><span class="sxs-lookup"><span data-stu-id="e2ac5-108">These events include:</span></span>

- <span data-ttu-id="e2ac5-109">用户的密码已重置</span><span class="sxs-lookup"><span data-stu-id="e2ac5-109">User's password has been reset</span></span>
- <span data-ttu-id="e2ac5-110">用户的设备不合规</span><span class="sxs-lookup"><span data-stu-id="e2ac5-110">User's device is out of compliance</span></span>
-   <span data-ttu-id="e2ac5-111">用户的帐户已吊销</span><span class="sxs-lookup"><span data-stu-id="e2ac5-111">User's account has been revoked</span></span>

<span data-ttu-id="e2ac5-112">发生此类事件时，Microsoft Graph 将发送特殊生命周期通知，`subscriptionRemoved`。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-112">When such an event happens, Microsoft Graph sends a special lifecycle notification, `subscriptionRemoved`.</span></span>

<span data-ttu-id="e2ac5-113">如果无法将更改通知传递到应用，Microsoft Graph 还会发送另一个生命周期通知 `missed`。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-113">Microsoft Graph also sends another lifecycle notification, `missed`, if a change notification cannot be delivered to an app.</span></span>

<span data-ttu-id="e2ac5-114">订阅更改通知的应用应收听 `subscriptionRemoved` 和 `missed` 信号，并执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="e2ac5-114">An app subscribing to change notifications should listen to the `subscriptionRemoved` and `missed` signals and do the following:</span></span>

- <span data-ttu-id="e2ac5-115">收到 `subscriptionRemoved` 生命周期通知后，该应用应重新创建订阅以保持连续流程。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-115">Upon receiving a `subscriptionRemoved` lifecycle notification, the app should recreate the subscription in order to maintain a continuous flow.</span></span>
- <span data-ttu-id="e2ac5-116">收到 `missed` 生命周期通知后，该应用使用 Microsoft Graph 重新同步资源数据。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-116">On receiving a `missed` lifecycle notification, the app should resynchronize resource data using Microsoft Graph.</span></span>

<span data-ttu-id="e2ac5-117">若要接收生命周期通知，你可以使用已接收更改通知的现有 **notificationUrl** 终结点，也可以注册单独的 **lifecycleNotificationUrl** 以在单独的终结点中接收 `subscriptionRemoved` 和 `missed` 生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-117">To receive lifecycle notifications, you can use the existing **notificationUrl** endpoint that already receives change notifications, or you can register a separate **lifecycleNotificationUrl** to receive `subscriptionRemoved` and `missed` lifecycle notifications in a separate endpoint.</span></span>

<span data-ttu-id="e2ac5-118">在以下资源类型上创建的订阅支持生命周期通知：</span><span class="sxs-lookup"><span data-stu-id="e2ac5-118">Lifecycle notifications are supported for subscriptions created on these resource types:</span></span>

- <span data-ttu-id="e2ac5-119">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="e2ac5-119">Outlook [message][]</span></span>
- <span data-ttu-id="e2ac5-120">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="e2ac5-120">Outlook [event][]</span></span>
- <span data-ttu-id="e2ac5-121">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="e2ac5-121">Outlook personal [contact][]</span></span>
- <span data-ttu-id="e2ac5-122">Teams [chatMessage][]</span><span class="sxs-lookup"><span data-stu-id="e2ac5-122">Teams [chatMessage][]</span></span>

<span data-ttu-id="e2ac5-123">对于其他资源类型，在创建订阅时仍然可以提供 `lifecycleNotificationUrl`，并且只要资源实现订阅，应用程序就会收到生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-123">For other resource types, you may still provide a `lifecycleNotificationUrl` when creating the subscription and your application will receive lifecycle notifications whenever the resource implements it.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="e2ac5-124">创建订阅</span><span class="sxs-lookup"><span data-stu-id="e2ac5-124">Creating a subscription</span></span>

<span data-ttu-id="e2ac5-125">创建订阅时，你必须使用 **lifecycleNotificationUrl** 属性指定单独的通知终结点。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-125">When creating a subscription, you must specify a separate notification endpoint using the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="e2ac5-126">如果指定终结点，所有当前和未来类型的生命周期通知都将传递到那里。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-126">If you specify the endpoint, all current and future types of lifecycle notifications will be delivered there.</span></span> <span data-ttu-id="e2ac5-127">否则，将无法传递 `subscriptionRemoved` 和 `missed` 生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-127">Otherwise, `subscriptionRemoved` and `missed` lifecycle notifications will not be delivered.</span></span> <span data-ttu-id="e2ac5-128">此终结点可与 **notificationUrl** 相同。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-128">This endpoint can be the same as the **notificationUrl**.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="e2ac5-129">订阅请求示例</span><span class="sxs-lookup"><span data-stu-id="e2ac5-129">Subscription request example</span></span>

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/users/{id}/messages",
  "expirationDateTime": "2020-03-20T11:00:00.0000000Z",
  "clientState": "<secretClientState>"
}
```
 
> [!IMPORTANT]
> <span data-ttu-id="e2ac5-130">对两个通知 URL 使用相同的主机名 (FQDN)。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-130">Use the same hostname (FQDN) for both notifications URLs.</span></span> 

<span data-ttu-id="e2ac5-131">需要按照 [管理订阅](webhooks.md#managing-subscriptions)中的说明验证两个终结点。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-131">You need to validate both endpoints, as described in [Managing subscriptions](webhooks.md#managing-subscriptions).</span></span> <span data-ttu-id="e2ac5-132">如果选择针对两个终结点使用同一 URL，将收到并响应两个验证请求。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-132">If you choose to use the same URL for both endpoints, you will receive and respond to two validation requests.</span></span>

> <span data-ttu-id="e2ac5-133">**注意：** 无法更新 (`PATCH`) 现有订阅以添加 **lifecycleNotificationUrl** 属性。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-133">**Note:** You cannot update (`PATCH`) the existing subscriptions to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="e2ac5-134">应删除此类现有订阅，创建新订阅并指定 **lifecycleNotificationUrl** 属性。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-134">You should remove such existing subscriptions, create new subscriptions, and specify the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="e2ac5-135">没有 **lifecycleNotificationUrl** 属性的现有订阅将接收 `subscriptionRemoved` 和 `missed` 通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-135">Existing subscriptions without a **lifecycleNotificationUrl** property will not receive the `subscriptionRemoved` and `missed` notifications.</span></span>

## <a name="responding-to-subscriptionremoved-notifications"></a><span data-ttu-id="e2ac5-136">响应 subscriptionRemoved 通知</span><span class="sxs-lookup"><span data-stu-id="e2ac5-136">Responding to subscriptionRemoved notifications</span></span>

<span data-ttu-id="e2ac5-137">`subscriptionRemoved` 生命周期通知会通知你订阅已删除，如果想要继续接收更改通知，应重新创建。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-137">The `subscriptionRemoved` lifecycle notification informs you that a subscription has been removed and should be recreated, if you want to continue receiving change notifications.</span></span> 

<span data-ttu-id="e2ac5-138">可以创建长期订阅（3 天），更改通知将开始流向 **notificationUrl**。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-138">You can create a long-lived subscription (3 days), and change notifications will start flowing to the **notificationUrl**.</span></span> <span data-ttu-id="e2ac5-139">但是，资源数据的访问条件可能会随时间变化。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-139">However, the conditions of access to the resource data might change over time.</span></span> <span data-ttu-id="e2ac5-140">例如，服务中的事件可能会发生，需要应用程序对于用户重新进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-140">For example, an event in the service might occur that requires the app to re-authenticate the user.</span></span> <span data-ttu-id="e2ac5-141">在此类情况下，流程如下所示：</span><span class="sxs-lookup"><span data-stu-id="e2ac5-141">In such a case, the flow is as follows:</span></span>

1. <span data-ttu-id="e2ac5-142">服务检测到需要从 Microsoft Graph 删除订阅。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-142">The service detects that a subscription needs to be removed from Microsoft Graph.</span></span>
    
    <span data-ttu-id="e2ac5-143">这些事件没有固定的节奏。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-143">There is no set cadence for these events.</span></span> <span data-ttu-id="e2ac5-144">对于某些资源，它们可能经常发生，而对于其他资源，几乎永远不会发生。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-144">They might occur frequently for some resources, and almost never for others.</span></span>

2. <span data-ttu-id="e2ac5-145">Microsoft Graph 将发送 `subscriptionRemoved` 生命周期通知到 **lifecycleNotificationUrl**（如果指定）。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-145">Microsoft Graph sends a `subscriptionRemoved` lifecycle notification to the **lifecycleNotificationUrl** (if specified).</span></span>  

3. <span data-ttu-id="e2ac5-146">可以通过为同一资源创建新订阅来响应此生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-146">You can respond to this lifecycle notification by creating a new subscription for the same resource.</span></span> <span data-ttu-id="e2ac5-147">为此，你需要提供有效的访问令牌；在某些情况下，这意味着应用程序需要重新验证用户以获取新的有效访问令牌。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-147">To do this, you need to present a valid access token; in some cases, this means the app needs to re-authenticate the user to obtain a new valid access token.</span></span>

4. <span data-ttu-id="e2ac5-148">如果成功创建新订阅，更改通知将再次开始流动。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-148">If you successfully create a new subscription, change notifications will start flowing again.</span></span> <span data-ttu-id="e2ac5-149">但是，如果失败（例如，应用程序无法获取有效的访问令牌），将不会发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-149">However, if you fail (for example, the app can't obtain a valid access token), change notifications will not be sent.</span></span>

5. <span data-ttu-id="e2ac5-150">创建新订阅后，可以同步资源数据以标识任何缺失的更改。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-150">After creating the new subscription, you can sync the resource data to identify any missing changes.</span></span>

### <a name="subscriptionremoved-notification-example"></a><span data-ttu-id="e2ac5-151">subscriptionRemoved 通知示例</span><span class="sxs-lookup"><span data-stu-id="e2ac5-151">subscriptionRemoved notification example</span></span>

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

<span data-ttu-id="e2ac5-152">有关此类型通知的一些注意事项：</span><span class="sxs-lookup"><span data-stu-id="e2ac5-152">A few things to note about this type of notification:</span></span>

- <span data-ttu-id="e2ac5-153">`"lifecycleEvent": "subscriptionRemoved"` 字段将此通知指定为与订阅删除相关。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-153">The `"lifecycleEvent": "subscriptionRemoved"` field designates this notification as related to subscription removal.</span></span> <span data-ttu-id="e2ac5-154">其他类型的生命周期通知也是可能的，将来会引入新的通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-154">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="e2ac5-155">生命周期通知不包含有关特定资源的任何信息，因为它与资源更改无关，而与订阅状态更改有关。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-155">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="e2ac5-156">与更改通知类似，生命周期通知可以一起批处理（在 **值** 数组中），每个通知都有一个可能不同的 **lifecycleEvent** 值。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-156">Similar to change notifications, lifecycle notifications can be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="e2ac5-157">相应地批处理每个生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-157">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="e2ac5-158">**注意：** 有关传递更改通知时发送的数据的完整说明，请参阅 [changeNotificationCollection](/graph/api/resources/changenotificationcollection)。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-158">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="e2ac5-159">要采取的操作</span><span class="sxs-lookup"><span data-stu-id="e2ac5-159">Actions to take</span></span>

1. <span data-ttu-id="e2ac5-160">通过使用 `202 - Accepted` 来响应 POST 调用，[确认](webhooks.md#change-notifications)收到生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-160">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="e2ac5-161">[验证](webhooks.md#change-notifications)生命周期通知的真实性。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-161">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="e2ac5-162">确保应用程序具有执行下一步操作的有效访问令牌。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-162">Ensure that the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="e2ac5-163">**注意：** 如果使用其中一个 [身份验证库](/azure/active-directory/develop/reference-v2-libraries)，他们将通过重复使用有效的缓存令牌或获取新令牌，其中包括要求用户（使用新密码）再次登录来处理此问题。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-163">**Note:** If you're using one of the [authentication libraries](/azure/active-directory/develop/reference-v2-libraries), they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to sign in again (with a new password).</span></span> <span data-ttu-id="e2ac5-164">请注意，获取新令牌可能会失败，因为访问条件可能已更改，并且可能不再允许调用者访问资源数据。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-164">Note that obtaining a new token might fail, because the conditions of access might have changed, and the caller might no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="e2ac5-165">使用[此处](webhooks.md#subscription-request-example)描述的标准流程创建新订阅。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-165">Create a new subscription using the standard process described [here](webhooks.md#subscription-request-example).</span></span>

  > <span data-ttu-id="e2ac5-166">**注意：** 此操作可能会失败，因为系统执行的授权检查可能会拒绝应用程序或用户访问资源。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-166">**Note:** This action might fail, because the authorization checks performed by the system might deny the app or the user access to the resource.</span></span> <span data-ttu-id="e2ac5-167">应用程序可能需要从用户处获取新的访问令牌以成功重新授权订阅。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-167">It might be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> <span data-ttu-id="e2ac5-168">以后可以随时重试这些操作，例如，当访问条件发生变化时。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-168">You can retry these actions later, at any time; for example, when the conditions of access have changed.</span></span> <span data-ttu-id="e2ac5-169">从生命周期通知发送到应用程序成功重新创建订阅的时间段内的任何资源更改都将丢失。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-169">Any resource changes in the time period from when the lifecycle notification was sent, to when the app recreates the subscription successfully, will be lost.</span></span> <span data-ttu-id="e2ac5-170">该应用需要自己获取这些更改。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-170">The app will need to fetch those changes on its own.</span></span>

5. <span data-ttu-id="e2ac5-171">创建新订阅后，从收到此资源的更改通知的上次已知时间同步任何缺失的资源数据；例如：`GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span><span class="sxs-lookup"><span data-stu-id="e2ac5-171">After creating the new subscription, sync any missing resource data from the last known time you received a change notification for this resource; for example: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span></span>

## <a name="responding-to-missed-notifications"></a><span data-ttu-id="e2ac5-172">响应错过的通知</span><span class="sxs-lookup"><span data-stu-id="e2ac5-172">Responding to missed notifications</span></span>

<span data-ttu-id="e2ac5-173">这些信号通知你可能尚未发送某些更改通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-173">These signals inform you that some change notifications might not have been delivered.</span></span> <span data-ttu-id="e2ac5-174">你应决定是否忽略或处理这些信号。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-174">You should decide if you ignore or handle these signals.</span></span>

### <a name="notification-example"></a><span data-ttu-id="e2ac5-175">通知示例</span><span class="sxs-lookup"><span data-stu-id="e2ac5-175">Notification example</span></span>

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

<span data-ttu-id="e2ac5-176">有关此类型通知的一些注意事项：</span><span class="sxs-lookup"><span data-stu-id="e2ac5-176">A few things to note about this type of notification:</span></span>

- <span data-ttu-id="e2ac5-177">`"lifecycleEvent": "missed"` 字段将此指定为有关错过的更改通知的信号。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-177">The `"lifecycleEvent": "missed"` field designates this as a signal about missed change notifications.</span></span> <span data-ttu-id="e2ac5-178">其他类型的生命周期通知也是可能的，将来会引入新的通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-178">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="e2ac5-179">生命周期通知不包含有关特定资源的任何信息，因为它与资源更改无关，而与订阅状态更改有关。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-179">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="e2ac5-180">与更改通知类似，生命周期通知可以一起批处理（在 **值** 数组中），每个通知都有一个可能不同的 **lifecycleEvent** 值。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-180">Similar to change notifications, lifecycle notifications might be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="e2ac5-181">相应地批处理每个生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-181">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="e2ac5-182">**注意：** 有关传递更改通知时发送的数据的完整说明，请参阅 [changeNotificationCollection](/graph/api/resources/changenotificationcollection)。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-182">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="e2ac5-183">要采取的操作</span><span class="sxs-lookup"><span data-stu-id="e2ac5-183">Actions to take</span></span>

1. <span data-ttu-id="e2ac5-184">通过使用 `202 - Accepted` 来响应 POST 调用，[确认](webhooks.md#change-notifications)收到生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-184">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
    - <span data-ttu-id="e2ac5-185">如果忽略这些信号，则无需执行其他任何操作。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-185">If you ignore these signals, do nothing else.</span></span> <span data-ttu-id="e2ac5-186">或者：</span><span class="sxs-lookup"><span data-stu-id="e2ac5-186">Otherwise:</span></span>
2. <span data-ttu-id="e2ac5-187">[验证](webhooks.md#change-notifications)生命周期通知的真实性。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-187">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="e2ac5-188">执行资源的完整数据重新同步，以标识未作为通知发送的更改。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-188">Perform a full data resync of the resource to identify the changes that were not delivered as notifications.</span></span> 

## <a name="responding-to-reauthorizationrequired-notifications"></a><span data-ttu-id="e2ac5-189">响应 reauthorizationRequired 通知</span><span class="sxs-lookup"><span data-stu-id="e2ac5-189">Responding to reauthorizationRequired notifications</span></span>

<span data-ttu-id="e2ac5-190">收到`reauthorizationRequired`生命周期通知时，必须重新授权该订阅以保持数据流。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-190">When you receive a `reauthorizationRequired` lifecycle notification, you must reauthorize the subscription to maintain the data flow.</span></span>

<span data-ttu-id="e2ac5-191">可以创建长期订阅（3 天），更改通知流向 **notificationUrl**。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-191">You can create a long-lived subscription (3 days), which enables change notifications to flow to the **notificationUrl**.</span></span> <span data-ttu-id="e2ac5-192">自订阅创建起访问条件发生变化时，Microsoft Graph 可能要求你重新授权订阅，证明仍能访问资源数据。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-192">If the conditions of access have changed since the subscription was created, Microsoft Graph may require that you reauthorize the subscription to prove that you still have access to resource data.</span></span> <span data-ttu-id="e2ac5-193">下面是影响数据访问的更改示例：</span><span class="sxs-lookup"><span data-stu-id="e2ac5-193">The following are examples of changes that affect your access to data:</span></span>

- <span data-ttu-id="e2ac5-194">租户管理员可能会吊销应用程序读取资源的权限。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-194">A tenant administrator may revoke your app's permissions to read a resource.</span></span>
- <span data-ttu-id="e2ac5-195">在交互方案中，向应用程序提供身份验证令牌的用户，可能会受限于基于多种因素的动态策略，如位置、设备状态或风险评估。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-195">In an interactive scenario, the user who provides the authentication token to your app may be subject to dynamic policies based on various factors, such as their location, device state, or risk assessment.</span></span> <span data-ttu-id="e2ac5-196">例如，如果用户更改了物理位置，则该用户可能无法再访问该数据，并且应用程序无法重新授权订阅。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-196">For example, if the user changes their physical location, the user may no longer be allowed to access the data, and your app will not be able to reauthorize the subscription.</span></span> <span data-ttu-id="e2ac5-197">有关控制访问的动态策略的详细信息，请参阅 [Azure AD 条件性访问策略](/azure/active-directory/conditional-access/overview)。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-197">For more information about dynamic policies that control access, see [Azure AD conditional access policies](/azure/active-directory/conditional-access/overview).</span></span> 

<span data-ttu-id="e2ac5-198">以下步骤代表活动的订阅的授权质询流：</span><span class="sxs-lookup"><span data-stu-id="e2ac5-198">The following steps represent the flow of an authorization challenge for an active subscription:</span></span>

1. <span data-ttu-id="e2ac5-199">Microsoft Graph 需要重新授权的订阅。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-199">Microsoft Graph requires a subscription to be reauthorized.</span></span>
    
    <span data-ttu-id="e2ac5-200">发生这种情况的原因可能随资源而异，可能随着时间推移而发生变化。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-200">The reasons for this may vary from resource to resource, and may change over time.</span></span> <span data-ttu-id="e2ac5-201">无论重新授权事件如何造成的，你都必须对作出响应。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-201">You must respond to a reauthorization event no matter what caused it.</span></span>

2. <span data-ttu-id="e2ac5-202">Microsoft Graph 向 **lifecycleNotificationUrl** 发送授权质询通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-202">Microsoft Graph sends an authorization challenge notification to the **lifecycleNotificationUrl**.</span></span>

    <span data-ttu-id="e2ac5-203">请注意，更改通知流可能会持续一段时间，为你提供额外的响应时间。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-203">Note that the flow of change notifications may continue for a while, giving you extra time to respond.</span></span> <span data-ttu-id="e2ac5-204">但是更改通知传递将最终暂停，直至执行了所需操作。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-204">However, eventually change notification delivery pauses, until you take the required action.</span></span>

3. <span data-ttu-id="e2ac5-205">采用以下两种方法之一来响应此生命周期通知：</span><span class="sxs-lookup"><span data-stu-id="e2ac5-205">Respond to this lifecycle notification in one of two ways:</span></span>
    - <span data-ttu-id="e2ac5-206">重新授权订阅。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-206">Reauthorize the subscription.</span></span> <span data-ttu-id="e2ac5-207">这不会延长订阅的到期日期。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-207">This does not extend the expiry date of the subscription.</span></span>
    - <span data-ttu-id="e2ac5-208">续订订阅。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-208">Renew the subscription.</span></span> <span data-ttu-id="e2ac5-209">这将重新授权并延长到期日期。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-209">This both reauthorizes and extends the expiry date.</span></span>

    <span data-ttu-id="e2ac5-210">注意：两项操作都要求提供有效的身份验证令牌，类似于[新建订阅](webhooks.md#creating-a-subscription)或[到期前续订订阅](webhooks.md#renewing-a-subscription)。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-210">Note: Both actions require you to present a valid authentication token, similar to [creating a new subscription](webhooks.md#creating-a-subscription) or [renewing a subscription before its expiry](webhooks.md#renewing-a-subscription).</span></span>

4. <span data-ttu-id="e2ac5-211">如果成功重新授权或续订订阅，更改通知将继续。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-211">If you successfully reauthorize or renew the subscription, change notifications continue.</span></span> <span data-ttu-id="e2ac5-212">否则，更改通知保持暂停。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-212">Otherwise, change notifications remain paused.</span></span>

### <a name="reauthorizationrequired-notification-example"></a><span data-ttu-id="e2ac5-213">reauthorizationRequired 通知示例</span><span class="sxs-lookup"><span data-stu-id="e2ac5-213">reauthorizationRequired notification example</span></span>

```json
{
  "value": [
    {
      "lifecycleEvent": "reauthorizationRequired",
      "subscriptionId": "e3898f08-5cd0-4a6a-80fc-6addbfb73b7b",
      "subscriptionExpirationDateTime": "2019-09-18T00:52:45.9696658+00:00",
      "clientState": "{secret client state}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95"
    }
  ]
}
```

<span data-ttu-id="e2ac5-214">有关此类型通知的一些注意事项：</span><span class="sxs-lookup"><span data-stu-id="e2ac5-214">A few things to note about this type of notification:</span></span>

- <span data-ttu-id="e2ac5-215">“`"lifecycleEvent": "reauthorizationRequired"`”字段将通知标识为授权质询。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-215">The `"lifecycleEvent": "reauthorizationRequired"` field designates this notification as an authorization challenge.</span></span> <span data-ttu-id="e2ac5-216">其他类型的生命周期通知也是可能的，将来会引入新的通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-216">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="e2ac5-217">生命周期通知不包含有关特定资源的任何信息，因为它与资源更改无关，而与订阅状态更改有关。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-217">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="e2ac5-218">与更改通知类似，可以共同对生命周期通知进行批处理（**值** 集），各通知可能有不同的 **lifecycleEvent** 值。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-218">Similar to change notifications, you can batch lifecycle notifications together (in the **value** collection), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="e2ac5-219">相应地批处理每个生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-219">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="e2ac5-220">**注意：** 有关传递更改通知时发送的数据的完整说明，请参阅 [changeNotificationCollection](/graph/api/resources/changenotificationcollection)。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-220">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="e2ac5-221">要采取的操作</span><span class="sxs-lookup"><span data-stu-id="e2ac5-221">Actions to take</span></span>

1. <span data-ttu-id="e2ac5-222">通过使用 `202 - Accepted` 来响应 POST 调用，[确认](webhooks.md#change-notifications)收到生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-222">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="e2ac5-223">[验证](webhooks.md#change-notifications)生命周期通知的真实性。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-223">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="e2ac5-224">确保应用程序具有执行下一步操作的有效访问令牌。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-224">Ensure that the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="e2ac5-225">**注意：** 如果使用其中一个 [身份验证库](/azure/active-directory/develop/reference-v2-libraries)，他们将通过重复使用有效的缓存令牌或获取新令牌，其中包括要求用户（使用新密码）再次登录来处理此问题。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-225">**Note:** If you're using one of the [authentication libraries](/azure/active-directory/develop/reference-v2-libraries), they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to sign in again (with a new password).</span></span> <span data-ttu-id="e2ac5-226">请注意，获取新令牌可能会失败，因为访问条件可能已更改，并且可能不再允许调用者访问资源数据。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-226">Note that obtaining a new token might fail, because the conditions of access might have changed, and the caller might no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="e2ac5-227">调用下列两个API中的任意一个。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-227">Call either of the following two APIs.</span></span> <span data-ttu-id="e2ac5-228">如果 API 调用成功，则更改通知流将继续。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-228">If the API call succeeds, the change notification flow resumes.</span></span>

    - <span data-ttu-id="e2ac5-229">调用`/reauthorize`操作以重新批准订阅，但不延长到期日期：</span><span class="sxs-lookup"><span data-stu-id="e2ac5-229">Call the `/reauthorize` action to reauthorize the subscription without extending its expiration date:</span></span>
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - <span data-ttu-id="e2ac5-230">执行定期续订操作，以同时进行重新授权和续订：</span><span class="sxs-lookup"><span data-stu-id="e2ac5-230">Perform a regular renew action to reauthorize and renew the subscription at the same time:</span></span>
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      <span data-ttu-id="e2ac5-231">续订可能会失败，因为系统执行的授权检查可能会拒绝应用程序或用户对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-231">Renewing may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="e2ac5-232">应用程序可能需要从用户获取新的访问令牌以成功重新授权订阅。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-232">It may be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> 
      
      <span data-ttu-id="e2ac5-233">以后可以随时重试这些操作，例如访问条件发生变化时。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-233">You may retry these actions later, at any time, and succeed if the conditions of access change.</span></span> <span data-ttu-id="e2ac5-234">生命周期通知发送至应用再次成功重新创建订阅之间的有关资源更改的任何通知将丢失。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-234">Any notifications about resource changes that happen between the time the lifecycle notification was sent and the time when the app successfully creates the subscription again, would be lost.</span></span> <span data-ttu-id="e2ac5-235">在这种情况下，应用程序应单独获取这些更改。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-235">In such cases, the app should separately fetch those changes.</span></span>

### <a name="additional-information"></a><span data-ttu-id="e2ac5-236">其他信息</span><span class="sxs-lookup"><span data-stu-id="e2ac5-236">Additional information</span></span>

<span data-ttu-id="e2ac5-237">以下信息可帮助你了解身份验证质询：</span><span class="sxs-lookup"><span data-stu-id="e2ac5-237">The following information can help you understand authorization challenges:</span></span>

- <span data-ttu-id="e2ac5-238">授权质询不会替代到期前续订资源更改通知的需要。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-238">Authorization challenges do not replace the need to renew a resource change subscription before it expires.</span></span> 

    <span data-ttu-id="e2ac5-239">虽然可以选择在收到授权质询时续订订阅，但 Microsoft Graph 可能不会对所有订阅进行质询。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-239">While you can choose to renew a subscription when you receive an authorization challenge, Microsoft Graph may not challenge all of your subscriptions.</span></span> <span data-ttu-id="e2ac5-240">例如，没有任何活动且没有更改通知挂起传递的订阅不表示对应用有任何重新授权质询。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-240">For example, a subscription that does not have any activity and has no change notifications pending delivery may not signal any reauthorization challenges to your app.</span></span> <span data-ttu-id="e2ac5-241">请务必在订阅到期前 [续订订阅](webhooks.md#renewing-a-subscription)。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-241">Make sure to [renew subscriptions](webhooks.md#renewing-a-subscription) before they expire.</span></span>

- <span data-ttu-id="e2ac5-242">授权质询的频率可能会发生更改。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-242">The frequency of authorization challenges is subject to change.</span></span>

    <span data-ttu-id="e2ac5-243">不要对授权质询频率进行假设。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-243">Do not make assumptions about the frequency of authorization challenges.</span></span> <span data-ttu-id="e2ac5-244">这些生命周期通知会告诉你执行操作的时间，无需跟踪需要重新授权的订阅。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-244">These lifecycle notifications tell you when to take actions, saving you from having to track which subscriptions require reauthorization.</span></span> <span data-ttu-id="e2ac5-245">准备好每隔几分钟处理每个订阅的授权质询，极少情况下，只针对部分订阅。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-245">Be ready to handle authorization challenges from once every few minutes for every subscription to rarely for only some of your subscriptions.</span></span>

## <a name="future-proof-the-code-handling-lifecycle-notifications"></a><span data-ttu-id="e2ac5-246">前瞻性的代码处理生命周期通知</span><span class="sxs-lookup"><span data-stu-id="e2ac5-246">Future-proof the code handling lifecycle notifications</span></span>

<span data-ttu-id="e2ac5-247">将来，Microsoft Graph 将添加更多类型的订阅生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-247">In the future, Microsoft Graph will add more types of subscription lifecycle notifications.</span></span> <span data-ttu-id="e2ac5-248">它们将被发布到相同的终结点：**lifecycleNotificationUrl**，但是它们在 **lifecycleEvent** 下将具有不同的值，并且可能包含稍微不同的模式和属性，这些模式和属性特定于将为其发布的方案。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-248">They will be posted to the same endpoint: **lifecycleNotificationUrl**, but they will have a different value under **lifecycleEvent** and might contain a slightly different schema and properties, specific to the scenario for which they will be issued.</span></span>

<span data-ttu-id="e2ac5-249">你应该以前瞻性的方式实现代码，以便在 Microsoft Graph 引入新类型的生命周期通知时不会中断。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-249">You should implement your code in a future-proof way, so it does not break when Microsoft Graph introduces new types of lifecycle notifications.</span></span> <span data-ttu-id="e2ac5-250">建议使用以下方法：</span><span class="sxs-lookup"><span data-stu-id="e2ac5-250">We recommend the following approach:</span></span>

1. <span data-ttu-id="e2ac5-251">使用 **lifecycleEvent** 属性将每个生命周期通知显式标识为你支持的事件。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-251">Explicitly identify each lifecycle notification as an event that you support, using the **lifecycleEvent** property.</span></span> <span data-ttu-id="e2ac5-252">例如，查找 `"lifecycleEvent": "subscriptionRemoved"` 属性标识特定事件并处理它。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-252">For example, look for the `"lifecycleEvent": "subscriptionRemoved"` property to identify a specific event, and handle it.</span></span>

2. <span data-ttu-id="e2ac5-253">注意有关新方案的生命周期通知公告。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-253">Watch for announcements of lifecycle notifications for new scenarios.</span></span> <span data-ttu-id="e2ac5-254">将来可能会有更多类型的生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-254">There might be more types of lifecycle notifications in the future.</span></span>

3. <span data-ttu-id="e2ac5-255">在你的应用中，忽略应用无法识别的任何生命周期通知，并记录它们以获得认知。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-255">In your app, ignore any lifecycle notification that the app does not recognize, and log them to gain awareness.</span></span>

4. <span data-ttu-id="e2ac5-256">你可以自行决定查找新生命周期通知的相关文档，并根据需要实施对它们的支持。</span><span class="sxs-lookup"><span data-stu-id="e2ac5-256">At your discretion, look up the related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="see-also"></a><span data-ttu-id="e2ac5-257">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e2ac5-257">See also</span></span>

- [<span data-ttu-id="e2ac5-258">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="e2ac5-258">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="e2ac5-259">获取订阅</span><span class="sxs-lookup"><span data-stu-id="e2ac5-259">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="e2ac5-260">创建订阅</span><span class="sxs-lookup"><span data-stu-id="e2ac5-260">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="e2ac5-261">删除订阅</span><span class="sxs-lookup"><span data-stu-id="e2ac5-261">Delete subscription</span></span>](/graph/api/subscription-delete?view=graph-rest-1.0)
- [<span data-ttu-id="e2ac5-262">更新订阅</span><span class="sxs-lookup"><span data-stu-id="e2ac5-262">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)


[联系人]: /graph/api/resources/contact?view=graph-rest-1.0
[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[chatMessage]: /graph/api/resources/chatmessage
