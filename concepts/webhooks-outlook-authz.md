---
title: 减少 Outlook 资源丢失订阅和通知（预览版）
description: 由于用户密码重置等安全事件，Outlook 可能会暂停传递更改通知。 需要处理特殊生命周期事件（`subscriptionRemoved` 和 `missed`），以确保传递通知不间断。
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 481dbee58a5ee761816e05c88d44e115da736035
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216838"
---
# <a name="reduce-missing-subscriptions-and-notifications-for-outlook-resources-preview"></a><span data-ttu-id="60d73-104">减少 Outlook 资源丢失订阅和通知（预览版）</span><span class="sxs-lookup"><span data-stu-id="60d73-104">Reduce missing subscriptions and notifications for Outlook resources (preview)</span></span> 

<span data-ttu-id="60d73-105">订阅 Outlook 资源通知的应用程序可能会删除其订阅并错过一些通知。</span><span class="sxs-lookup"><span data-stu-id="60d73-105">Apps subscribing to notifications for Outlook resources may get their subscriptions removed and miss some notifications.</span></span> <span data-ttu-id="60d73-106">应用程序应实现逻辑以进行检测并恢复丢失的内容，以及恢复连续通知流程。</span><span class="sxs-lookup"><span data-stu-id="60d73-106">Apps should implement logic to detect and recover from the loss, and resume a continuous notification flow.</span></span>

<span data-ttu-id="60d73-107">Outlook 中的某些事件可能导致订阅被删除。</span><span class="sxs-lookup"><span data-stu-id="60d73-107">Certain events in Outlook can cause a subscription to be removed.</span></span> <span data-ttu-id="60d73-108">这些事件包括：</span><span class="sxs-lookup"><span data-stu-id="60d73-108">These events include:</span></span>

- <span data-ttu-id="60d73-109">用户的密码已重置</span><span class="sxs-lookup"><span data-stu-id="60d73-109">User's password has been reset</span></span>
- <span data-ttu-id="60d73-110">用户的设备不合规</span><span class="sxs-lookup"><span data-stu-id="60d73-110">User's device is out of compliance</span></span>
-   <span data-ttu-id="60d73-111">用户的帐户已吊销</span><span class="sxs-lookup"><span data-stu-id="60d73-111">User's account has been revoked</span></span>

<span data-ttu-id="60d73-112">发生此类事件时，Outlook 将发送特殊生命周期通知 `subscriptionRemoved`。</span><span class="sxs-lookup"><span data-stu-id="60d73-112">When such an event happens, Outlook sends a special lifecycle notification, `subscriptionRemoved`.</span></span>

<span data-ttu-id="60d73-113">如果无法将通知传递到应用程序，Outlook 还会发送另一个生命周期通知 `missed`。</span><span class="sxs-lookup"><span data-stu-id="60d73-113">Outlook also sends another lifecycle notification, `missed`, if a notification cannot be delivered to an app.</span></span>

<span data-ttu-id="60d73-114">订阅 Outlook 资源通知的应用程序（如**邮件**和**事件**）应收听 `subscriptionRemoved` 和 `missed` 信号，并执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="60d73-114">An app subscribing to notifications for Outlook resources, such as **message** and **event**, should listen to the `subscriptionRemoved` and `missed` signals:</span></span>

- <span data-ttu-id="60d73-115">收到 `subscriptionRemoved` 通知后，该应用程序应重新创建订阅以保持连续流程。</span><span class="sxs-lookup"><span data-stu-id="60d73-115">Upon receiving a `subscriptionRemoved` notification, the app should recreate the subscription in order to maintain a continuous flow.</span></span>
- <span data-ttu-id="60d73-116">收到 `missed` 通知后，该应用使用 Microsoft Graph 重新同步资源数据。</span><span class="sxs-lookup"><span data-stu-id="60d73-116">On receiving a `missed` notification, the app should resynchronize resource data using Microsoft Graph.</span></span>

