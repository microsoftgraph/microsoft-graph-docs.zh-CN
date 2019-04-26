---
title: 通知资源类型
description: '表示由面向指定用户的应用程序服务器发布的通知。 通知存储在 Microsoft Graph 中, 并分发给用户拥有的不同设备终结点。 '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: af130c9806511b0afbdaedb602790c7c40d3ca2e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563324"
---
# <a name="notification-resource-type"></a><span data-ttu-id="80134-104">通知资源类型</span><span class="sxs-lookup"><span data-stu-id="80134-104">notification resource type</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80134-105">表示由面向指定用户的应用程序服务器发布的通知。</span><span class="sxs-lookup"><span data-stu-id="80134-105">Represents a notification that is published by an app server that targets a specified user.</span></span> <span data-ttu-id="80134-106">通知存储在 Microsoft Graph 中, 并分发给用户拥有的不同设备终结点。</span><span class="sxs-lookup"><span data-stu-id="80134-106">The notification is stored in Microsoft Graph and is distributed to different device endpoints owned by the user.</span></span> 

<span data-ttu-id="80134-107">通知可以是操作系统可解释的可视化通知有效负载, 包括 Windows、Android 和 iOS 平台。</span><span class="sxs-lookup"><span data-stu-id="80134-107">A notification can be a visual notification payload that can be interpreted by the operating system, including Windows, Android, and iOS platforms.</span></span> <span data-ttu-id="80134-108">它还可以是应用程序客户端传递和处理的数据有效负载, 然后在每个设备上确定相应的用户体验–通常是与生成的原始数据有效负载中的内容相对应的可视化通知 UIsmu.</span><span class="sxs-lookup"><span data-stu-id="80134-108">It can also be a data payload that's delivered to and handled by app clients, which then determine the corresponding user experience on each device – usually, a visual notification UI that corresponds to the content in the original data payload that's generated locally.</span></span> 

