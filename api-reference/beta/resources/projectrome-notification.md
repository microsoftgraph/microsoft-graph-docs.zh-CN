---
title: 通知资源类型
description: '代表由指定的用户的目标应用程序服务器发布的通知。 通知存储在 Microsoft Graph 中并分发到不同设备用户所拥有的终结点。 '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: af130c9806511b0afbdaedb602790c7c40d3ca2e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509257"
---
# <a name="notification-resource-type"></a><span data-ttu-id="5fb68-104">通知资源类型</span><span class="sxs-lookup"><span data-stu-id="5fb68-104">notification resource type</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fb68-105">代表由指定的用户的目标应用程序服务器发布的通知。</span><span class="sxs-lookup"><span data-stu-id="5fb68-105">Represents a notification that is published by an app server that targets a specified user.</span></span> <span data-ttu-id="5fb68-106">通知存储在 Microsoft Graph 中并分发到不同设备用户所拥有的终结点。</span><span class="sxs-lookup"><span data-stu-id="5fb68-106">The notification is stored in Microsoft Graph and is distributed to different device endpoints owned by the user.</span></span> 

<span data-ttu-id="5fb68-107">通知可以是可由操作系统，包括 Windows、 Android 和 iOS 平台解释 visual 通知负载。</span><span class="sxs-lookup"><span data-stu-id="5fb68-107">A notification can be a visual notification payload that can be interpreted by the operating system, including Windows, Android, and iOS platforms.</span></span> <span data-ttu-id="5fb68-108">也可以是数据负载的已送达和处理应用程序的客户端，然后确定相应的用户体验上每个设备 – 通常情况下，visual 通知对应于中生成的原始数据有效负载的内容的 UI本地。</span><span class="sxs-lookup"><span data-stu-id="5fb68-108">It can also be a data payload that's delivered to and handled by app clients, which then determine the corresponding user experience on each device – usually, a visual notification UI that corresponds to the content in the original data payload that's generated locally.</span></span> 

