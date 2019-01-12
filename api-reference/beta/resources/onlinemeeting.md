---
title: onlineMeeting 资源类型
description: 捕获有关会议，包括加入 URL、 与会者列表中，及其说明的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6bae6cf22e8790050f0b77ab903c5702354ea1f5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980396"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="5a462-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a462-103">onlineMeeting resource type</span></span>

> <span data-ttu-id="5a462-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5a462-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a462-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5a462-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a462-106">捕获有关会议，包括加入 URL、 与会者列表中，及其说明的信息。</span><span class="sxs-lookup"><span data-stu-id="5a462-106">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="5a462-107">方法</span><span class="sxs-lookup"><span data-stu-id="5a462-107">Methods</span></span>

| <span data-ttu-id="5a462-108">方法</span><span class="sxs-lookup"><span data-stu-id="5a462-108">Method</span></span>         | <span data-ttu-id="5a462-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5a462-109">Return Type</span></span> | <span data-ttu-id="5a462-110">说明</span><span class="sxs-lookup"><span data-stu-id="5a462-110">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="5a462-111">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="5a462-111">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="5a462-112">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="5a462-112">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="5a462-113">读取属性和 onlineMeeting 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="5a462-113">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5a462-114">属性</span><span class="sxs-lookup"><span data-stu-id="5a462-114">Properties</span></span>