<span data-ttu-id="80134-109">当用户在视觉通知中进行操作时, 应用程序客户端可以使用客户端 Project 罗马 SDK 更新 Microsoft Graph 中相应通知源的状态, 例如, 将通知标记为已关闭。</span><span class="sxs-lookup"><span data-stu-id="80134-109">When a user acts on a visual notification, the app client can then use client-side Project Rome SDK to update the state of the corresponding notification feed in Microsoft Graph - for example, by marking a notification as dismissed.</span></span> <span data-ttu-id="80134-110">然后, 该更新将分发到所有其他应用程序客户端终结点, 客户端将相应地处理更改, 例如, 通过关闭通知阻止用户查看冗余信息。</span><span class="sxs-lookup"><span data-stu-id="80134-110">The update will then be distributed to all other app client endpoints, and the clients handle the change accordingly, for example by dismissing the notification to prevent the user from seeing redundant information.</span></span> <span data-ttu-id="80134-111">应用程序客户端可以在过期之前 (甚至在将其标记为解除标记时) 访问相同的通知资源, 这是通过[Project 罗马 SDK](https://github.com/Microsoft/project-rome)的通知历史记录。</span><span class="sxs-lookup"><span data-stu-id="80134-111">App clients can access the same notification resource at a later time before it expires (even after it is marked as dismissed), as notification history, via the [Project Rome SDK](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="methods"></a><span data-ttu-id="80134-112">方法</span><span class="sxs-lookup"><span data-stu-id="80134-112">Methods</span></span>
|<span data-ttu-id="80134-113">方法</span><span class="sxs-lookup"><span data-stu-id="80134-113">Method</span></span> | <span data-ttu-id="80134-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="80134-114">Return Type</span></span> | <span data-ttu-id="80134-115">说明</span><span class="sxs-lookup"><span data-stu-id="80134-115">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="80134-116">创建通知</span><span class="sxs-lookup"><span data-stu-id="80134-116">Create notification</span></span>](../api/projectrome-notification-post.md) | [<span data-ttu-id="80134-117">通告</span><span class="sxs-lookup"><span data-stu-id="80134-117">notification</span></span>](projectrome-notification.md) |<span data-ttu-id="80134-118">创建并发送通知。</span><span class="sxs-lookup"><span data-stu-id="80134-118">Create and send a notification.</span></span> |

## <a name="properties"></a><span data-ttu-id="80134-119">属性</span><span class="sxs-lookup"><span data-stu-id="80134-119">Properties</span></span>
|<span data-ttu-id="80134-120">名称</span><span class="sxs-lookup"><span data-stu-id="80134-120">Name</span></span> | <span data-ttu-id="80134-121">类型</span><span class="sxs-lookup"><span data-stu-id="80134-121">Type</span></span> | <span data-ttu-id="80134-122">说明</span><span class="sxs-lookup"><span data-stu-id="80134-122">Description</span></span>|
|:----|:-----|:-----------|
| <span data-ttu-id="80134-123">targetHostName</span><span class="sxs-lookup"><span data-stu-id="80134-123">targetHostName</span></span> | <span data-ttu-id="80134-124">String</span><span class="sxs-lookup"><span data-stu-id="80134-124">String</span></span> | <span data-ttu-id="80134-125">表示呼叫服务要为其发布通知的应用程序的主机名 (针对给定用户)。</span><span class="sxs-lookup"><span data-stu-id="80134-125">Represents the host name of the app to which the calling service wants to post the notification, for the given user.</span></span> |
| <span data-ttu-id="80134-126">appNotificationId</span><span class="sxs-lookup"><span data-stu-id="80134-126">appNotificationId</span></span> | <span data-ttu-id="80134-127">String</span><span class="sxs-lookup"><span data-stu-id="80134-127">String</span></span> | <span data-ttu-id="80134-128">通知的应用程序服务器设置的唯一 id, 用于标识和定位单个通知。</span><span class="sxs-lookup"><span data-stu-id="80134-128">The unique id set by the app server of a notification that is used to identify and target an individual notification.</span></span> |
| <span data-ttu-id="80134-129">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="80134-129">expirationDateTime</span></span> | <span data-ttu-id="80134-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80134-130">DateTimeOffset</span></span> | <span data-ttu-id="80134-131">在用户通知上设置 UTC 过期时间-当时间启动时, 将从 Microsoft Graph 通知源存储中完全删除通知, 并且不再是通知历史记录的一部分。</span><span class="sxs-lookup"><span data-stu-id="80134-131">Sets a UTC expiration time on a user notification - when time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.</span></span> <span data-ttu-id="80134-132">最大值为30天。</span><span class="sxs-lookup"><span data-stu-id="80134-132">Max value is 30 days.</span></span> |
| <span data-ttu-id="80134-133">payload</span><span class="sxs-lookup"><span data-stu-id="80134-133">payload</span></span> | <span data-ttu-id="80134-134">Edm、JSON 对象</span><span class="sxs-lookup"><span data-stu-id="80134-134">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="80134-135">这是原始或直观的用户通知的数据内容, 这些通知将传递给应用客户端接收此通知并由其使用。</span><span class="sxs-lookup"><span data-stu-id="80134-135">This is the data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> |
| <span data-ttu-id="80134-136">rawContent</span><span class="sxs-lookup"><span data-stu-id="80134-136">payload.rawContent</span></span> | <span data-ttu-id="80134-137">String</span><span class="sxs-lookup"><span data-stu-id="80134-137">String</span></span> | <span data-ttu-id="80134-138">原始用户通知的通知内容, 该通知内容将传递给应用程序客户端接收此通知并由其使用。</span><span class="sxs-lookup"><span data-stu-id="80134-138">The notification content of a raw user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> <span data-ttu-id="80134-139">RawContent 和 VisualContent 中至少有一个有效的和需要对 POST 通知请求有效。</span><span class="sxs-lookup"><span data-stu-id="80134-139">At least one of Payload.RawContent and Payload.VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="80134-140">有效负载。 visual</span><span class="sxs-lookup"><span data-stu-id="80134-140">payload.visual</span></span> | <span data-ttu-id="80134-141">Edm、JSON 对象</span><span class="sxs-lookup"><span data-stu-id="80134-141">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="80134-142">直观用户通知的可视内容, 它将由每个移动平台上的通知平台使用, 并为用户呈现。</span><span class="sxs-lookup"><span data-stu-id="80134-142">The visual content of a visual user notification, which will be consumed by the notification platform on each mobile platform and rendered for the users.</span></span> <span data-ttu-id="80134-143">至少有一个内容和 VisualContent 需要对 POST 通知请求有效。</span><span class="sxs-lookup"><span data-stu-id="80134-143">At least one of Content and VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="80134-144">有效负载. 标题</span><span class="sxs-lookup"><span data-stu-id="80134-144">payload.visual.title</span></span> | <span data-ttu-id="80134-145">String</span><span class="sxs-lookup"><span data-stu-id="80134-145">String</span></span> | <span data-ttu-id="80134-146">可视用户通知的标题。</span><span class="sxs-lookup"><span data-stu-id="80134-146">The title of a visual user notification.</span></span> <span data-ttu-id="80134-147">必须具有 "标题" 或 "正文"。</span><span class="sxs-lookup"><span data-stu-id="80134-147">Must have either title or body.</span></span> |
| <span data-ttu-id="80134-148">有效负载</span><span class="sxs-lookup"><span data-stu-id="80134-148">payload.visual.body</span></span> | <span data-ttu-id="80134-149">String</span><span class="sxs-lookup"><span data-stu-id="80134-149">String</span></span> | <span data-ttu-id="80134-150">可视化用户通知的正文。</span><span class="sxs-lookup"><span data-stu-id="80134-150">The body of a visual user notification.</span></span> <span data-ttu-id="80134-151">必须具有 "标题" 或 "正文"。</span><span class="sxs-lookup"><span data-stu-id="80134-151">Must have either title or body.</span></span> |
| <span data-ttu-id="80134-152">displayTimeToLive</span><span class="sxs-lookup"><span data-stu-id="80134-152">displayTimeToLive</span></span> | <span data-ttu-id="80134-153">阈值</span><span class="sxs-lookup"><span data-stu-id="80134-153">Int</span></span> | <span data-ttu-id="80134-154">设置此通知内容将在每个平台的通知查看器中保留多长时间 (以秒为单位)。</span><span class="sxs-lookup"><span data-stu-id="80134-154">Sets how long (in seconds) this notification content will stay in each platform’s notification viewer.</span></span> <span data-ttu-id="80134-155">例如, 将通知传递给 Windows 设备时, 此属性的值将传递给 ToastNotification, 以确定 toast 通知将在用户的 Windows 操作中心保留多长时间。</span><span class="sxs-lookup"><span data-stu-id="80134-155">For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification will stay in the user’s Windows Action Center.</span></span> |
| <span data-ttu-id="80134-156">priority</span><span class="sxs-lookup"><span data-stu-id="80134-156">priority</span></span> | <span data-ttu-id="80134-157">EnumType</span><span class="sxs-lookup"><span data-stu-id="80134-157">EnumType</span></span> | <span data-ttu-id="80134-158">指示原始用户通知的优先级。</span><span class="sxs-lookup"><span data-stu-id="80134-158">Indicates the priority of a raw user notification.</span></span> <span data-ttu-id="80134-159">默认情况下, 视觉通知以高优先级发送。</span><span class="sxs-lookup"><span data-stu-id="80134-159">Visual notifications are sent with high priority by default.</span></span> <span data-ttu-id="80134-160">有效值为 "高" 和 "低"。</span><span class="sxs-lookup"><span data-stu-id="80134-160">Valid values are High and Low.</span></span> |
| <span data-ttu-id="80134-161">名</span><span class="sxs-lookup"><span data-stu-id="80134-161">groupName</span></span> | <span data-ttu-id="80134-162">String</span><span class="sxs-lookup"><span data-stu-id="80134-162">String</span></span> | <span data-ttu-id="80134-163">此通知所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="80134-163">The name of the group that this notification belongs to.</span></span> <span data-ttu-id="80134-164">它由开发人员设置, 用于将通知分组在一起。</span><span class="sxs-lookup"><span data-stu-id="80134-164">It is set by the developer for the purpose of grouping notifications together.</span></span> |
| <span data-ttu-id="80134-165">targetPolicy</span><span class="sxs-lookup"><span data-stu-id="80134-165">targetPolicy</span></span> | <span data-ttu-id="80134-166">Edm、JSON 对象</span><span class="sxs-lookup"><span data-stu-id="80134-166">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="80134-167">目标策略对象在两个不同的级别 (应针对其目标的终结点类型 (Windows、iOS 和 Android) 以及应针对目标的特定终结点 (由订阅 id 标识) 中处理通知传递策略。</span><span class="sxs-lookup"><span data-stu-id="80134-167">Target policy object handles notification delivery policy at two different levels - endpoint types (Windows, iOS and Android) that should be targeted, and specific endpoints (identified by subscription ids) that should be targeted.</span></span> |
| <span data-ttu-id="80134-168">targetPolicy。 platformTypes</span><span class="sxs-lookup"><span data-stu-id="80134-168">targetPolicy.platformTypes</span></span> | <span data-ttu-id="80134-169">Edm、集合 (EnumType)</span><span class="sxs-lookup"><span data-stu-id="80134-169">Edm.ComplexType, Collection (EnumType)</span></span> | <span data-ttu-id="80134-170">使用将通知分发筛选到特定平台或平台。</span><span class="sxs-lookup"><span data-stu-id="80134-170">Use to filter the notification distribution to a specific platform or platforms.</span></span> <span data-ttu-id="80134-171">默认情况下, 将启用所有 "推送终结点类型" (iOS、Windows 和 Android)。</span><span class="sxs-lookup"><span data-stu-id="80134-171">By default, all push endpoint types (iOS, Windows, and Android) are enabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="80134-172">关系</span><span class="sxs-lookup"><span data-stu-id="80134-172">Relationships</span></span>
<span data-ttu-id="80134-173">无。</span><span class="sxs-lookup"><span data-stu-id="80134-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="80134-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80134-174">JSON representation</span></span>
<span data-ttu-id="80134-175">以下是在发布传递到目标操作系统的直接直观通知时, 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80134-175">The following is a JSON representation of the resource when you publish a direct visual notification that is delivered to the destination operating system.</span></span>

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

<span data-ttu-id="80134-176">以下是在发布传递给应用程序客户端的原始数据通知时的资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80134-176">The following is a JSON representation of the resource when you publish a raw data notification that is delivered to app clients.</span></span>
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
