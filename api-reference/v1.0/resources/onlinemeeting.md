---
title: onlineMeeting 资源类型
description: 包含有关会议的信息，包括联接 URL、与会者列表和说明。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 812f094667b217d167509be324843227e552e0a5
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556224"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="b457a-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="b457a-103">onlineMeeting resource type</span></span>

<span data-ttu-id="b457a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b457a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b457a-105">包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="b457a-105">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="b457a-106">Methods</span><span class="sxs-lookup"><span data-stu-id="b457a-106">Methods</span></span>

| <span data-ttu-id="b457a-107">方法</span><span class="sxs-lookup"><span data-stu-id="b457a-107">Method</span></span>         | <span data-ttu-id="b457a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b457a-108">Return Type</span></span> | <span data-ttu-id="b457a-109">说明</span><span class="sxs-lookup"><span data-stu-id="b457a-109">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="b457a-110">创建 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b457a-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="b457a-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b457a-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="b457a-112">创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="b457a-112">Create an online meeting.</span></span> |
| [<span data-ttu-id="b457a-113">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b457a-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="b457a-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b457a-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="b457a-115">读取**onlineMeeting**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b457a-115">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="b457a-116">删除 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b457a-116">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md) | <span data-ttu-id="b457a-117">无</span><span class="sxs-lookup"><span data-stu-id="b457a-117">None</span></span> | <span data-ttu-id="b457a-118">删除联机会议。</span><span class="sxs-lookup"><span data-stu-id="b457a-118">Delete an online meeting.</span></span> |
| [<span data-ttu-id="b457a-119">创建或获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b457a-119">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="b457a-120">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b457a-120">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="b457a-121">使用自定义外部 ID 创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="b457a-121">Create an online meeting with a custom, external ID.</span></span> <span data-ttu-id="b457a-122">如果会议已存在，请检索其属性。</span><span class="sxs-lookup"><span data-stu-id="b457a-122">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="b457a-123">属性</span><span class="sxs-lookup"><span data-stu-id="b457a-123">Properties</span></span>

| <span data-ttu-id="b457a-124">属性</span><span class="sxs-lookup"><span data-stu-id="b457a-124">Property</span></span>                  | <span data-ttu-id="b457a-125">类型</span><span class="sxs-lookup"><span data-stu-id="b457a-125">Type</span></span>                                                   | <span data-ttu-id="b457a-126">说明</span><span class="sxs-lookup"><span data-stu-id="b457a-126">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b457a-127">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="b457a-127">audioConferencing</span></span>         | [<span data-ttu-id="b457a-128">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="b457a-128">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="b457a-129">联机会议的电话访问（拨入）信息。</span><span class="sxs-lookup"><span data-stu-id="b457a-129">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="b457a-130">只读。</span><span class="sxs-lookup"><span data-stu-id="b457a-130">Read-only.</span></span> |
| <span data-ttu-id="b457a-131">chatInfo</span><span class="sxs-lookup"><span data-stu-id="b457a-131">chatInfo</span></span>                  | [<span data-ttu-id="b457a-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="b457a-132">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="b457a-133">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="b457a-133">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="b457a-134">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="b457a-134">creationDateTime</span></span>          | <span data-ttu-id="b457a-135">日期/时间</span><span class="sxs-lookup"><span data-stu-id="b457a-135">DateTime</span></span>                                               | <span data-ttu-id="b457a-136">以 UTC 表示的会议创建时间。</span><span class="sxs-lookup"><span data-stu-id="b457a-136">The meeting creation time in UTC.</span></span> <span data-ttu-id="b457a-137">只读。</span><span class="sxs-lookup"><span data-stu-id="b457a-137">Read-only.</span></span> |
| <span data-ttu-id="b457a-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b457a-138">startDateTime</span></span>             | <span data-ttu-id="b457a-139">日期/时间</span><span class="sxs-lookup"><span data-stu-id="b457a-139">DateTime</span></span>                                               | <span data-ttu-id="b457a-140">以 UTC 表示的会议开始时间。</span><span class="sxs-lookup"><span data-stu-id="b457a-140">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="b457a-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b457a-141">endDateTime</span></span>               | <span data-ttu-id="b457a-142">日期/时间</span><span class="sxs-lookup"><span data-stu-id="b457a-142">DateTime</span></span>                                               | <span data-ttu-id="b457a-143">以 UTC 表示的会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="b457a-143">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="b457a-144">id</span><span class="sxs-lookup"><span data-stu-id="b457a-144">id</span></span>                        | <span data-ttu-id="b457a-145">字符串</span><span class="sxs-lookup"><span data-stu-id="b457a-145">String</span></span>                                                 | <span data-ttu-id="b457a-146">与联机会议关联的默认 ID。</span><span class="sxs-lookup"><span data-stu-id="b457a-146">The default ID associated with the online meeting.</span></span> <span data-ttu-id="b457a-147">只读。</span><span class="sxs-lookup"><span data-stu-id="b457a-147">Read-only.</span></span> |
| <span data-ttu-id="b457a-148">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="b457a-148">joinWebUrl</span></span>                | <span data-ttu-id="b457a-149">String</span><span class="sxs-lookup"><span data-stu-id="b457a-149">String</span></span>                                                 | <span data-ttu-id="b457a-150">联机会议的加入 URL。</span><span class="sxs-lookup"><span data-stu-id="b457a-150">The join URL of the online meeting.</span></span> <span data-ttu-id="b457a-151">只读。</span><span class="sxs-lookup"><span data-stu-id="b457a-151">Read-only.</span></span>|
| <span data-ttu-id="b457a-152">participants</span><span class="sxs-lookup"><span data-stu-id="b457a-152">participants</span></span>              | [<span data-ttu-id="b457a-153">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="b457a-153">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="b457a-154">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="b457a-154">The participants associated with the online meeting.</span></span>  <span data-ttu-id="b457a-155">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="b457a-155">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="b457a-156">subject</span><span class="sxs-lookup"><span data-stu-id="b457a-156">subject</span></span>                   | <span data-ttu-id="b457a-157">String</span><span class="sxs-lookup"><span data-stu-id="b457a-157">String</span></span>                                                 | <span data-ttu-id="b457a-158">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="b457a-158">The subject of the online meeting.</span></span> |
| <span data-ttu-id="b457a-159">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="b457a-159">videoTeleconferenceId</span></span>     | <span data-ttu-id="b457a-160">String</span><span class="sxs-lookup"><span data-stu-id="b457a-160">String</span></span>                                                 | <span data-ttu-id="b457a-161">视频电话会议 ID。</span><span class="sxs-lookup"><span data-stu-id="b457a-161">The video teleconferencing ID.</span></span> <span data-ttu-id="b457a-162">只读。</span><span class="sxs-lookup"><span data-stu-id="b457a-162">Read-only.</span></span> |
| <span data-ttu-id="b457a-163">joinInformation</span><span class="sxs-lookup"><span data-stu-id="b457a-163">joinInformation</span></span> | [<span data-ttu-id="b457a-164">itemBody</span><span class="sxs-lookup"><span data-stu-id="b457a-164">itemBody</span></span>](itembody.md) | <span data-ttu-id="b457a-165">请求 HTTP 标头中指定的语言和区域设置变量中的联接信息 `Accept-Language` 。</span><span class="sxs-lookup"><span data-stu-id="b457a-165">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="b457a-166">只读。</span><span class="sxs-lookup"><span data-stu-id="b457a-166">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b457a-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b457a-167">JSON representation</span></span>

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