| <span data-ttu-id="5a462-115">属性</span><span class="sxs-lookup"><span data-stu-id="5a462-115">Property</span></span>                  | <span data-ttu-id="5a462-116">类型</span><span class="sxs-lookup"><span data-stu-id="5a462-116">Type</span></span>                                                   | <span data-ttu-id="5a462-117">Description</span><span class="sxs-lookup"><span data-stu-id="5a462-117">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5a462-118">accessLevel</span><span class="sxs-lookup"><span data-stu-id="5a462-118">accessLevel</span></span>               | <span data-ttu-id="5a462-119">字符串</span><span class="sxs-lookup"><span data-stu-id="5a462-119">String</span></span>                                                 | <span data-ttu-id="5a462-120">控制允许加入联机会议的访问级别。</span><span class="sxs-lookup"><span data-stu-id="5a462-120">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="5a462-121">可取值为：`everyone`、`invited`、`locked`、`sameEnterprise`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="5a462-121">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="5a462-122">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="5a462-122">audioConferencing</span></span>         | [<span data-ttu-id="5a462-123">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="5a462-123">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="5a462-124">代表 onlineMeeting 电话访问信息。</span><span class="sxs-lookup"><span data-stu-id="5a462-124">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="5a462-125">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="5a462-125">canceledDateTime</span></span>          | <span data-ttu-id="5a462-126">日期时间</span><span class="sxs-lookup"><span data-stu-id="5a462-126">DateTime</span></span>                                               | <span data-ttu-id="5a462-127">当取消会议的时间。</span><span class="sxs-lookup"><span data-stu-id="5a462-127">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="5a462-128">chatInfo</span><span class="sxs-lookup"><span data-stu-id="5a462-128">chatInfo</span></span>                  | [<span data-ttu-id="5a462-129">chatInfo</span><span class="sxs-lookup"><span data-stu-id="5a462-129">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="5a462-130">与此会议聊天。</span><span class="sxs-lookup"><span data-stu-id="5a462-130">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="5a462-131">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="5a462-131">creationDateTime</span></span>          | <span data-ttu-id="5a462-132">日期时间</span><span class="sxs-lookup"><span data-stu-id="5a462-132">DateTime</span></span>                                               | <span data-ttu-id="5a462-133">已创建会议的时间。</span><span class="sxs-lookup"><span data-stu-id="5a462-133">The time when the meeting was created.</span></span> <span data-ttu-id="5a462-134">Readonly。</span><span class="sxs-lookup"><span data-stu-id="5a462-134">Readonly.</span></span>
| <span data-ttu-id="5a462-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5a462-135">endDateTime</span></span>               | <span data-ttu-id="5a462-136">日期时间</span><span class="sxs-lookup"><span data-stu-id="5a462-136">DateTime</span></span>                                               | <span data-ttu-id="5a462-137">会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="5a462-137">End time of the meeting.</span></span> |
| <span data-ttu-id="5a462-138">entryExitAnnouncement</span><span class="sxs-lookup"><span data-stu-id="5a462-138">entryExitAnnouncement</span></span>     | <span data-ttu-id="5a462-139">布尔</span><span class="sxs-lookup"><span data-stu-id="5a462-139">Boolean</span></span>                                                | <span data-ttu-id="5a462-140">联机会议助理通知状态。</span><span class="sxs-lookup"><span data-stu-id="5a462-140">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="5a462-141">如果启用了出勤通知，联机会议将通过音频会议宣布 participantswho 联接的名称。</span><span class="sxs-lookup"><span data-stu-id="5a462-141">When attendance announcements are enabled, the online meeting will announce the names of the participantswho join the meeting through audio.</span></span> |
| <span data-ttu-id="5a462-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5a462-142">expirationDateTime</span></span>        | <span data-ttu-id="5a462-143">日期时间</span><span class="sxs-lookup"><span data-stu-id="5a462-143">DateTime</span></span>                                               | <span data-ttu-id="5a462-144">绝对协调世界时 (UTC) 日期和时间之后可以删除的联机会议。</span><span class="sxs-lookup"><span data-stu-id="5a462-144">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="5a462-145">日期和时间必须在前，一年之间十年后，当前日期和时间的服务器上。</span><span class="sxs-lookup"><span data-stu-id="5a462-145">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="5a462-146">id</span><span class="sxs-lookup"><span data-stu-id="5a462-146">id</span></span>                        | <span data-ttu-id="5a462-147">字符串</span><span class="sxs-lookup"><span data-stu-id="5a462-147">String</span></span>                                                 | <span data-ttu-id="5a462-148">与联机会议相关的 ID。</span><span class="sxs-lookup"><span data-stu-id="5a462-148">The ID associated with the online meeting.</span></span> <span data-ttu-id="5a462-149">获取 HTTP 请求中用作 id。</span><span class="sxs-lookup"><span data-stu-id="5a462-149">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="5a462-150">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="5a462-150">Read-only.</span></span> <span data-ttu-id="5a462-151">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="5a462-151">Server generated.</span></span> |
| <span data-ttu-id="5a462-152">isCancelled</span><span class="sxs-lookup"><span data-stu-id="5a462-152">isCancelled</span></span>               | <span data-ttu-id="5a462-153">布尔</span><span class="sxs-lookup"><span data-stu-id="5a462-153">Boolean</span></span>                                                | <span data-ttu-id="5a462-154">是否已被取消会议。</span><span class="sxs-lookup"><span data-stu-id="5a462-154">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="5a462-155">joinUrl</span><span class="sxs-lookup"><span data-stu-id="5a462-155">joinUrl</span></span>                   | <span data-ttu-id="5a462-156">字符串</span><span class="sxs-lookup"><span data-stu-id="5a462-156">String</span></span>                                                 | <span data-ttu-id="5a462-157">从 web 加入联机会议时所使用的 URL。</span><span class="sxs-lookup"><span data-stu-id="5a462-157">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="5a462-158">meetingType</span><span class="sxs-lookup"><span data-stu-id="5a462-158">meetingType</span></span>               | <span data-ttu-id="5a462-159">字符串</span><span class="sxs-lookup"><span data-stu-id="5a462-159">String</span></span>                                                 | <span data-ttu-id="5a462-160">可能的值为： `meetNow`， `scheduled`， `recurring`，`broadcast`</span><span class="sxs-lookup"><span data-stu-id="5a462-160">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast`</span></span> |
| <span data-ttu-id="5a462-161">participants</span><span class="sxs-lookup"><span data-stu-id="5a462-161">participants</span></span>              | [<span data-ttu-id="5a462-162">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="5a462-162">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="5a462-163">相关联的联机会议参与者。</span><span class="sxs-lookup"><span data-stu-id="5a462-163">The participants associated with the online meeting.</span></span>  <span data-ttu-id="5a462-164">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="5a462-164">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="5a462-165">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5a462-165">startDateTime</span></span>             | <span data-ttu-id="5a462-166">日期时间</span><span class="sxs-lookup"><span data-stu-id="5a462-166">DateTime</span></span>                                               | <span data-ttu-id="5a462-167">会议的开始时间。</span><span class="sxs-lookup"><span data-stu-id="5a462-167">Start time of the meeting.</span></span> |
| <span data-ttu-id="5a462-168">subject</span><span class="sxs-lookup"><span data-stu-id="5a462-168">subject</span></span>                   | <span data-ttu-id="5a462-169">字符串</span><span class="sxs-lookup"><span data-stu-id="5a462-169">String</span></span>                                                 | <span data-ttu-id="5a462-170">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="5a462-170">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5a462-171">Relationships</span><span class="sxs-lookup"><span data-stu-id="5a462-171">Relationships</span></span>
<span data-ttu-id="5a462-172">无</span><span class="sxs-lookup"><span data-stu-id="5a462-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a462-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a462-173">JSON representation</span></span>

<span data-ttu-id="5a462-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a462-174">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "accessLevel": "everyone | invited | locked | sameEnterprise",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "entryExitAnnouncement": true,
  "expirationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCancelled": false,
  "joinUrl": "String",
  "meetingType": "meetNow | scheduled | recurring | broadcast",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