<span data-ttu-id="60d73-117">若要接收生命周期通知，可以使用已接收资源通知的现有 **notificationUrl** 终结点，也可以注册单独的 **lifecycleNotificationUrl** 以在单独的终结点中接收 `subscriptionRemoved` 和 `missed` 通知。</span><span class="sxs-lookup"><span data-stu-id="60d73-117">To receive lifecycle notifications, you can use the existing **notificationUrl** endpoint that already receives resource notifications, or you can register a separate **lifecycleNotificationUrl** to receive `subscriptionRemoved` and `missed` notifications in a separate endpoint.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="60d73-118">创建订阅</span><span class="sxs-lookup"><span data-stu-id="60d73-118">Creating a subscription</span></span>

<span data-ttu-id="60d73-119">创建订阅时，你可以使用 **lifecycleNotificationUrl** 属性指定单独的通知终结点。</span><span class="sxs-lookup"><span data-stu-id="60d73-119">When creating a subscription, you can specify a separate notification endpoint using the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="60d73-120">如果指定终结点，所有当前和未来类型的生命周期通知都将传递到那里。</span><span class="sxs-lookup"><span data-stu-id="60d73-120">If you specify the endpoint, all current and future types of lifecycle notifications will be delivered there.</span></span> <span data-ttu-id="60d73-121">否则，`subscriptionRemoved` 和 `missed` 通知都将传递到所有现有订阅的现有 **notificationUrl**。</span><span class="sxs-lookup"><span data-stu-id="60d73-121">Otherwise, `subscriptionRemoved` and `missed` notifications will be delivered to the existing **notificationUrl** for all existing subscriptions.</span></span>

> <span data-ttu-id="60d73-122">**注意：** 只能使用 Microsoft Graph beta API 设置或读取 **lifecycleNotificationUrl** 属性。</span><span class="sxs-lookup"><span data-stu-id="60d73-122">**Note:** At the moment, the **lifecycleNotificationUrl** property can only be set or read using the  version of Microsoft Graph APIs.</span></span> <span data-ttu-id="60d73-123">但是，使用 beta API 创建的订阅与使用 v1.0 创建的订阅存储在同一个生产环境中，因此除了使用 v1.0 API 创建的订阅外，还可以实现新 Outlook 流程。</span><span class="sxs-lookup"><span data-stu-id="60d73-123">However, subscriptions created using beta APIs are stored in the same production environment as those created using v1.0, so you can implement the new Outlook flow in addition to your subscriptions creating using v1.0 APIs.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="60d73-124">订阅请求示例</span><span class="sxs-lookup"><span data-stu-id="60d73-124">Subscription request example</span></span>

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
 
> <span data-ttu-id="60d73-125">**重要提示：** 对两个通知 URL 使用相同的主机名。</span><span class="sxs-lookup"><span data-stu-id="60d73-125">**Important:** Use the same hostname for both notifications URLs.</span></span> 

