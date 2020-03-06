---
title: onlineMeeting 资源类型
description: 包含有关会议的信息，包括联接 URL、与会者列表和说明。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 531413ee2a9c322af99a98ecf2270faa50ccb0e0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534156"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="689d7-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="689d7-103">onlineMeeting resource type</span></span>

<span data-ttu-id="689d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="689d7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="689d7-105">包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="689d7-105">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="689d7-106">Methods</span><span class="sxs-lookup"><span data-stu-id="689d7-106">Methods</span></span>

| <span data-ttu-id="689d7-107">方法</span><span class="sxs-lookup"><span data-stu-id="689d7-107">Method</span></span>         | <span data-ttu-id="689d7-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="689d7-108">Return Type</span></span> | <span data-ttu-id="689d7-109">说明</span><span class="sxs-lookup"><span data-stu-id="689d7-109">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="689d7-110">创建 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="689d7-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="689d7-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="689d7-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="689d7-112">创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="689d7-112">Create an online meeting.</span></span> |
| [<span data-ttu-id="689d7-113">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="689d7-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="689d7-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="689d7-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="689d7-115">读取**onlineMeeting**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="689d7-115">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="689d7-116">删除 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="689d7-116">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md) | <span data-ttu-id="689d7-117">无</span><span class="sxs-lookup"><span data-stu-id="689d7-117">None</span></span> | <span data-ttu-id="689d7-118">删除联机会议</span><span class="sxs-lookup"><span data-stu-id="689d7-118">Delete an online meeting</span></span> |

## <a name="properties"></a><span data-ttu-id="689d7-119">属性</span><span class="sxs-lookup"><span data-stu-id="689d7-119">Properties</span></span>

| <span data-ttu-id="689d7-120">属性</span><span class="sxs-lookup"><span data-stu-id="689d7-120">Property</span></span>                  | <span data-ttu-id="689d7-121">类型</span><span class="sxs-lookup"><span data-stu-id="689d7-121">Type</span></span>                                                   | <span data-ttu-id="689d7-122">说明</span><span class="sxs-lookup"><span data-stu-id="689d7-122">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="689d7-123">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="689d7-123">audioConferencing</span></span>         | [<span data-ttu-id="689d7-124">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="689d7-124">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="689d7-125">联机会议的电话访问（拨入）信息。</span><span class="sxs-lookup"><span data-stu-id="689d7-125">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="689d7-126">只读。</span><span class="sxs-lookup"><span data-stu-id="689d7-126">Read-only.</span></span> |
| <span data-ttu-id="689d7-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="689d7-127">chatInfo</span></span>                  | [<span data-ttu-id="689d7-128">chatInfo</span><span class="sxs-lookup"><span data-stu-id="689d7-128">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="689d7-129">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="689d7-129">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="689d7-130">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="689d7-130">creationDateTime</span></span>          | <span data-ttu-id="689d7-131">日期时间</span><span class="sxs-lookup"><span data-stu-id="689d7-131">DateTime</span></span>                                               | <span data-ttu-id="689d7-132">以 UTC 表示的会议创建时间。</span><span class="sxs-lookup"><span data-stu-id="689d7-132">The meeting creation time in UTC.</span></span> <span data-ttu-id="689d7-133">只读。</span><span class="sxs-lookup"><span data-stu-id="689d7-133">Read-only.</span></span> |
| <span data-ttu-id="689d7-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="689d7-134">startDateTime</span></span>             | <span data-ttu-id="689d7-135">日期时间</span><span class="sxs-lookup"><span data-stu-id="689d7-135">DateTime</span></span>                                               | <span data-ttu-id="689d7-136">以 UTC 表示的会议开始时间。</span><span class="sxs-lookup"><span data-stu-id="689d7-136">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="689d7-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="689d7-137">endDateTime</span></span>               | <span data-ttu-id="689d7-138">日期时间</span><span class="sxs-lookup"><span data-stu-id="689d7-138">DateTime</span></span>                                               | <span data-ttu-id="689d7-139">以 UTC 表示的会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="689d7-139">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="689d7-140">id</span><span class="sxs-lookup"><span data-stu-id="689d7-140">id</span></span>                        | <span data-ttu-id="689d7-141">字符串</span><span class="sxs-lookup"><span data-stu-id="689d7-141">String</span></span>                                                 | <span data-ttu-id="689d7-142">与联机会议关联的默认 ID。</span><span class="sxs-lookup"><span data-stu-id="689d7-142">The default ID associated with the online meeting.</span></span> <span data-ttu-id="689d7-143">只读。</span><span class="sxs-lookup"><span data-stu-id="689d7-143">Read-only.</span></span> |
| <span data-ttu-id="689d7-144">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="689d7-144">joinWebUrl</span></span>                | <span data-ttu-id="689d7-145">字符串</span><span class="sxs-lookup"><span data-stu-id="689d7-145">String</span></span>                                                 | <span data-ttu-id="689d7-146">联机会议的加入 URL。</span><span class="sxs-lookup"><span data-stu-id="689d7-146">The join URL of the online meeting.</span></span> <span data-ttu-id="689d7-147">只读。</span><span class="sxs-lookup"><span data-stu-id="689d7-147">Read-only.</span></span>|
| <span data-ttu-id="689d7-148">participants</span><span class="sxs-lookup"><span data-stu-id="689d7-148">participants</span></span>              | [<span data-ttu-id="689d7-149">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="689d7-149">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="689d7-150">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="689d7-150">The participants associated with the online meeting.</span></span>  <span data-ttu-id="689d7-151">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="689d7-151">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="689d7-152">subject</span><span class="sxs-lookup"><span data-stu-id="689d7-152">subject</span></span>                   | <span data-ttu-id="689d7-153">String</span><span class="sxs-lookup"><span data-stu-id="689d7-153">String</span></span>                                                 | <span data-ttu-id="689d7-154">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="689d7-154">The subject of the online meeting.</span></span> |
| <span data-ttu-id="689d7-155">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="689d7-155">videoTeleconferenceId</span></span>     | <span data-ttu-id="689d7-156">字符串</span><span class="sxs-lookup"><span data-stu-id="689d7-156">String</span></span>                                                 | <span data-ttu-id="689d7-157">视频电话会议 ID。</span><span class="sxs-lookup"><span data-stu-id="689d7-157">The video teleconferencing ID.</span></span> <span data-ttu-id="689d7-158">只读。</span><span class="sxs-lookup"><span data-stu-id="689d7-158">Read-only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="689d7-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="689d7-159">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "videoTeleconferenceId": "String"
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
