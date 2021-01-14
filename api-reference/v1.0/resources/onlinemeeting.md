---
title: onlineMeeting 资源类型
description: 包含有关会议的信息。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 139cd4a20a6097691189d1bd1f843850ba911a21
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866107"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="332e6-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="332e6-103">onlineMeeting resource type</span></span>

<span data-ttu-id="332e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="332e6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="332e6-105">包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="332e6-105">Contains information about a meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="332e6-106">Methods</span><span class="sxs-lookup"><span data-stu-id="332e6-106">Methods</span></span>

| <span data-ttu-id="332e6-107">方法</span><span class="sxs-lookup"><span data-stu-id="332e6-107">Method</span></span>                                                             | <span data-ttu-id="332e6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="332e6-108">Return Type</span></span>                       | <span data-ttu-id="332e6-109">说明</span><span class="sxs-lookup"><span data-stu-id="332e6-109">Description</span></span>                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="332e6-110">创建 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="332e6-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md)  | [<span data-ttu-id="332e6-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="332e6-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="332e6-112">创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="332e6-112">Create an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="332e6-113">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="332e6-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md)                   | [<span data-ttu-id="332e6-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="332e6-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="332e6-115">读取 **onlineMeeting 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="332e6-115">Read the properties and relationships of an **onlineMeeting** object.</span></span>                                        |
| [<span data-ttu-id="332e6-116">删除 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="332e6-116">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md)             | <span data-ttu-id="332e6-117">无</span><span class="sxs-lookup"><span data-stu-id="332e6-117">None</span></span>                              | <span data-ttu-id="332e6-118">删除联机会议。</span><span class="sxs-lookup"><span data-stu-id="332e6-118">Delete an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="332e6-119">创建或获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="332e6-119">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="332e6-120">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="332e6-120">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="332e6-121">使用自定义外部 ID 创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="332e6-121">Create an online meeting with a custom, external ID.</span></span> <span data-ttu-id="332e6-122">如果会议已存在，请检索其属性。</span><span class="sxs-lookup"><span data-stu-id="332e6-122">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="332e6-123">属性</span><span class="sxs-lookup"><span data-stu-id="332e6-123">Properties</span></span>

| <span data-ttu-id="332e6-124">属性</span><span class="sxs-lookup"><span data-stu-id="332e6-124">Property</span></span>              | <span data-ttu-id="332e6-125">类型</span><span class="sxs-lookup"><span data-stu-id="332e6-125">Type</span></span>                                          | <span data-ttu-id="332e6-126">说明</span><span class="sxs-lookup"><span data-stu-id="332e6-126">Description</span></span>                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="332e6-127">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="332e6-127">audioConferencing</span></span>     | [<span data-ttu-id="332e6-128">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="332e6-128">audioConferencing</span></span>](audioconferencing.md)     | <span data-ttu-id="332e6-129">电话访问 (拨入) 联机会议的信息。</span><span class="sxs-lookup"><span data-stu-id="332e6-129">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="332e6-130">只读。</span><span class="sxs-lookup"><span data-stu-id="332e6-130">Read-only.</span></span>                                                   |
| <span data-ttu-id="332e6-131">chatInfo</span><span class="sxs-lookup"><span data-stu-id="332e6-131">chatInfo</span></span>              | [<span data-ttu-id="332e6-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="332e6-132">chatInfo</span></span>](chatinfo.md)                       | <span data-ttu-id="332e6-133">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="332e6-133">The chat information associated with this online meeting.</span></span>                                                                  |
| <span data-ttu-id="332e6-134">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="332e6-134">creationDateTime</span></span>      | <span data-ttu-id="332e6-135">日期时间</span><span class="sxs-lookup"><span data-stu-id="332e6-135">DateTime</span></span>                                      | <span data-ttu-id="332e6-136">会议创建时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="332e6-136">The meeting creation time in UTC.</span></span> <span data-ttu-id="332e6-137">只读。</span><span class="sxs-lookup"><span data-stu-id="332e6-137">Read-only.</span></span>                                                                               |
| <span data-ttu-id="332e6-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="332e6-138">startDateTime</span></span>         | <span data-ttu-id="332e6-139">日期时间</span><span class="sxs-lookup"><span data-stu-id="332e6-139">DateTime</span></span>                                      | <span data-ttu-id="332e6-140">会议开始时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="332e6-140">The meeting start time in UTC.</span></span>                                                                                             |
| <span data-ttu-id="332e6-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="332e6-141">endDateTime</span></span>           | <span data-ttu-id="332e6-142">日期时间</span><span class="sxs-lookup"><span data-stu-id="332e6-142">DateTime</span></span>                                      | <span data-ttu-id="332e6-143">会议结束时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="332e6-143">The meeting end time in UTC.</span></span>                                                                                               |
| <span data-ttu-id="332e6-144">id</span><span class="sxs-lookup"><span data-stu-id="332e6-144">id</span></span>                    | <span data-ttu-id="332e6-145">String</span><span class="sxs-lookup"><span data-stu-id="332e6-145">String</span></span>                                        | <span data-ttu-id="332e6-146">与联机会议关联的默认 ID。</span><span class="sxs-lookup"><span data-stu-id="332e6-146">The default ID associated with the online meeting.</span></span> <span data-ttu-id="332e6-147">只读。</span><span class="sxs-lookup"><span data-stu-id="332e6-147">Read-only.</span></span>                                                              |
| <span data-ttu-id="332e6-148">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="332e6-148">joinWebUrl</span></span>            | <span data-ttu-id="332e6-149">String</span><span class="sxs-lookup"><span data-stu-id="332e6-149">String</span></span>                                        | <span data-ttu-id="332e6-150">联机会议加入 URL。</span><span class="sxs-lookup"><span data-stu-id="332e6-150">The join URL of the online meeting.</span></span> <span data-ttu-id="332e6-151">只读。</span><span class="sxs-lookup"><span data-stu-id="332e6-151">Read-only.</span></span>                                                                             |
| <span data-ttu-id="332e6-152">participants</span><span class="sxs-lookup"><span data-stu-id="332e6-152">participants</span></span>          | [<span data-ttu-id="332e6-153">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="332e6-153">meetingParticipants</span></span>](meetingparticipants.md) | <span data-ttu-id="332e6-154">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="332e6-154">The participants associated with the online meeting.</span></span>  <span data-ttu-id="332e6-155">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="332e6-155">This includes the organizer and the attendees.</span></span>                       |
| <span data-ttu-id="332e6-156">subject</span><span class="sxs-lookup"><span data-stu-id="332e6-156">subject</span></span>               | <span data-ttu-id="332e6-157">String</span><span class="sxs-lookup"><span data-stu-id="332e6-157">String</span></span>                                        | <span data-ttu-id="332e6-158">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="332e6-158">The subject of the online meeting.</span></span>                                                                                         |
| <span data-ttu-id="332e6-159">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="332e6-159">videoTeleconferenceId</span></span> | <span data-ttu-id="332e6-160">String</span><span class="sxs-lookup"><span data-stu-id="332e6-160">String</span></span>                                        | <span data-ttu-id="332e6-161">视频电话会议 ID。</span><span class="sxs-lookup"><span data-stu-id="332e6-161">The video teleconferencing ID.</span></span> <span data-ttu-id="332e6-162">只读。</span><span class="sxs-lookup"><span data-stu-id="332e6-162">Read-only.</span></span>                                                                                  |
| <span data-ttu-id="332e6-163">joinInformation</span><span class="sxs-lookup"><span data-stu-id="332e6-163">joinInformation</span></span>       | [<span data-ttu-id="332e6-164">itemBody</span><span class="sxs-lookup"><span data-stu-id="332e6-164">itemBody</span></span>](itembody.md)                       | <span data-ttu-id="332e6-165">请求 HTTP 标头中指定的语言和区域设置变量 `Accept-Language` 的联接信息。</span><span class="sxs-lookup"><span data-stu-id="332e6-165">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="332e6-166">只读。</span><span class="sxs-lookup"><span data-stu-id="332e6-166">Read-only.</span></span> |
| <span data-ttu-id="332e6-167">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="332e6-167">isEntryExitAnnounced</span></span>  | <span data-ttu-id="332e6-168">布尔</span><span class="sxs-lookup"><span data-stu-id="332e6-168">Boolean</span></span>                                       | <span data-ttu-id="332e6-169">呼叫者加入或离开时是否宣布。</span><span class="sxs-lookup"><span data-stu-id="332e6-169">Whether or not to announce when callers join or leave.</span></span>                                                                     |
| <span data-ttu-id="332e6-170">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="332e6-170">lobbyBypassSettings</span></span>   | [<span data-ttu-id="332e6-171">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="332e6-171">lobbyBypassSettings</span></span>](lobbyBypassSettings.md) | <span data-ttu-id="332e6-172">指定哪些参与者可以绕过会议厅。</span><span class="sxs-lookup"><span data-stu-id="332e6-172">Specifies which participants can bypass the meeting   lobby.</span></span>                                                               |
| <span data-ttu-id="332e6-173">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="332e6-173">allowedPresenters</span></span>     | <span data-ttu-id="332e6-174">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="332e6-174">onlineMeetingPresenters</span></span>                       | <span data-ttu-id="332e6-175">指定可在会议中成为演示者的人。</span><span class="sxs-lookup"><span data-stu-id="332e6-175">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="332e6-176">下表列出了可能的值。</span><span class="sxs-lookup"><span data-stu-id="332e6-176">Possible values are listed in the following table.</span></span>                          |

### <a name="onlinemeetingpresenters-values"></a><span data-ttu-id="332e6-177">onlineMeetingPresenters 值</span><span class="sxs-lookup"><span data-stu-id="332e6-177">onlineMeetingPresenters values</span></span>

| <span data-ttu-id="332e6-178">值</span><span class="sxs-lookup"><span data-stu-id="332e6-178">Value</span></span>              | <span data-ttu-id="332e6-179">说明</span><span class="sxs-lookup"><span data-stu-id="332e6-179">Description</span></span>                                                   |
| ------------------ | ------------------------------------------------------------- |
| <span data-ttu-id="332e6-180">everyone</span><span class="sxs-lookup"><span data-stu-id="332e6-180">everyone</span></span>           | <span data-ttu-id="332e6-181">每个人都是演示者 (这是默认选项) 。</span><span class="sxs-lookup"><span data-stu-id="332e6-181">Everyone is a presenter (This is default option).</span></span>             |
| <span data-ttu-id="332e6-182">组织</span><span class="sxs-lookup"><span data-stu-id="332e6-182">organization</span></span>       | <span data-ttu-id="332e6-183">组织者组织中的每个人都是演示者。</span><span class="sxs-lookup"><span data-stu-id="332e6-183">Everyone in organizer’s organization is a presenter.</span></span>          |
| <span data-ttu-id="332e6-184">roleIsPresenter</span><span class="sxs-lookup"><span data-stu-id="332e6-184">roleIsPresenter</span></span>    | <span data-ttu-id="332e6-185">只有其角色为演示者的参与者是演示者。</span><span class="sxs-lookup"><span data-stu-id="332e6-185">Only the participants whose role is presenter are presenters.</span></span> |
| <span data-ttu-id="332e6-186">组织者</span><span class="sxs-lookup"><span data-stu-id="332e6-186">organizer</span></span>          | <span data-ttu-id="332e6-187">只有组织者是演示者。</span><span class="sxs-lookup"><span data-stu-id="332e6-187">Only the organizer  is a presenter.</span></span>                           |
| <span data-ttu-id="332e6-188">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="332e6-188">unknownFutureValue</span></span> | <span data-ttu-id="332e6-189">未知未来值。</span><span class="sxs-lookup"><span data-stu-id="332e6-189">Unknow future value.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="332e6-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="332e6-190">JSON representation</span></span>

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
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "#microsoft.graph.lobbyBypassSettings"},
  "allowedPresenters": "String"
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

