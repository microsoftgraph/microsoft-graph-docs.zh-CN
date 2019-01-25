---
title: onlineMeeting 资源类型
description: 捕获有关会议，包括加入 URL、 与会者列表中，及其说明的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d7009ceaf815986d50c8eb3b64d2541c32f01a88
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519596"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="da0cf-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="da0cf-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da0cf-104">捕获有关会议，包括加入 URL、 与会者列表中，及其说明的信息。</span><span class="sxs-lookup"><span data-stu-id="da0cf-104">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="da0cf-105">方法</span><span class="sxs-lookup"><span data-stu-id="da0cf-105">Methods</span></span>

| <span data-ttu-id="da0cf-106">方法</span><span class="sxs-lookup"><span data-stu-id="da0cf-106">Method</span></span>         | <span data-ttu-id="da0cf-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="da0cf-107">Return Type</span></span> | <span data-ttu-id="da0cf-108">说明</span><span class="sxs-lookup"><span data-stu-id="da0cf-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="da0cf-109">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="da0cf-109">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="da0cf-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="da0cf-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="da0cf-111">读取属性和 onlineMeeting 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="da0cf-111">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="da0cf-112">属性</span><span class="sxs-lookup"><span data-stu-id="da0cf-112">Properties</span></span>

| <span data-ttu-id="da0cf-113">属性</span><span class="sxs-lookup"><span data-stu-id="da0cf-113">Property</span></span>                  | <span data-ttu-id="da0cf-114">类型</span><span class="sxs-lookup"><span data-stu-id="da0cf-114">Type</span></span>                                                   | <span data-ttu-id="da0cf-115">说明</span><span class="sxs-lookup"><span data-stu-id="da0cf-115">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="da0cf-116">AccessLevel</span><span class="sxs-lookup"><span data-stu-id="da0cf-116">accessLevel</span></span>               | <span data-ttu-id="da0cf-117">String</span><span class="sxs-lookup"><span data-stu-id="da0cf-117">String</span></span>                                                 | <span data-ttu-id="da0cf-118">控制允许加入联机会议的访问级别。</span><span class="sxs-lookup"><span data-stu-id="da0cf-118">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="da0cf-119">可取值为：`everyone`、`invited`、`locked`、`sameEnterprise`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="da0cf-119">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="da0cf-120">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="da0cf-120">audioConferencing</span></span>         | [<span data-ttu-id="da0cf-121">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="da0cf-121">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="da0cf-122">代表 onlineMeeting 电话访问信息。</span><span class="sxs-lookup"><span data-stu-id="da0cf-122">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="da0cf-123">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="da0cf-123">canceledDateTime</span></span>          | <span data-ttu-id="da0cf-124">日期/时间</span><span class="sxs-lookup"><span data-stu-id="da0cf-124">DateTime</span></span>                                               | <span data-ttu-id="da0cf-125">当取消会议的时间。</span><span class="sxs-lookup"><span data-stu-id="da0cf-125">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="da0cf-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="da0cf-126">chatInfo</span></span>                  | [<span data-ttu-id="da0cf-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="da0cf-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="da0cf-128">与此会议聊天。</span><span class="sxs-lookup"><span data-stu-id="da0cf-128">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="da0cf-129">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="da0cf-129">creationDateTime</span></span>          | <span data-ttu-id="da0cf-130">日期/时间</span><span class="sxs-lookup"><span data-stu-id="da0cf-130">DateTime</span></span>                                               | <span data-ttu-id="da0cf-131">已创建会议的时间。</span><span class="sxs-lookup"><span data-stu-id="da0cf-131">The time when the meeting was created.</span></span> <span data-ttu-id="da0cf-132">ReadOnly</span><span class="sxs-lookup"><span data-stu-id="da0cf-132">Readonly.</span></span>
| <span data-ttu-id="da0cf-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="da0cf-133">endDateTime</span></span>               | <span data-ttu-id="da0cf-134">日期/时间</span><span class="sxs-lookup"><span data-stu-id="da0cf-134">DateTime</span></span>                                               | <span data-ttu-id="da0cf-135">会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="da0cf-135">End time of the meeting.</span></span> |
| <span data-ttu-id="da0cf-136">entryExitAnnouncement</span><span class="sxs-lookup"><span data-stu-id="da0cf-136">entryExitAnnouncement</span></span>     | <span data-ttu-id="da0cf-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="da0cf-137">Boolean</span></span>                                                | <span data-ttu-id="da0cf-138">联机会议助理通知状态。</span><span class="sxs-lookup"><span data-stu-id="da0cf-138">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="da0cf-139">如果启用了出勤通知，联机会议将通过音频会议宣布 participantswho 联接的名称。</span><span class="sxs-lookup"><span data-stu-id="da0cf-139">When attendance announcements are enabled, the online meeting will announce the names of the participantswho join the meeting through audio.</span></span> |
| <span data-ttu-id="da0cf-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="da0cf-140">expirationDateTime</span></span>        | <span data-ttu-id="da0cf-141">日期/时间</span><span class="sxs-lookup"><span data-stu-id="da0cf-141">DateTime</span></span>                                               | <span data-ttu-id="da0cf-142">绝对协调世界时 (UTC) 日期和时间之后可以删除的联机会议。</span><span class="sxs-lookup"><span data-stu-id="da0cf-142">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="da0cf-143">日期和时间必须在前，一年之间十年后，当前日期和时间的服务器上。</span><span class="sxs-lookup"><span data-stu-id="da0cf-143">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="da0cf-144">id</span><span class="sxs-lookup"><span data-stu-id="da0cf-144">id</span></span>                        | <span data-ttu-id="da0cf-145">String</span><span class="sxs-lookup"><span data-stu-id="da0cf-145">String</span></span>                                                 | <span data-ttu-id="da0cf-146">与联机会议相关的 ID。</span><span class="sxs-lookup"><span data-stu-id="da0cf-146">The ID associated with the online meeting.</span></span> <span data-ttu-id="da0cf-147">获取 HTTP 请求中用作 id。</span><span class="sxs-lookup"><span data-stu-id="da0cf-147">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="da0cf-148">只读。</span><span class="sxs-lookup"><span data-stu-id="da0cf-148">Read-only.</span></span> <span data-ttu-id="da0cf-149">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="da0cf-149">Server generated.</span></span> |
| <span data-ttu-id="da0cf-150">isCancelled</span><span class="sxs-lookup"><span data-stu-id="da0cf-150">isCancelled</span></span>               | <span data-ttu-id="da0cf-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="da0cf-151">Boolean</span></span>                                                | <span data-ttu-id="da0cf-152">是否已被取消会议。</span><span class="sxs-lookup"><span data-stu-id="da0cf-152">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="da0cf-153">joinUrl</span><span class="sxs-lookup"><span data-stu-id="da0cf-153">joinUrl</span></span>                   | <span data-ttu-id="da0cf-154">String</span><span class="sxs-lookup"><span data-stu-id="da0cf-154">String</span></span>                                                 | <span data-ttu-id="da0cf-155">从 web 加入联机会议时所使用的 URL。</span><span class="sxs-lookup"><span data-stu-id="da0cf-155">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="da0cf-156">meetingType</span><span class="sxs-lookup"><span data-stu-id="da0cf-156">meetingType</span></span>               | <span data-ttu-id="da0cf-157">String</span><span class="sxs-lookup"><span data-stu-id="da0cf-157">String</span></span>                                                 | <span data-ttu-id="da0cf-158">可取值为：`meetNow`、`scheduled`、`recurring`。</span><span class="sxs-lookup"><span data-stu-id="da0cf-158">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast`</span></span> |
| <span data-ttu-id="da0cf-159">participants</span><span class="sxs-lookup"><span data-stu-id="da0cf-159">participants</span></span>              | [<span data-ttu-id="da0cf-160">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="da0cf-160">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="da0cf-161">相关联的联机会议参与者。</span><span class="sxs-lookup"><span data-stu-id="da0cf-161">The participants associated with the online meeting.</span></span>  <span data-ttu-id="da0cf-162">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="da0cf-162">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="da0cf-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="da0cf-163">startDateTime</span></span>             | <span data-ttu-id="da0cf-164">日期/时间</span><span class="sxs-lookup"><span data-stu-id="da0cf-164">DateTime</span></span>                                               | <span data-ttu-id="da0cf-165">会议的开始时间。</span><span class="sxs-lookup"><span data-stu-id="da0cf-165">Start time of the meeting.</span></span> |
| <span data-ttu-id="da0cf-166">subject</span><span class="sxs-lookup"><span data-stu-id="da0cf-166">subject</span></span>                   | <span data-ttu-id="da0cf-167">String</span><span class="sxs-lookup"><span data-stu-id="da0cf-167">String</span></span>                                                 | <span data-ttu-id="da0cf-168">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="da0cf-168">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="da0cf-169">关系</span><span class="sxs-lookup"><span data-stu-id="da0cf-169">Relationships</span></span>
<span data-ttu-id="da0cf-170">无</span><span class="sxs-lookup"><span data-stu-id="da0cf-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da0cf-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da0cf-171">JSON representation</span></span>

<span data-ttu-id="da0cf-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da0cf-172">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onlinemeeting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
