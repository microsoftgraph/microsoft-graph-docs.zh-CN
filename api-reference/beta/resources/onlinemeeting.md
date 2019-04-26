---
title: onlineMeeting 资源类型
description: 捕获有关会议的信息, 包括联接 URL、与会者列表和说明。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d7009ceaf815986d50c8eb3b64d2541c32f01a88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568856"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="71995-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="71995-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71995-104">捕获有关会议的信息, 包括联接 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="71995-104">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="71995-105">方法</span><span class="sxs-lookup"><span data-stu-id="71995-105">Methods</span></span>

| <span data-ttu-id="71995-106">方法</span><span class="sxs-lookup"><span data-stu-id="71995-106">Method</span></span>         | <span data-ttu-id="71995-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="71995-107">Return Type</span></span> | <span data-ttu-id="71995-108">说明</span><span class="sxs-lookup"><span data-stu-id="71995-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="71995-109">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="71995-109">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="71995-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="71995-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="71995-111">读取 onlineMeeting 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="71995-111">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="71995-112">属性</span><span class="sxs-lookup"><span data-stu-id="71995-112">Properties</span></span>

| <span data-ttu-id="71995-113">属性</span><span class="sxs-lookup"><span data-stu-id="71995-113">Property</span></span>                  | <span data-ttu-id="71995-114">类型</span><span class="sxs-lookup"><span data-stu-id="71995-114">Type</span></span>                                                   | <span data-ttu-id="71995-115">说明</span><span class="sxs-lookup"><span data-stu-id="71995-115">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="71995-116">accessLevel</span><span class="sxs-lookup"><span data-stu-id="71995-116">accessLevel</span></span>               | <span data-ttu-id="71995-117">String</span><span class="sxs-lookup"><span data-stu-id="71995-117">String</span></span>                                                 | <span data-ttu-id="71995-118">控制联机会议的许可的访问级别。</span><span class="sxs-lookup"><span data-stu-id="71995-118">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="71995-119">可取值为：`everyone`、`invited`、`locked`、`sameEnterprise` 或 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="71995-119">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="71995-120">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="71995-120">audioConferencing</span></span>         | [<span data-ttu-id="71995-121">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="71995-121">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="71995-122">表示 onlineMeeting 的电话访问信息。</span><span class="sxs-lookup"><span data-stu-id="71995-122">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="71995-123">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="71995-123">canceledDateTime</span></span>          | <span data-ttu-id="71995-124">日期/时间</span><span class="sxs-lookup"><span data-stu-id="71995-124">DateTime</span></span>                                               | <span data-ttu-id="71995-125">取消会议的时间。</span><span class="sxs-lookup"><span data-stu-id="71995-125">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="71995-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="71995-126">chatInfo</span></span>                  | [<span data-ttu-id="71995-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="71995-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="71995-128">与此会议关联的聊天。</span><span class="sxs-lookup"><span data-stu-id="71995-128">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="71995-129">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="71995-129">creationDateTime</span></span>          | <span data-ttu-id="71995-130">日期/时间</span><span class="sxs-lookup"><span data-stu-id="71995-130">DateTime</span></span>                                               | <span data-ttu-id="71995-131">会议的创建时间。</span><span class="sxs-lookup"><span data-stu-id="71995-131">The time when the meeting was created.</span></span> <span data-ttu-id="71995-132">只读.</span><span class="sxs-lookup"><span data-stu-id="71995-132">Readonly.</span></span>
| <span data-ttu-id="71995-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="71995-133">endDateTime</span></span>               | <span data-ttu-id="71995-134">日期/时间</span><span class="sxs-lookup"><span data-stu-id="71995-134">DateTime</span></span>                                               | <span data-ttu-id="71995-135">会议的结束时间。</span><span class="sxs-lookup"><span data-stu-id="71995-135">End time of the meeting.</span></span> |
| <span data-ttu-id="71995-136">entryExitAnnouncement</span><span class="sxs-lookup"><span data-stu-id="71995-136">entryExitAnnouncement</span></span>     | <span data-ttu-id="71995-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="71995-137">Boolean</span></span>                                                | <span data-ttu-id="71995-138">联机会议的出席通知状态。</span><span class="sxs-lookup"><span data-stu-id="71995-138">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="71995-139">启用出席通知后, 联机会议将宣布 participantswho 的名称通过音频加入会议。</span><span class="sxs-lookup"><span data-stu-id="71995-139">When attendance announcements are enabled, the online meeting will announce the names of the participantswho join the meeting through audio.</span></span> |
| <span data-ttu-id="71995-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="71995-140">expirationDateTime</span></span>        | <span data-ttu-id="71995-141">日期/时间</span><span class="sxs-lookup"><span data-stu-id="71995-141">DateTime</span></span>                                               | <span data-ttu-id="71995-142">可在其后删除联机会议的绝对协调通用时间 (UTC) 日期和时间。</span><span class="sxs-lookup"><span data-stu-id="71995-142">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="71995-143">日期和时间必须在服务器上的当前日期和时间之后的一年前一年和之后10年。</span><span class="sxs-lookup"><span data-stu-id="71995-143">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="71995-144">id</span><span class="sxs-lookup"><span data-stu-id="71995-144">id</span></span>                        | <span data-ttu-id="71995-145">字符串</span><span class="sxs-lookup"><span data-stu-id="71995-145">String</span></span>                                                 | <span data-ttu-id="71995-146">与联机会议相关联的 ID。</span><span class="sxs-lookup"><span data-stu-id="71995-146">The ID associated with the online meeting.</span></span> <span data-ttu-id="71995-147">在 GET HTTP 请求中用作 ID。</span><span class="sxs-lookup"><span data-stu-id="71995-147">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="71995-148">只读。</span><span class="sxs-lookup"><span data-stu-id="71995-148">Read-only.</span></span> <span data-ttu-id="71995-149">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="71995-149">Server generated.</span></span> |
| <span data-ttu-id="71995-150">isCancelled</span><span class="sxs-lookup"><span data-stu-id="71995-150">isCancelled</span></span>               | <span data-ttu-id="71995-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="71995-151">Boolean</span></span>                                                | <span data-ttu-id="71995-152">会议是否已被取消。</span><span class="sxs-lookup"><span data-stu-id="71995-152">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="71995-153">joinUrl</span><span class="sxs-lookup"><span data-stu-id="71995-153">joinUrl</span></span>                   | <span data-ttu-id="71995-154">String</span><span class="sxs-lookup"><span data-stu-id="71995-154">String</span></span>                                                 | <span data-ttu-id="71995-155">从 web 加入联机会议时使用的 URL。</span><span class="sxs-lookup"><span data-stu-id="71995-155">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="71995-156">meetingType</span><span class="sxs-lookup"><span data-stu-id="71995-156">meetingType</span></span>               | <span data-ttu-id="71995-157">String</span><span class="sxs-lookup"><span data-stu-id="71995-157">String</span></span>                                                 | <span data-ttu-id="71995-158">可能的值是`meetNow`: `scheduled`、 `recurring`、、`broadcast`</span><span class="sxs-lookup"><span data-stu-id="71995-158">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast`</span></span> |
| <span data-ttu-id="71995-159">participants</span><span class="sxs-lookup"><span data-stu-id="71995-159">participants</span></span>              | [<span data-ttu-id="71995-160">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="71995-160">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="71995-161">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="71995-161">The participants associated with the online meeting.</span></span>  <span data-ttu-id="71995-162">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="71995-162">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="71995-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="71995-163">startDateTime</span></span>             | <span data-ttu-id="71995-164">日期/时间</span><span class="sxs-lookup"><span data-stu-id="71995-164">DateTime</span></span>                                               | <span data-ttu-id="71995-165">会议的开始时间。</span><span class="sxs-lookup"><span data-stu-id="71995-165">Start time of the meeting.</span></span> |
| <span data-ttu-id="71995-166">主题</span><span class="sxs-lookup"><span data-stu-id="71995-166">subject</span></span>                   | <span data-ttu-id="71995-167">String</span><span class="sxs-lookup"><span data-stu-id="71995-167">String</span></span>                                                 | <span data-ttu-id="71995-168">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="71995-168">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="71995-169">关系</span><span class="sxs-lookup"><span data-stu-id="71995-169">Relationships</span></span>
<span data-ttu-id="71995-170">无</span><span class="sxs-lookup"><span data-stu-id="71995-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71995-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71995-171">JSON representation</span></span>

<span data-ttu-id="71995-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71995-172">The following is a JSON representation of the resource.</span></span>

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
