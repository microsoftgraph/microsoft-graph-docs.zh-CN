---
title: 通知资源类型
description: '表示由面向指定用户的应用程序服务器发布的通知。 通知存储在 Microsoft Graph 中，并分发给用户拥有的不同设备终结点。 '
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: 2b72c55d7159f44fbc368acda9c431ef96be3905
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521402"
---
# <a name="notification-resource-type"></a><span data-ttu-id="0abe3-104">通知资源类型</span><span class="sxs-lookup"><span data-stu-id="0abe3-104">notification resource type</span></span>

<span data-ttu-id="0abe3-105">命名空间： microsoft. graph[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="0abe3-105">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="0abe3-106">表示由面向指定用户的应用程序服务器发布的通知。</span><span class="sxs-lookup"><span data-stu-id="0abe3-106">Represents a notification that is published by an app server that targets a specified user.</span></span> <span data-ttu-id="0abe3-107">通知存储在 Microsoft Graph 中，并分发给用户拥有的不同设备终结点。</span><span class="sxs-lookup"><span data-stu-id="0abe3-107">The notification is stored in Microsoft Graph and is distributed to different device endpoints owned by the user.</span></span> 

<span data-ttu-id="0abe3-108">通知可以是操作系统（Windows、Android 和 iOS 平台）可解释的视觉通知负载。</span><span class="sxs-lookup"><span data-stu-id="0abe3-108">A notification can be a visual notification payload that can be interpreted by the operating system (Windows, Android, and iOS platforms).</span></span> <span data-ttu-id="0abe3-109">它还可以是由应用程序客户端（包括 web）传递和处理的数据有效负载（rawContent），然后在每个设备上确定相应的用户体验。</span><span class="sxs-lookup"><span data-stu-id="0abe3-109">It can also be a data payload (rawContent) that's delivered to and handled by app clients (including web), which then determine the corresponding user experience on each device.</span></span>  <span data-ttu-id="0abe3-110">这通常是本地生成的 visual 通知 UI，与原始数据有效负载中的内容相对应。</span><span class="sxs-lookup"><span data-stu-id="0abe3-110">This is usually a visual notification UI, generated locally, that corresponds to the content in the original data payload.</span></span> 

<span data-ttu-id="0abe3-111">当用户在视觉通知中进行操作时，应用程序客户端可以使用客户端通知 SDK 更新 Microsoft Graph 中相应通知源的状态（例如，通过将通知标记为已关闭）。</span><span class="sxs-lookup"><span data-stu-id="0abe3-111">When a user acts on a visual notification, the app client can then use the client-side notifications SDK to update the state of the corresponding notification feed in Microsoft Graph - for example, by marking a notification as dismissed.</span></span> <span data-ttu-id="0abe3-112">然后，该更新将分发到所有其他应用程序客户端终结点，客户端将相应地处理更改，例如，通过关闭通知阻止用户查看冗余信息。</span><span class="sxs-lookup"><span data-stu-id="0abe3-112">The update will then be distributed to all other app client endpoints, and the clients handle the change accordingly, for example by dismissing the notification to prevent the user from seeing redundant information.</span></span> <span data-ttu-id="0abe3-113">应用程序客户端可以在过期之前（甚至在将其标记为 "已解除" 时）访问相同的通知资源，这是通过[通知 SDK](https://aka.ms/GNSDK)的通知历史记录。</span><span class="sxs-lookup"><span data-stu-id="0abe3-113">App clients can access the same notification resource at a later time before it expires (even after it is marked as dismissed), as notification history, via the [notification SDK](https://aka.ms/GNSDK).</span></span> 

> [!NOTE]
> <span data-ttu-id="0abe3-114">通知状态更新（如 "已读" 或 "已消除"）将不会扇到 web 终结点。</span><span class="sxs-lookup"><span data-stu-id="0abe3-114">Notification state updates, such as read or dismissed, will not be fanned out to web endpoints.</span></span> <span data-ttu-id="0abe3-115">这是因为跨不同浏览器的 web 推送需要向用户显示可视 toast 通知。</span><span class="sxs-lookup"><span data-stu-id="0abe3-115">This is because web pushes across various browsers require visual toast notifications to be displayed to a user.</span></span> <span data-ttu-id="0abe3-116">由于状态更改没有对应的可视化内容，因此将仅扇针对 Windows、iOS 或 Android 平台的通知。</span><span class="sxs-lookup"><span data-stu-id="0abe3-116">Because state changes have no corresponding visual content, they will only be fanned-out for notifications targeting Windows, iOS, or Android platforms.</span></span>

## <a name="methods"></a><span data-ttu-id="0abe3-117">方法</span><span class="sxs-lookup"><span data-stu-id="0abe3-117">Methods</span></span>
|<span data-ttu-id="0abe3-118">方法</span><span class="sxs-lookup"><span data-stu-id="0abe3-118">Method</span></span> | <span data-ttu-id="0abe3-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="0abe3-119">Return Type</span></span> | <span data-ttu-id="0abe3-120">说明</span><span class="sxs-lookup"><span data-stu-id="0abe3-120">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="0abe3-121">创建通知</span><span class="sxs-lookup"><span data-stu-id="0abe3-121">Create notification</span></span>](../api/user-post-notifications.md) | [<span data-ttu-id="0abe3-122">通告</span><span class="sxs-lookup"><span data-stu-id="0abe3-122">notification</span></span>](projectrome-notification.md) |<span data-ttu-id="0abe3-123">创建并发送通知。</span><span class="sxs-lookup"><span data-stu-id="0abe3-123">Create and send a notification.</span></span> |

## <a name="properties"></a><span data-ttu-id="0abe3-124">属性</span><span class="sxs-lookup"><span data-stu-id="0abe3-124">Properties</span></span>
|<span data-ttu-id="0abe3-125">名称</span><span class="sxs-lookup"><span data-stu-id="0abe3-125">Name</span></span> | <span data-ttu-id="0abe3-126">类型</span><span class="sxs-lookup"><span data-stu-id="0abe3-126">Type</span></span> | <span data-ttu-id="0abe3-127">说明</span><span class="sxs-lookup"><span data-stu-id="0abe3-127">Description</span></span>|
|:----|:-----|:-----------|
| <span data-ttu-id="0abe3-128">targetHostName</span><span class="sxs-lookup"><span data-stu-id="0abe3-128">targetHostName</span></span> | <span data-ttu-id="0abe3-129">String</span><span class="sxs-lookup"><span data-stu-id="0abe3-129">String</span></span> | <span data-ttu-id="0abe3-130">表示呼叫服务要为其发布通知的应用程序的主机名（针对给定用户）。</span><span class="sxs-lookup"><span data-stu-id="0abe3-130">Represents the host name of the app to which the calling service wants to post the notification, for the given user.</span></span> <span data-ttu-id="0abe3-131">如果将 web 终结点作为目标（请参阅**targetPolicy**），请确保**targetHostName**与在应用程序 JSON 属性中的客户端创建订阅时使用的名称相同。</span><span class="sxs-lookup"><span data-stu-id="0abe3-131">If targeting web endpoints (see **targetPolicy.platformTypes**), ensure that **targetHostName** is the same as the name used when creating a subscription on the client side within the application JSON property.</span></span> |
| <span data-ttu-id="0abe3-132">appNotificationId</span><span class="sxs-lookup"><span data-stu-id="0abe3-132">appNotificationId</span></span> | <span data-ttu-id="0abe3-133">String</span><span class="sxs-lookup"><span data-stu-id="0abe3-133">String</span></span> | <span data-ttu-id="0abe3-134">通知的应用程序服务器设置的唯一 ID，用于标识和定位单个通知。</span><span class="sxs-lookup"><span data-stu-id="0abe3-134">The unique ID set by the app server of a notification that is used to identify and target an individual notification.</span></span> |
| <span data-ttu-id="0abe3-135">名</span><span class="sxs-lookup"><span data-stu-id="0abe3-135">groupName</span></span> | <span data-ttu-id="0abe3-136">String</span><span class="sxs-lookup"><span data-stu-id="0abe3-136">String</span></span> | <span data-ttu-id="0abe3-137">此通知所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="0abe3-137">The name of the group that this notification belongs to.</span></span> <span data-ttu-id="0abe3-138">它由开发人员设置，用于将通知分组在一起。</span><span class="sxs-lookup"><span data-stu-id="0abe3-138">It is set by the developer for the purpose of grouping notifications together.</span></span> |
| <span data-ttu-id="0abe3-139">targetPolicy</span><span class="sxs-lookup"><span data-stu-id="0abe3-139">targetPolicy</span></span> | [<span data-ttu-id="0abe3-140">targetPolicyEndpoints</span><span class="sxs-lookup"><span data-stu-id="0abe3-140">targetPolicyEndpoints</span></span>](targetpolicyendpoints.md) | <span data-ttu-id="0abe3-141">目标策略对象处理应针对的终结点类型（Windows、iOS、Android 和 WebPush）的通知传递策略（针对给定用户）。</span><span class="sxs-lookup"><span data-stu-id="0abe3-141">Target policy object handles notification delivery policy for endpoint types that should be targeted (Windows, iOS, Android and WebPush) for the given user.</span></span> |
| <span data-ttu-id="0abe3-142">payload</span><span class="sxs-lookup"><span data-stu-id="0abe3-142">payload</span></span> | [<span data-ttu-id="0abe3-143">payloadTypes</span><span class="sxs-lookup"><span data-stu-id="0abe3-143">payloadTypes</span></span>](payloadtypes.md)| <span data-ttu-id="0abe3-144">这是原始或直观的用户通知的数据内容，这些通知将传递给应用客户端接收此通知并由其使用。</span><span class="sxs-lookup"><span data-stu-id="0abe3-144">This is the data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> |
| <span data-ttu-id="0abe3-145">displayTimeToLive</span><span class="sxs-lookup"><span data-stu-id="0abe3-145">displayTimeToLive</span></span> | <span data-ttu-id="0abe3-146">Int32</span><span class="sxs-lookup"><span data-stu-id="0abe3-146">Int32</span></span> | <span data-ttu-id="0abe3-147">设置此通知内容将在每个平台的通知查看器中保留多长时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="0abe3-147">Sets how long (in seconds) this notification content will stay in each platform’s notification viewer.</span></span> <span data-ttu-id="0abe3-148">例如，将通知传递给 Windows 设备时，此属性的值将传递给 ToastNotification，以确定 toast 通知将在用户的 Windows 操作中心保留多长时间。</span><span class="sxs-lookup"><span data-stu-id="0abe3-148">For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification will stay in the user’s Windows Action Center.</span></span> |
| <span data-ttu-id="0abe3-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0abe3-149">expirationDateTime</span></span> | <span data-ttu-id="0abe3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0abe3-150">DateTimeOffset</span></span> | <span data-ttu-id="0abe3-151">使用 ISO 8601 格式为用户通知设置 UTC 过期日期和时间（例如，1月1日午夜 UTC，2019将如下所示： `'2019-01-01T00:00:00Z'`）。</span><span class="sxs-lookup"><span data-stu-id="0abe3-151">Sets a UTC expiration date and time on a user notification using ISO 8601 format (for example, midnight UTC on Jan 1, 2019 would look like this: `'2019-01-01T00:00:00Z'`).</span></span> <span data-ttu-id="0abe3-152">当时间启动时，通知将从 Microsoft Graph 通知源存储中完全删除，并且不再是通知历史记录的一部分。</span><span class="sxs-lookup"><span data-stu-id="0abe3-152">When time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.</span></span> <span data-ttu-id="0abe3-153">最大值为30天。</span><span class="sxs-lookup"><span data-stu-id="0abe3-153">Max value is 30 days.</span></span> |
| <span data-ttu-id="0abe3-154">priority</span><span class="sxs-lookup"><span data-stu-id="0abe3-154">priority</span></span> | <span data-ttu-id="0abe3-155">string</span><span class="sxs-lookup"><span data-stu-id="0abe3-155">string</span></span> | <span data-ttu-id="0abe3-156">指示原始用户通知的优先级。</span><span class="sxs-lookup"><span data-stu-id="0abe3-156">Indicates the priority of a raw user notification.</span></span> <span data-ttu-id="0abe3-157">默认情况下，视觉通知以高优先级发送。</span><span class="sxs-lookup"><span data-stu-id="0abe3-157">Visual notifications are sent with high priority by default.</span></span> <span data-ttu-id="0abe3-158">有效值为 `None`、`High` 和 `Low`。</span><span class="sxs-lookup"><span data-stu-id="0abe3-158">Valid values are `None`, `High` and `Low`.</span></span> |
| <span data-ttu-id="0abe3-159">fallbackPolicy</span><span class="sxs-lookup"><span data-stu-id="0abe3-159">fallbackPolicy</span></span> | [<span data-ttu-id="0abe3-160">fallbackPolicy</span><span class="sxs-lookup"><span data-stu-id="0abe3-160">fallbackPolicy</span></span>](fallbackpolicy.md) | <span data-ttu-id="0abe3-161">可选回退策略对象仅处理 iOS 终结点的通知回退策略，旨在用于由于特定于平台的限制而无法发送到设备的高优先级原始通知（例如节电模式）。</span><span class="sxs-lookup"><span data-stu-id="0abe3-161">Optional fallback policy object handles notification fallback policy for iOS endpoints only and is designed to be used for high-priority raw notifications that might not be delivered to devices due to platform specific restrictions (e.g. battery saver mode).</span></span> |


## <a name="relationships"></a><span data-ttu-id="0abe3-162">关系</span><span class="sxs-lookup"><span data-stu-id="0abe3-162">Relationships</span></span>
<span data-ttu-id="0abe3-163">无。</span><span class="sxs-lookup"><span data-stu-id="0abe3-163">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0abe3-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0abe3-164">JSON representation</span></span>
<span data-ttu-id="0abe3-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0abe3-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notification",
  "baseType": "",
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
