---
title: 通知资源类型
description: '表示由面向指定用户的应用服务器发布的通知。 通知存储在 Microsoft Graph 中，并分发到用户拥有的不同设备终结点。 '
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: abd17119e80e4e8a7967197356811ee519d813ba
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159449"
---
# <a name="notification-resource-type"></a><span data-ttu-id="141d0-104">通知资源类型</span><span class="sxs-lookup"><span data-stu-id="141d0-104">notification resource type</span></span>

<span data-ttu-id="141d0-105">命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="141d0-105">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="141d0-106">表示由面向指定用户的应用服务器发布的通知。</span><span class="sxs-lookup"><span data-stu-id="141d0-106">Represents a notification that is published by an app server that targets a specified user.</span></span> <span data-ttu-id="141d0-107">通知存储在 Microsoft Graph 中，并分发到用户拥有的不同设备终结点。</span><span class="sxs-lookup"><span data-stu-id="141d0-107">The notification is stored in Microsoft Graph and is distributed to different device endpoints owned by the user.</span></span> 

<span data-ttu-id="141d0-108">通知可以是可视通知有效负载，操作系统可以在 Windows、Android 和 iOS (解释该负载) 。</span><span class="sxs-lookup"><span data-stu-id="141d0-108">A notification can be a visual notification payload that can be interpreted by the operating system (Windows, Android, and iOS platforms).</span></span> <span data-ttu-id="141d0-109">它还可以是传递到应用客户端 ( (（) 包括 Web) ）并处理的 rawContent) 的数据负载，然后确定每台设备上相应的用户体验。</span><span class="sxs-lookup"><span data-stu-id="141d0-109">It can also be a data payload (rawContent) that's delivered to and handled by app clients (including web), which then determine the corresponding user experience on each device.</span></span>  <span data-ttu-id="141d0-110">这通常是本地生成的可视通知 UI，对应于原始数据负载中的内容。</span><span class="sxs-lookup"><span data-stu-id="141d0-110">This is usually a visual notification UI, generated locally, that corresponds to the content in the original data payload.</span></span> 