> <span data-ttu-id="60d73-126">**注意：** 需要按照[管理订阅](webhooks.md#managing-subscriptions)中的说明验证两个通知终结点。</span><span class="sxs-lookup"><span data-stu-id="60d73-126">**Note:** You need to validate both notification endpoints as described in [the generic notification article](webhooks.md#managing-subscriptions).</span></span>
<span data-ttu-id="60d73-127">如果选择对两个终结点使用相同的 URL，将收到并响应两个验证请求。</span><span class="sxs-lookup"><span data-stu-id="60d73-127">If you choose to use the same URL for both endpoints you will receive and respond to two validation requests.</span></span>

> <span data-ttu-id="60d73-128">**注意：** 无法更新 (`PATCH`) 现有订阅以添加 **lifecycleNotificationUrl** 属性。</span><span class="sxs-lookup"><span data-stu-id="60d73-128">**Note:** You cannot update (`PATCH`) the existing subscriptions to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="60d73-129">应删除此类现有订阅，创建新订阅并指定 **lifecycleNotificationUrl** 属性。</span><span class="sxs-lookup"><span data-stu-id="60d73-129">You should remove such existing subscriptions, and create new subscriptions and specify the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="60d73-130">没有 **lifecycleNotificationUrl** 属性的现有订阅将通过 **notificationUrl** 接收 `subscriptionRemoved` 和 `missed` 通知。</span><span class="sxs-lookup"><span data-stu-id="60d73-130">Existing subscriptions without **lifecycleNotificationUrl** property will receive the `subscriptionRemoved` and `missed` notifications via the **notificationUrl**.</span></span> 

## <a name="responding-to-subscriptionremoved-notifications"></a><span data-ttu-id="60d73-131">响应 subscriptionRemoved 通知</span><span class="sxs-lookup"><span data-stu-id="60d73-131">Responding to subscriptionRemoved notifications</span></span>

<span data-ttu-id="60d73-132">`subscriptionRemoved` 通知会通知你订阅已删除，如果想要继续接收通知，应重新创建。</span><span class="sxs-lookup"><span data-stu-id="60d73-132">The `subscriptionRemoved` notification informs you that a subscription has been removed and should be recreated, if you want to continue receiving notifications.</span></span> 

<span data-ttu-id="60d73-133">可以创建长期订阅（3 天），资源数据通知将开始流向 **notificationUrl**。</span><span class="sxs-lookup"><span data-stu-id="60d73-133">You can create a long-lived subscription (e.g. 3 days), and resource data notifications will start flowing to the **notificationUrl**.</span></span> <span data-ttu-id="60d73-134">但是，资源数据的访问条件可能会随时间变化。</span><span class="sxs-lookup"><span data-stu-id="60d73-134">However, the conditions of access to the resource data may change over time.</span></span> <span data-ttu-id="60d73-135">例如，Outlook 服务中的事件可能会发生，需要应用程序对于用户重新进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="60d73-135">For example, an event in the Outlook service may occur that requires the app to re-authenticate the user.</span></span> <span data-ttu-id="60d73-136">在此类情况下，流程如下所示：</span><span class="sxs-lookup"><span data-stu-id="60d73-136">In such a case, the flow looks as follows:</span></span>

1. <span data-ttu-id="60d73-137">Outlook 检测到需要从 Microsoft Graph 删除订阅。</span><span class="sxs-lookup"><span data-stu-id="60d73-137">Outlook detects that a subscription needs to be removed from Microsoft Graph.</span></span>
    
    <span data-ttu-id="60d73-138">这些事件没有固定的节奏。</span><span class="sxs-lookup"><span data-stu-id="60d73-138">There is no set cadence for these events.</span></span> <span data-ttu-id="60d73-139">对于某些资源，它们可能经常发生，而对于其他资源，几乎永远不会发生。</span><span class="sxs-lookup"><span data-stu-id="60d73-139">They may occur frequently for some resources, and almost never for others.</span></span>

2. <span data-ttu-id="60d73-140">Microsoft Graph 将发送 `subscriptionRemoved` 通知到 **lifecycleNotificationUrl**（如果指定）或 **notificationUrl**。</span><span class="sxs-lookup"><span data-stu-id="60d73-140">Microsoft Graph sends a `subscriptionRemoved` notification to the **lifecycleNotificationUrl** (if specified), or the **notificationUrl**.</span></span>  

3. <span data-ttu-id="60d73-141">可以通过为同一资源创建新订阅来响应此通知。</span><span class="sxs-lookup"><span data-stu-id="60d73-141">You can respond to this notification by creating a new subscription for the same resource.</span></span> <span data-ttu-id="60d73-142">为此，你需要提供有效的访问令牌；在某些情况下，这意味着应用程序需要重新验证用户以获取新的有效访问令牌。</span><span class="sxs-lookup"><span data-stu-id="60d73-142">To do this, you need to present a valid access token; in some cases this means the app needs to re-authenticate the user to obtain a new valid access token.</span></span>

4. <span data-ttu-id="60d73-143">如果成功创建新订阅，资源通知将再次开始流动。</span><span class="sxs-lookup"><span data-stu-id="60d73-143">If you successfully create a new subscription, resource notifications will start flowing again.</span></span> <span data-ttu-id="60d73-144">但是，如果失败（例如，应用程序无法获取有效的访问令牌），将不会发送资源通知。</span><span class="sxs-lookup"><span data-stu-id="60d73-144">However, if you fail (for example, the app could not obtain a valid access token), resource notifications will not be sent.</span></span>

5. <span data-ttu-id="60d73-145">创建新订阅后，可以同步资源数据以标识任何缺失的更改。</span><span class="sxs-lookup"><span data-stu-id="60d73-145">After creating the new subscription, you can sync the resource data to identify any missing changes.</span></span>

### <a name="subscriptionremoved-notification-example"></a><span data-ttu-id="60d73-146">subscriptionRemoved 通知示例</span><span class="sxs-lookup"><span data-stu-id="60d73-146">subscriptionRemoved notification example</span></span>

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

<span data-ttu-id="60d73-147">有关此类型通知的一些注意事项：</span><span class="sxs-lookup"><span data-stu-id="60d73-147">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="60d73-148">`"lifecycleEvent": "subscriptionRemoved"` 字段将此通知指定为与订阅删除相关。</span><span class="sxs-lookup"><span data-stu-id="60d73-148">The `"lifecycleEvent": "subscriptionRemoved"` field designates this notification as related to subscription removal.</span></span> <span data-ttu-id="60d73-149">其他类型的生命周期通知也是可能的，将来会引入新的通知。</span><span class="sxs-lookup"><span data-stu-id="60d73-149">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="60d73-150">通知不包含有关特定资源的任何信息，因为它与资源更改无关，而与订阅状态更改有关。</span><span class="sxs-lookup"><span data-stu-id="60d73-150">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="60d73-151">与资源通知类似，生命周期通知可以一起批处理（在**值**数组中），每个通知都有一个可能不同的 **lifecycleEvent** 值。</span><span class="sxs-lookup"><span data-stu-id="60d73-151">Similar to resource notifications, lifecycle notifications may be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="60d73-152">相应地批处理每个通知。</span><span class="sxs-lookup"><span data-stu-id="60d73-152">Process each notification in the batch accordingly.</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="60d73-153">要采取的操作</span><span class="sxs-lookup"><span data-stu-id="60d73-153">Actions to take</span></span>

1. <span data-ttu-id="60d73-154">通过使用 `202 - Accepted` 响应 POST 调用[确认](webhooks.md#notifications)收到通知。</span><span class="sxs-lookup"><span data-stu-id="60d73-154">[Acknowledge](webhooks.md#notifications) the receipt of the notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="60d73-155">[验证](webhooks.md#notifications)通知的真实性。</span><span class="sxs-lookup"><span data-stu-id="60d73-155">[Validate](webhooks.md#notifications) the authenticity of the notification.</span></span>
3. <span data-ttu-id="60d73-156">确保应用程序具有执行下一步操作的有效访问令牌。</span><span class="sxs-lookup"><span data-stu-id="60d73-156">Ensure the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="60d73-157">**注意：** 如果使用其中一个[身份验证库](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)，他们将通过重复使用有效的缓存令牌或获取新令牌，其中包括要求用户（使用新密码）再次登录来处理此问题。</span><span class="sxs-lookup"><span data-stu-id="60d73-157">**Note:** If you are using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to login again (e.g. with a new password).</span></span> <span data-ttu-id="60d73-158">请注意，获取新令牌可能会失败，因为访问条件可能已更改，并且可能不再允许调用者访问资源数据。</span><span class="sxs-lookup"><span data-stu-id="60d73-158">Note that obtaining a new token may fail, since the conditions of access may have changed, and the caller may no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="60d73-159">使用[此处](webhooks.md#subscription-request-example)描述的标准流程创建新订阅。</span><span class="sxs-lookup"><span data-stu-id="60d73-159">Create a new subscription using the standard process described [here](webhooks.md#subscription-request-example).</span></span>

  > <span data-ttu-id="60d73-160">**注意：** 此操作可能会失败，因为系统执行的授权检查可能会拒绝应用程序或用户访问资源。</span><span class="sxs-lookup"><span data-stu-id="60d73-160">**Note:** This action may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="60d73-161">应用程序可能需要从用户处获取新的访问令牌以成功重新授权订阅。</span><span class="sxs-lookup"><span data-stu-id="60d73-161">It may be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> <span data-ttu-id="60d73-162">以后可以随时重试这些操作，例如，当访问条件发生变化时。</span><span class="sxs-lookup"><span data-stu-id="60d73-162">You may retry these actions later, at any time, for example when the conditions of access have change.</span></span> <span data-ttu-id="60d73-163">从生命周期通知发送到应用程序成功重新创建订阅的时间段内的任何资源更改都将丢失。</span><span class="sxs-lookup"><span data-stu-id="60d73-163">Any resource changes in the time period from when the lifecycle notification was sent, to when the app re-creates the subscription successfully, will be lost.</span></span> <span data-ttu-id="60d73-164">该应用程序需要自己获取这些更改。</span><span class="sxs-lookup"><span data-stu-id="60d73-164">The app will need to fetch those changes on its own.</span></span>

5. <span data-ttu-id="60d73-165">创建新订阅后，从收到此资源通知的上次已知时间同步任何缺失的资源数据；例如：`GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span><span class="sxs-lookup"><span data-stu-id="60d73-165">After creating the new subscription, sync any missing resource data from the last known time you received a notification for this resource; for example: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span></span>

## <a name="responding-to-missed-notifications"></a><span data-ttu-id="60d73-166">响应错过的通知</span><span class="sxs-lookup"><span data-stu-id="60d73-166">Responding to missed notifications</span></span>

<span data-ttu-id="60d73-167">这些信号通知你可能尚未发送某些通知。</span><span class="sxs-lookup"><span data-stu-id="60d73-167">These signals inform you that some notifications may have not been delivered.</span></span> <span data-ttu-id="60d73-168">你应决定是否忽略或处理这些信号。</span><span class="sxs-lookup"><span data-stu-id="60d73-168">You should decide if you ignore or handle these signals.</span></span>

### <a name="notification-example"></a><span data-ttu-id="60d73-169">通知示例</span><span class="sxs-lookup"><span data-stu-id="60d73-169">Notification example</span></span>

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

<span data-ttu-id="60d73-170">有关此类型通知的一些注意事项：</span><span class="sxs-lookup"><span data-stu-id="60d73-170">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="60d73-171">`"lifecycleEvent": "missed"` 字段将此指定为有关错过的通知的信号。</span><span class="sxs-lookup"><span data-stu-id="60d73-171">The `"lifecycleEvent": "missed"` field designates this as a signal about missed notifications.</span></span> <span data-ttu-id="60d73-172">其他类型的生命周期通知也是可能的，将来会引入新的通知。</span><span class="sxs-lookup"><span data-stu-id="60d73-172">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="60d73-173">通知不包含有关特定资源的任何信息，因为它与资源更改无关，而与订阅状态更改有关。</span><span class="sxs-lookup"><span data-stu-id="60d73-173">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="60d73-174">与资源通知类似，生命周期通知可以一起批处理（在**值**数组中），每个通知都有一个可能不同的 **lifecycleEvent** 值。</span><span class="sxs-lookup"><span data-stu-id="60d73-174">Similar to resource notifications, lifecycle notifications may be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="60d73-175">相应地批处理每个通知。</span><span class="sxs-lookup"><span data-stu-id="60d73-175">Process each notification in the batch accordingly.</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="60d73-176">要采取的操作</span><span class="sxs-lookup"><span data-stu-id="60d73-176">Actions to take</span></span>

1. <span data-ttu-id="60d73-177">通过使用 `202 - Accepted` 响应 POST 调用[确认](webhooks.md#notifications)收到通知。</span><span class="sxs-lookup"><span data-stu-id="60d73-177">[Acknowledge](webhooks.md#notifications) the receipt of the notification, by responding to the POST call with `202 - Accepted`.</span></span>
    - <span data-ttu-id="60d73-178">如果忽略这些信号，则无需执行其他任何操作。</span><span class="sxs-lookup"><span data-stu-id="60d73-178">If you ignore these, signals, do nothing else.</span></span> <span data-ttu-id="60d73-179">或者：</span><span class="sxs-lookup"><span data-stu-id="60d73-179">Otherwise:</span></span>
2. <span data-ttu-id="60d73-180">[验证](webhooks.md#notifications)通知的真实性。</span><span class="sxs-lookup"><span data-stu-id="60d73-180">[Validate](webhooks.md#notifications) the authenticity of the notification.</span></span>
3. <span data-ttu-id="60d73-181">执行资源的完整数据重新同步，以标识未作为通知发送的更改。</span><span class="sxs-lookup"><span data-stu-id="60d73-181">Perform a full data resync of the resource to identify the changes that were not delivered as notifications.</span></span> 


## <a name="future-proof-the-code-handling-life-cycle-notifications"></a><span data-ttu-id="60d73-182">前瞻性的代码处理生命周期通知</span><span class="sxs-lookup"><span data-stu-id="60d73-182">Future-proof the code handling lifecycle notifications</span></span>

<span data-ttu-id="60d73-183">将来，Microsoft Graph 将添加更多类型的订阅生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="60d73-183">In the future Microsoft Graph will add more types of subscription lifecycle notifications.</span></span> <span data-ttu-id="60d73-184">它们将被发布到相同的终结点：**lifecycleNotificationUrl**，但是它们在 **lifecycleEvent** 下将具有不同的值，并且可能包含稍微不同的模式和属性，这些模式和属性特定于将为其发布的方案。</span><span class="sxs-lookup"><span data-stu-id="60d73-184">They will be posted to the same endpoint: **lifecycleNotificationUrl**, but they will have a different value under **lifecycleEvent** and may contain a slightly different schema and properties, specific to the scenario for which they will be issued.</span></span>

<span data-ttu-id="60d73-185">应以前瞻性的方式实现代码，以便在 Microsoft Graph 引入新类型的生命周期通知时不会中断。</span><span class="sxs-lookup"><span data-stu-id="60d73-185">You should implement your code in a future-proof way so it does not break when Microsoft Graph introduces new types of lifecycle notifications.</span></span> <span data-ttu-id="60d73-186">建议使用以下方法：</span><span class="sxs-lookup"><span data-stu-id="60d73-186">We recommend the following approach:</span></span>

1. <span data-ttu-id="60d73-187">使用 **lifecycleEvent** 属性将每个通知显式标识为你支持的事件。</span><span class="sxs-lookup"><span data-stu-id="60d73-187">Explicitly identify each notification as an event that you support, using the **lifecycleEvent** property.</span></span> <span data-ttu-id="60d73-188">例如，查找 `"lifecycleEvent": "subscriptionRemoved"` 属性标识特定事件并处理它。</span><span class="sxs-lookup"><span data-stu-id="60d73-188">For example, look for the `"lifecycleEvent": "subscriptionRemoved"` property to identify a specific event, and handle it.</span></span>

2. <span data-ttu-id="60d73-189">注意有关新方案的通知公告。</span><span class="sxs-lookup"><span data-stu-id="60d73-189">Watch for announcements of notifications for new scenarions.</span></span> <span data-ttu-id="60d73-190">将来可能会有更多类型的生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="60d73-190">There might be more types of life cycle notifications in the future.</span></span>

3. <span data-ttu-id="60d73-191">在你的应用程序中，忽略应用程序无法识别的任何生命周期事件，并记录它们以引起重视。</span><span class="sxs-lookup"><span data-stu-id="60d73-191">In your app, ignore any lifecycle events that the app does not recognize, and log them to gain awareness.</span></span>

4. <span data-ttu-id="60d73-192">可以自行决定查找新生命周期通知的相关文档，并根据需要提供支持。</span><span class="sxs-lookup"><span data-stu-id="60d73-192">At your discretion, look up the related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="see-also"></a><span data-ttu-id="60d73-193">另请参阅</span><span class="sxs-lookup"><span data-stu-id="60d73-193">See also</span></span>

- [<span data-ttu-id="60d73-194">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="60d73-194">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="60d73-195">获取订阅</span><span class="sxs-lookup"><span data-stu-id="60d73-195">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="60d73-196">创建订阅</span><span class="sxs-lookup"><span data-stu-id="60d73-196">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="60d73-197">删除订阅</span><span class="sxs-lookup"><span data-stu-id="60d73-197">Delete subscription</span></span>](/graph/api/subscription-delete?view=graph-rest-1.0)
- [<span data-ttu-id="60d73-198">更新订阅</span><span class="sxs-lookup"><span data-stu-id="60d73-198">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