<span data-ttu-id="5fb68-109">当用户对 visual 通知时，应用程序客户端然后可以使用客户端项目 Rome SDK 更新的源中 Microsoft Graph-例如，通过将通知标记为消除相应通知状态。</span><span class="sxs-lookup"><span data-stu-id="5fb68-109">When a user acts on a visual notification, the app client can then use client-side Project Rome SDK to update the state of the corresponding notification feed in Microsoft Graph - for example, by marking a notification as dismissed.</span></span> <span data-ttu-id="5fb68-110">更新将随后可分配给所有其他应用程序客户端终结点，并在客户端更改据此处理，例如通过消除该通知以防止用户看到冗余信息。</span><span class="sxs-lookup"><span data-stu-id="5fb68-110">The update will then be distributed to all other app client endpoints, and the clients handle the change accordingly, for example by dismissing the notification to prevent the user from seeing redundant information.</span></span> <span data-ttu-id="5fb68-111">应用程序客户端可以在以后到期 （即使该被标记为消除） 之前, 访问相同的通知资源作为通知历史记录，通过[Project Rome SDK](https://github.com/Microsoft/project-rome)。</span><span class="sxs-lookup"><span data-stu-id="5fb68-111">App clients can access the same notification resource at a later time before it expires (even after it is marked as dismissed), as notification history, via the [Project Rome SDK](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="methods"></a><span data-ttu-id="5fb68-112">方法</span><span class="sxs-lookup"><span data-stu-id="5fb68-112">Methods</span></span>
|<span data-ttu-id="5fb68-113">方法</span><span class="sxs-lookup"><span data-stu-id="5fb68-113">Method</span></span> | <span data-ttu-id="5fb68-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="5fb68-114">Return Type</span></span> | <span data-ttu-id="5fb68-115">说明</span><span class="sxs-lookup"><span data-stu-id="5fb68-115">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="5fb68-116">创建通知</span><span class="sxs-lookup"><span data-stu-id="5fb68-116">Create notification</span></span>](../api/projectrome-notification-post.md) | <span data-ttu-id="5fb68-117">通知</span><span class="sxs-lookup"><span data-stu-id="5fb68-117">[notification](projectrome-notification.md)</span></span> |<span data-ttu-id="5fb68-118">创建和发送通知。</span><span class="sxs-lookup"><span data-stu-id="5fb68-118">Create and send a notification.</span></span> |

## <a name="properties"></a><span data-ttu-id="5fb68-119">属性</span><span class="sxs-lookup"><span data-stu-id="5fb68-119">Properties</span></span>
|<span data-ttu-id="5fb68-120">名称</span><span class="sxs-lookup"><span data-stu-id="5fb68-120">Name</span></span> | <span data-ttu-id="5fb68-121">类型</span><span class="sxs-lookup"><span data-stu-id="5fb68-121">Type</span></span> | <span data-ttu-id="5fb68-122">说明</span><span class="sxs-lookup"><span data-stu-id="5fb68-122">Description</span></span>|
|:----|:-----|:-----------|
| <span data-ttu-id="5fb68-123">targetHostName</span><span class="sxs-lookup"><span data-stu-id="5fb68-123">targetHostName</span></span> | <span data-ttu-id="5fb68-124">String</span><span class="sxs-lookup"><span data-stu-id="5fb68-124">String</span></span> | <span data-ttu-id="5fb68-125">代表调用服务希望发布的给定用户的通知应用程序的主机名。</span><span class="sxs-lookup"><span data-stu-id="5fb68-125">Represents the host name of the app to which the calling service wants to post the notification, for the given user.</span></span> |
| <span data-ttu-id="5fb68-126">appNotificationId</span><span class="sxs-lookup"><span data-stu-id="5fb68-126">appNotificationId</span></span> | <span data-ttu-id="5fb68-127">String</span><span class="sxs-lookup"><span data-stu-id="5fb68-127">String</span></span> | <span data-ttu-id="5fb68-128">设置用于标识和目标单个通知的通知的应用程序服务器的唯一 id。</span><span class="sxs-lookup"><span data-stu-id="5fb68-128">The unique id set by the app server of a notification that is used to identify and target an individual notification.</span></span> |
| <span data-ttu-id="5fb68-129">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5fb68-129">expirationDateTime</span></span> | <span data-ttu-id="5fb68-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fb68-130">DateTimeOffset</span></span> | <span data-ttu-id="5fb68-131">设置 UTC 过期时间用户通知的时间时，通知已从 Microsoft Graph 通知源存储完全并且不再通知历史记录的一部分。</span><span class="sxs-lookup"><span data-stu-id="5fb68-131">Sets a UTC expiration time on a user notification - when time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.</span></span> <span data-ttu-id="5fb68-132">最大值为 30 天。</span><span class="sxs-lookup"><span data-stu-id="5fb68-132">Max value is 30 days.</span></span> |
| <span data-ttu-id="5fb68-133">payload</span><span class="sxs-lookup"><span data-stu-id="5fb68-133">payload</span></span> | <span data-ttu-id="5fb68-134">Edm.ComplexType，JSON 对象</span><span class="sxs-lookup"><span data-stu-id="5fb68-134">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="5fb68-135">这是将传递到和使用应用程序客户端接收该通知的原始或 visual 用户通知的数据内容。</span><span class="sxs-lookup"><span data-stu-id="5fb68-135">This is the data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> |
| <span data-ttu-id="5fb68-136">payload.rawContent</span><span class="sxs-lookup"><span data-stu-id="5fb68-136">payload.rawContent</span></span> | <span data-ttu-id="5fb68-137">String</span><span class="sxs-lookup"><span data-stu-id="5fb68-137">String</span></span> | <span data-ttu-id="5fb68-138">将传递到和使用应用程序客户端接收该通知的原始用户通知通知内容。</span><span class="sxs-lookup"><span data-stu-id="5fb68-138">The notification content of a raw user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> <span data-ttu-id="5fb68-139">至少一个 Payload.RawContent 和 Payload.VisualContent 需要有效 POST 通知请求。</span><span class="sxs-lookup"><span data-stu-id="5fb68-139">At least one of Payload.RawContent and Payload.VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="5fb68-140">payload.visual</span><span class="sxs-lookup"><span data-stu-id="5fb68-140">payload.visual</span></span> | <span data-ttu-id="5fb68-141">Edm.ComplexType，JSON 对象</span><span class="sxs-lookup"><span data-stu-id="5fb68-141">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="5fb68-142">Visual 可视化用户通知，其中将使用每个移动平台上的通知平台和呈现的用户的内容。</span><span class="sxs-lookup"><span data-stu-id="5fb68-142">The visual content of a visual user notification, which will be consumed by the notification platform on each mobile platform and rendered for the users.</span></span> <span data-ttu-id="5fb68-143">至少一个内容和 VisualContent 需要有效 POST 通知请求。</span><span class="sxs-lookup"><span data-stu-id="5fb68-143">At least one of Content and VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="5fb68-144">payload.visual.title</span><span class="sxs-lookup"><span data-stu-id="5fb68-144">payload.visual.title</span></span> | <span data-ttu-id="5fb68-145">String</span><span class="sxs-lookup"><span data-stu-id="5fb68-145">String</span></span> | <span data-ttu-id="5fb68-146">可视化用户通知的标题。</span><span class="sxs-lookup"><span data-stu-id="5fb68-146">The title of a visual user notification.</span></span> <span data-ttu-id="5fb68-147">必须具有标题或正文。</span><span class="sxs-lookup"><span data-stu-id="5fb68-147">Must have either title or body.</span></span> |
| <span data-ttu-id="5fb68-148">payload.visual.body</span><span class="sxs-lookup"><span data-stu-id="5fb68-148">payload.visual.body</span></span> | <span data-ttu-id="5fb68-149">String</span><span class="sxs-lookup"><span data-stu-id="5fb68-149">String</span></span> | <span data-ttu-id="5fb68-150">可视化用户通知的正文。</span><span class="sxs-lookup"><span data-stu-id="5fb68-150">The body of a visual user notification.</span></span> <span data-ttu-id="5fb68-151">必须具有标题或正文。</span><span class="sxs-lookup"><span data-stu-id="5fb68-151">Must have either title or body.</span></span> |
| <span data-ttu-id="5fb68-152">displayTimeToLive</span><span class="sxs-lookup"><span data-stu-id="5fb68-152">displayTimeToLive</span></span> | <span data-ttu-id="5fb68-153">Int</span><span class="sxs-lookup"><span data-stu-id="5fb68-153">Int</span></span> | <span data-ttu-id="5fb68-154">设置多长时间 （以秒为单位） 此通知内容将保持在每个平台通知查看器中。</span><span class="sxs-lookup"><span data-stu-id="5fb68-154">Sets how long (in seconds) this notification content will stay in each platform’s notification viewer.</span></span> <span data-ttu-id="5fb68-155">例如，通知传递到 Windows 设备，此属性的值被传递到 ToastNotification.ExpirationTime，确定长吐司通知将保持在用户的 Windows 操作中心。</span><span class="sxs-lookup"><span data-stu-id="5fb68-155">For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification will stay in the user’s Windows Action Center.</span></span> |
| <span data-ttu-id="5fb68-156">priority</span><span class="sxs-lookup"><span data-stu-id="5fb68-156">priority</span></span> | <span data-ttu-id="5fb68-157">EnumType</span><span class="sxs-lookup"><span data-stu-id="5fb68-157">EnumType</span></span> | <span data-ttu-id="5fb68-158">指示原始用户通知的优先级。</span><span class="sxs-lookup"><span data-stu-id="5fb68-158">Indicates the priority of a raw user notification.</span></span> <span data-ttu-id="5fb68-159">默认情况下，visual 通知发送高优先级。</span><span class="sxs-lookup"><span data-stu-id="5fb68-159">Visual notifications are sent with high priority by default.</span></span> <span data-ttu-id="5fb68-160">有效值为上限和下限。</span><span class="sxs-lookup"><span data-stu-id="5fb68-160">Valid values are High and Low.</span></span> |
| <span data-ttu-id="5fb68-161">GroupName</span><span class="sxs-lookup"><span data-stu-id="5fb68-161">groupName</span></span> | <span data-ttu-id="5fb68-162">String</span><span class="sxs-lookup"><span data-stu-id="5fb68-162">String</span></span> | <span data-ttu-id="5fb68-163">此通知所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="5fb68-163">The name of the group that this notification belongs to.</span></span> <span data-ttu-id="5fb68-164">它通过将通知组合在一起以开发人员进行设置。</span><span class="sxs-lookup"><span data-stu-id="5fb68-164">It is set by the developer for the purpose of grouping notifications together.</span></span> |
| <span data-ttu-id="5fb68-165">targetPolicy</span><span class="sxs-lookup"><span data-stu-id="5fb68-165">targetPolicy</span></span> | <span data-ttu-id="5fb68-166">Edm.ComplexType，JSON 对象</span><span class="sxs-lookup"><span data-stu-id="5fb68-166">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="5fb68-167">目标策略对象处理在两个不同级别的目标应该的终结点类型 （Windows、 iOS 和 Android） 和特定的终结点 （由订阅 id 标识） 的目标应该通知传递策略。</span><span class="sxs-lookup"><span data-stu-id="5fb68-167">Target policy object handles notification delivery policy at two different levels - endpoint types (Windows, iOS and Android) that should be targeted, and specific endpoints (identified by subscription ids) that should be targeted.</span></span> |
| <span data-ttu-id="5fb68-168">targetPolicy.platformTypes</span><span class="sxs-lookup"><span data-stu-id="5fb68-168">targetPolicy.platformTypes</span></span> | <span data-ttu-id="5fb68-169">Edm.ComplexType，集合 (EnumType)</span><span class="sxs-lookup"><span data-stu-id="5fb68-169">Edm.ComplexType, Collection (EnumType)</span></span> | <span data-ttu-id="5fb68-170">用于筛选通知分发给特定平台或平台。</span><span class="sxs-lookup"><span data-stu-id="5fb68-170">Use to filter the notification distribution to a specific platform or platforms.</span></span> <span data-ttu-id="5fb68-171">默认情况下，启用所有推送终结点类型 （iOS、 Windows 和 Android）。</span><span class="sxs-lookup"><span data-stu-id="5fb68-171">By default, all push endpoint types (iOS, Windows, and Android) are enabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5fb68-172">关系</span><span class="sxs-lookup"><span data-stu-id="5fb68-172">Relationships</span></span>
<span data-ttu-id="5fb68-173">无。</span><span class="sxs-lookup"><span data-stu-id="5fb68-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fb68-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5fb68-174">JSON representation</span></span>
<span data-ttu-id="5fb68-175">下面是资源的当您发布送达目标操作系统的直接可视化通知的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fb68-175">The following is a JSON representation of the resource when you publish a direct visual notification that is delivered to the destination operating system.</span></span>

```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "visualContent": 
    {
      "title": "String",
      "body": "String"
    },
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```

<span data-ttu-id="5fb68-176">下面是资源的当您发布传递到应用程序客户端的原始数据通知的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fb68-176">The following is a JSON representation of the resource when you publish a raw data notification that is delivered to app clients.</span></span>
```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "rawContent": "String"
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-notification.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