<span data-ttu-id="141d0-111">当用户对可视通知操作时，应用客户端随后可以使用客户端通知 SDK 更新 Microsoft Graph 中相应通知源的状态，例如，通过将通知标记为已消除。</span><span class="sxs-lookup"><span data-stu-id="141d0-111">When a user acts on a visual notification, the app client can then use the client-side notifications SDK to update the state of the corresponding notification feed in Microsoft Graph - for example, by marking a notification as dismissed.</span></span> <span data-ttu-id="141d0-112">然后，更新将分发到所有其他应用客户端终结点，客户端会相应地处理更改，例如通过消除通知来阻止用户看到冗余信息。</span><span class="sxs-lookup"><span data-stu-id="141d0-112">The update will then be distributed to all other app client endpoints, and the clients handle the change accordingly, for example by dismissing the notification to prevent the user from seeing redundant information.</span></span> <span data-ttu-id="141d0-113">应用客户端可以在过期前稍后访问同一通知资源 (即使通过通知 SDK 将通知) 标记为已取消，也作为通知 [历史记录](https://aka.ms/GNSDK)。</span><span class="sxs-lookup"><span data-stu-id="141d0-113">App clients can access the same notification resource at a later time before it expires (even after it is marked as dismissed), as notification history, via the [notification SDK](https://aka.ms/GNSDK).</span></span> 

> [!NOTE]
> <span data-ttu-id="141d0-114">通知状态更新（如读取或消除）不会扇出到 Web 终结点。</span><span class="sxs-lookup"><span data-stu-id="141d0-114">Notification state updates, such as read or dismissed, will not be fanned out to web endpoints.</span></span> <span data-ttu-id="141d0-115">这是因为跨各种浏览器的 Web 推送需要向用户显示可视 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="141d0-115">This is because web pushes across various browsers require visual toast notifications to be displayed to a user.</span></span> <span data-ttu-id="141d0-116">由于状态更改没有相应的可视内容，因此它们只会针对面向 Windows、iOS 或 Android 平台的通知扇出。</span><span class="sxs-lookup"><span data-stu-id="141d0-116">Because state changes have no corresponding visual content, they will only be fanned-out for notifications targeting Windows, iOS, or Android platforms.</span></span>

## <a name="methods"></a><span data-ttu-id="141d0-117">方法</span><span class="sxs-lookup"><span data-stu-id="141d0-117">Methods</span></span>
|<span data-ttu-id="141d0-118">方法</span><span class="sxs-lookup"><span data-stu-id="141d0-118">Method</span></span> | <span data-ttu-id="141d0-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="141d0-119">Return Type</span></span> | <span data-ttu-id="141d0-120">说明</span><span class="sxs-lookup"><span data-stu-id="141d0-120">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="141d0-121">创建通知</span><span class="sxs-lookup"><span data-stu-id="141d0-121">Create notification</span></span>](../api/user-post-notifications.md) | [<span data-ttu-id="141d0-122">notification</span><span class="sxs-lookup"><span data-stu-id="141d0-122">notification</span></span>](projectrome-notification.md) |<span data-ttu-id="141d0-123">创建并发送通知。</span><span class="sxs-lookup"><span data-stu-id="141d0-123">Create and send a notification.</span></span> |

## <a name="properties"></a><span data-ttu-id="141d0-124">属性</span><span class="sxs-lookup"><span data-stu-id="141d0-124">Properties</span></span>
|<span data-ttu-id="141d0-125">名称</span><span class="sxs-lookup"><span data-stu-id="141d0-125">Name</span></span> | <span data-ttu-id="141d0-126">类型</span><span class="sxs-lookup"><span data-stu-id="141d0-126">Type</span></span> | <span data-ttu-id="141d0-127">说明</span><span class="sxs-lookup"><span data-stu-id="141d0-127">Description</span></span>|
|:----|:-----|:-----------|
| <span data-ttu-id="141d0-128">targetHostName</span><span class="sxs-lookup"><span data-stu-id="141d0-128">targetHostName</span></span> | <span data-ttu-id="141d0-129">String</span><span class="sxs-lookup"><span data-stu-id="141d0-129">String</span></span> | <span data-ttu-id="141d0-130">表示调用服务要向其中发布通知的应用的主机名（针对给定用户）。</span><span class="sxs-lookup"><span data-stu-id="141d0-130">Represents the host name of the app to which the calling service wants to post the notification, for the given user.</span></span> <span data-ttu-id="141d0-131">如果面向 Web 终结点 (请参阅 **targetPolicy.platformTypes**) ，请确保 **targetHostName** 与在应用程序 JSON 属性内的客户端上创建订阅时所使用的名称相同。</span><span class="sxs-lookup"><span data-stu-id="141d0-131">If targeting web endpoints (see **targetPolicy.platformTypes**), ensure that **targetHostName** is the same as the name used when creating a subscription on the client side within the application JSON property.</span></span> |
| <span data-ttu-id="141d0-132">appNotificationId</span><span class="sxs-lookup"><span data-stu-id="141d0-132">appNotificationId</span></span> | <span data-ttu-id="141d0-133">String</span><span class="sxs-lookup"><span data-stu-id="141d0-133">String</span></span> | <span data-ttu-id="141d0-134">应用服务器设置的唯一 ID，用于标识和定位单个通知的通知。</span><span class="sxs-lookup"><span data-stu-id="141d0-134">The unique ID set by the app server of a notification that is used to identify and target an individual notification.</span></span> |
| <span data-ttu-id="141d0-135">groupName</span><span class="sxs-lookup"><span data-stu-id="141d0-135">groupName</span></span> | <span data-ttu-id="141d0-136">String</span><span class="sxs-lookup"><span data-stu-id="141d0-136">String</span></span> | <span data-ttu-id="141d0-137">此通知所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="141d0-137">The name of the group that this notification belongs to.</span></span> <span data-ttu-id="141d0-138">它由开发人员设置，用于将通知分组在一起。</span><span class="sxs-lookup"><span data-stu-id="141d0-138">It is set by the developer for the purpose of grouping notifications together.</span></span> |
| <span data-ttu-id="141d0-139">targetPolicy</span><span class="sxs-lookup"><span data-stu-id="141d0-139">targetPolicy</span></span> | [<span data-ttu-id="141d0-140">targetPolicyEndpoints</span><span class="sxs-lookup"><span data-stu-id="141d0-140">targetPolicyEndpoints</span></span>](targetpolicyendpoints.md) | <span data-ttu-id="141d0-141">目标策略对象处理应面向给定用户的 (Windows、iOS、Android 和 WebPush) 类型的通知传递策略。</span><span class="sxs-lookup"><span data-stu-id="141d0-141">Target policy object handles notification delivery policy for endpoint types that should be targeted (Windows, iOS, Android and WebPush) for the given user.</span></span> |
| <span data-ttu-id="141d0-142">payload</span><span class="sxs-lookup"><span data-stu-id="141d0-142">payload</span></span> | [<span data-ttu-id="141d0-143">payloadTypes</span><span class="sxs-lookup"><span data-stu-id="141d0-143">payloadTypes</span></span>](payloadtypes.md)| <span data-ttu-id="141d0-144">这是原始或可视用户通知的数据内容，将传递给接收此通知的应用客户端，并供应用客户端使用。</span><span class="sxs-lookup"><span data-stu-id="141d0-144">This is the data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> |
| <span data-ttu-id="141d0-145">displayTimeToLive</span><span class="sxs-lookup"><span data-stu-id="141d0-145">displayTimeToLive</span></span> | <span data-ttu-id="141d0-146">Int32</span><span class="sxs-lookup"><span data-stu-id="141d0-146">Int32</span></span> | <span data-ttu-id="141d0-147">设置此 (内容在每个平台的通知查看器中) 持续多久（以秒表示）。</span><span class="sxs-lookup"><span data-stu-id="141d0-147">Sets how long (in seconds) this notification content will stay in each platform’s notification viewer.</span></span> <span data-ttu-id="141d0-148">例如，当通知传递到 Windows 设备时，此属性的值将传递到 ToastNotification.ExpirationTime，这将确定 Toast 通知将在用户的 Windows 操作中心中停留的时间。</span><span class="sxs-lookup"><span data-stu-id="141d0-148">For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification will stay in the user’s Windows Action Center.</span></span> |
| <span data-ttu-id="141d0-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="141d0-149">expirationDateTime</span></span> | <span data-ttu-id="141d0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="141d0-150">DateTimeOffset</span></span> | <span data-ttu-id="141d0-151">使用 ISO 8601 格式设置用户通知的 UTC 过期日期和时间 (例如，2019 年 1 月 1 日午夜 UTC 如下所示 `'2019-01-01T00:00:00Z'` ：) 。</span><span class="sxs-lookup"><span data-stu-id="141d0-151">Sets a UTC expiration date and time on a user notification using ISO 8601 format (for example, midnight UTC on Jan 1, 2019 would look like this: `'2019-01-01T00:00:00Z'`).</span></span> <span data-ttu-id="141d0-152">时间开始后，通知将从 Microsoft Graph 通知源存储中完全删除，并且不再属于通知历史记录。</span><span class="sxs-lookup"><span data-stu-id="141d0-152">When time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.</span></span> <span data-ttu-id="141d0-153">最大值为 30 天。</span><span class="sxs-lookup"><span data-stu-id="141d0-153">Max value is 30 days.</span></span> |
| <span data-ttu-id="141d0-154">priority</span><span class="sxs-lookup"><span data-stu-id="141d0-154">priority</span></span> | <span data-ttu-id="141d0-155">string</span><span class="sxs-lookup"><span data-stu-id="141d0-155">string</span></span> | <span data-ttu-id="141d0-156">指示原始用户通知的优先级。</span><span class="sxs-lookup"><span data-stu-id="141d0-156">Indicates the priority of a raw user notification.</span></span> <span data-ttu-id="141d0-157">默认情况下，以高优先级发送视觉通知。</span><span class="sxs-lookup"><span data-stu-id="141d0-157">Visual notifications are sent with high priority by default.</span></span> <span data-ttu-id="141d0-158">有效值为 `None`、`High` 和 `Low`。</span><span class="sxs-lookup"><span data-stu-id="141d0-158">Valid values are `None`, `High` and `Low`.</span></span> |
| <span data-ttu-id="141d0-159">fallbackPolicy</span><span class="sxs-lookup"><span data-stu-id="141d0-159">fallbackPolicy</span></span> | [<span data-ttu-id="141d0-160">fallbackpolicy</span><span class="sxs-lookup"><span data-stu-id="141d0-160">fallbackpolicy</span></span>](fallbackpolicy.md) | <span data-ttu-id="141d0-161">可选回退策略对象仅处理 iOS 终结点的通知回退策略，旨在用于由于特定于平台的限制（例如节电模式 () ）而可能无法传递到设备的高优先级原始通知。</span><span class="sxs-lookup"><span data-stu-id="141d0-161">Optional fallback policy object handles notification fallback policy for iOS endpoints only and is designed to be used for high-priority raw notifications that might not be delivered to devices due to platform specific restrictions (e.g. battery saver mode).</span></span> |


## <a name="relationships"></a><span data-ttu-id="141d0-162">关系</span><span class="sxs-lookup"><span data-stu-id="141d0-162">Relationships</span></span>
<span data-ttu-id="141d0-163">无。</span><span class="sxs-lookup"><span data-stu-id="141d0-163">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="141d0-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="141d0-164">JSON representation</span></span>
<span data-ttu-id="141d0-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="141d0-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notification",
  "keyProperty": "id"
}-->

```json
{
  "targetHostName": "String",
  "appNotificationid": "String (identifier)",
  "groupName": "String", 
  "targetPolicy": {"@odata.type": "microsoft.graph.targetPolicyEndpoints"},
  "payload": {"@odata.type": "microsoft.graph.payloadTypes"},
  "displayTimeToLive": 1024,
  "expirationDateTime": "String (timestamp)",
  "priority": "string",
  "fallbackPolicy": {"@odata.type": "microsoft.graph.fallbackpolicy"},  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


