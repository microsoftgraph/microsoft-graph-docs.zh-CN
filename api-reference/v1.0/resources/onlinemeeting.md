---
title: onlineMeeting 资源类型
description: 包含有关会议的信息，包括联接 URL、与会者列表和说明。
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 105c9f3ffa594dd457b40124070aef0dbb96689a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871069"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="7445b-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="7445b-103">onlineMeeting resource type</span></span>

<span data-ttu-id="7445b-104">包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="7445b-104">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="7445b-105">方法</span><span class="sxs-lookup"><span data-stu-id="7445b-105">Methods</span></span>

| <span data-ttu-id="7445b-106">方法</span><span class="sxs-lookup"><span data-stu-id="7445b-106">Method</span></span>         | <span data-ttu-id="7445b-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="7445b-107">Return Type</span></span> | <span data-ttu-id="7445b-108">说明</span><span class="sxs-lookup"><span data-stu-id="7445b-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="7445b-109">创建 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="7445b-109">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="7445b-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="7445b-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="7445b-111">创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="7445b-111">Create an online meeting.</span></span> |
| [<span data-ttu-id="7445b-112">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="7445b-112">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="7445b-113">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="7445b-113">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="7445b-114">读取**onlineMeeting**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7445b-114">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="7445b-115">删除 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="7445b-115">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md) | <span data-ttu-id="7445b-116">无</span><span class="sxs-lookup"><span data-stu-id="7445b-116">None</span></span> | <span data-ttu-id="7445b-117">删除联机会议</span><span class="sxs-lookup"><span data-stu-id="7445b-117">Delete an online meeting</span></span> |

## <a name="properties"></a><span data-ttu-id="7445b-118">属性</span><span class="sxs-lookup"><span data-stu-id="7445b-118">Properties</span></span>

| <span data-ttu-id="7445b-119">属性</span><span class="sxs-lookup"><span data-stu-id="7445b-119">Property</span></span>                  | <span data-ttu-id="7445b-120">类型</span><span class="sxs-lookup"><span data-stu-id="7445b-120">Type</span></span>                                                   | <span data-ttu-id="7445b-121">说明</span><span class="sxs-lookup"><span data-stu-id="7445b-121">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7445b-122">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="7445b-122">audioConferencing</span></span>         | [<span data-ttu-id="7445b-123">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="7445b-123">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="7445b-124">联机会议的电话访问（拨入）信息。</span><span class="sxs-lookup"><span data-stu-id="7445b-124">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="7445b-125">只读。</span><span class="sxs-lookup"><span data-stu-id="7445b-125">Read-only.</span></span> |
| <span data-ttu-id="7445b-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="7445b-126">chatInfo</span></span>                  | [<span data-ttu-id="7445b-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="7445b-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="7445b-128">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="7445b-128">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="7445b-129">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="7445b-129">creationDateTime</span></span>          | <span data-ttu-id="7445b-130">日期时间</span><span class="sxs-lookup"><span data-stu-id="7445b-130">DateTime</span></span>                                               | <span data-ttu-id="7445b-131">以 UTC 表示的会议创建时间。</span><span class="sxs-lookup"><span data-stu-id="7445b-131">The meeting creation time in UTC.</span></span> <span data-ttu-id="7445b-132">只读。</span><span class="sxs-lookup"><span data-stu-id="7445b-132">Read-only.</span></span> |
| <span data-ttu-id="7445b-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7445b-133">startDateTime</span></span>             | <span data-ttu-id="7445b-134">日期时间</span><span class="sxs-lookup"><span data-stu-id="7445b-134">DateTime</span></span>                                               | <span data-ttu-id="7445b-135">以 UTC 表示的会议开始时间。</span><span class="sxs-lookup"><span data-stu-id="7445b-135">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="7445b-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7445b-136">endDateTime</span></span>               | <span data-ttu-id="7445b-137">日期时间</span><span class="sxs-lookup"><span data-stu-id="7445b-137">DateTime</span></span>                                               | <span data-ttu-id="7445b-138">以 UTC 表示的会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="7445b-138">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="7445b-139">id</span><span class="sxs-lookup"><span data-stu-id="7445b-139">id</span></span>                        | <span data-ttu-id="7445b-140">字符串</span><span class="sxs-lookup"><span data-stu-id="7445b-140">String</span></span>                                                 | <span data-ttu-id="7445b-141">与联机会议关联的默认 ID。</span><span class="sxs-lookup"><span data-stu-id="7445b-141">The default ID associated with the online meeting.</span></span> <span data-ttu-id="7445b-142">只读。</span><span class="sxs-lookup"><span data-stu-id="7445b-142">Read-only.</span></span> |
| <span data-ttu-id="7445b-143">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="7445b-143">joinWebUrl</span></span>                | <span data-ttu-id="7445b-144">String</span><span class="sxs-lookup"><span data-stu-id="7445b-144">String</span></span>                                                 | <span data-ttu-id="7445b-145">联机会议的加入 URL。</span><span class="sxs-lookup"><span data-stu-id="7445b-145">The join URL of the online meeting.</span></span> <span data-ttu-id="7445b-146">只读。</span><span class="sxs-lookup"><span data-stu-id="7445b-146">Read-only.</span></span>|
| <span data-ttu-id="7445b-147">participants</span><span class="sxs-lookup"><span data-stu-id="7445b-147">participants</span></span>              | [<span data-ttu-id="7445b-148">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="7445b-148">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="7445b-149">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="7445b-149">The participants associated with the online meeting.</span></span>  <span data-ttu-id="7445b-150">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="7445b-150">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="7445b-151">subject</span><span class="sxs-lookup"><span data-stu-id="7445b-151">subject</span></span>                   | <span data-ttu-id="7445b-152">String</span><span class="sxs-lookup"><span data-stu-id="7445b-152">String</span></span>                                                 | <span data-ttu-id="7445b-153">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="7445b-153">The subject of the online meeting.</span></span> |
| <span data-ttu-id="7445b-154">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="7445b-154">videoTeleconferenceId</span></span>     | <span data-ttu-id="7445b-155">String</span><span class="sxs-lookup"><span data-stu-id="7445b-155">String</span></span>                                                 | <span data-ttu-id="7445b-156">Videio 电话会议 ID。</span><span class="sxs-lookup"><span data-stu-id="7445b-156">The videio teleconferencing ID.</span></span> <span data-ttu-id="7445b-157">只读。</span><span class="sxs-lookup"><span data-stu-id="7445b-157">Read-only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="7445b-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7445b-158">JSON representation</span></span>

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
