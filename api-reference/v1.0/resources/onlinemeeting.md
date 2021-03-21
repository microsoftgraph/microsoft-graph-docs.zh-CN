---
title: onlineMeeting 资源类型
description: 包含有关会议的信息。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: ce334002b58849671ab2e602594af0c8335b1377
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961942"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="93592-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="93592-103">onlineMeeting resource type</span></span>

<span data-ttu-id="93592-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93592-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93592-105">包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="93592-105">Contains information about a meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="93592-106">Methods</span><span class="sxs-lookup"><span data-stu-id="93592-106">Methods</span></span>

| <span data-ttu-id="93592-107">方法</span><span class="sxs-lookup"><span data-stu-id="93592-107">Method</span></span>                                                             | <span data-ttu-id="93592-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="93592-108">Return Type</span></span>                       | <span data-ttu-id="93592-109">说明</span><span class="sxs-lookup"><span data-stu-id="93592-109">Description</span></span>                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="93592-110">创建 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="93592-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md)  | [<span data-ttu-id="93592-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="93592-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="93592-112">创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="93592-112">Create an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="93592-113">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="93592-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md)                   | [<span data-ttu-id="93592-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="93592-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="93592-115">读取 **onlineMeeting 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="93592-115">Read the properties and relationships of an **onlineMeeting** object.</span></span>                                        |
| [<span data-ttu-id="93592-116">更新</span><span class="sxs-lookup"><span data-stu-id="93592-116">Update</span></span>](../api/onlinemeeting-update.md)                           | [<span data-ttu-id="93592-117">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="93592-117">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="93592-118">更新 **onlineMeeting 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="93592-118">Update the properties of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="93592-119">删除 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="93592-119">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md)             | <span data-ttu-id="93592-120">无</span><span class="sxs-lookup"><span data-stu-id="93592-120">None</span></span>                              | <span data-ttu-id="93592-121">删除 **onlineMeeting** 对象。</span><span class="sxs-lookup"><span data-stu-id="93592-121">Delete an **onlineMeeting** object.</span></span>                                                                                    |
| [<span data-ttu-id="93592-122">创建或获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="93592-122">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="93592-123">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="93592-123">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="93592-124">创建具有自定义外部 ID 的 **onlineMeeting** 对象。</span><span class="sxs-lookup"><span data-stu-id="93592-124">Create an **onlineMeeting** object with a custom, external ID.</span></span> <span data-ttu-id="93592-125">如果会议已存在，请检索其属性。</span><span class="sxs-lookup"><span data-stu-id="93592-125">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="93592-126">属性</span><span class="sxs-lookup"><span data-stu-id="93592-126">Properties</span></span>

| <span data-ttu-id="93592-127">属性</span><span class="sxs-lookup"><span data-stu-id="93592-127">Property</span></span>              | <span data-ttu-id="93592-128">类型</span><span class="sxs-lookup"><span data-stu-id="93592-128">Type</span></span>                                          | <span data-ttu-id="93592-129">说明</span><span class="sxs-lookup"><span data-stu-id="93592-129">Description</span></span>                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="93592-130">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="93592-130">allowedPresenters</span></span>     | [<span data-ttu-id="93592-131">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="93592-131">onlineMeetingPresenters</span></span>](#onlinemeetingpresenters-values)                       | <span data-ttu-id="93592-132">指定可在会议中成为演示者的人。</span><span class="sxs-lookup"><span data-stu-id="93592-132">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="93592-133">下表列出了可能的值。</span><span class="sxs-lookup"><span data-stu-id="93592-133">Possible values are listed in the following table.</span></span>                          |
| <span data-ttu-id="93592-134">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="93592-134">audioConferencing</span></span>     | [<span data-ttu-id="93592-135">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="93592-135">audioConferencing</span></span>](audioconferencing.md)     | <span data-ttu-id="93592-136">电话访问 (拨入) 联机会议的信息。</span><span class="sxs-lookup"><span data-stu-id="93592-136">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="93592-137">只读。</span><span class="sxs-lookup"><span data-stu-id="93592-137">Read-only.</span></span>                                                   |
| <span data-ttu-id="93592-138">chatInfo</span><span class="sxs-lookup"><span data-stu-id="93592-138">chatInfo</span></span>              | [<span data-ttu-id="93592-139">chatInfo</span><span class="sxs-lookup"><span data-stu-id="93592-139">chatInfo</span></span>](chatinfo.md)                       | <span data-ttu-id="93592-140">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="93592-140">The chat information associated with this online meeting.</span></span>                                                                  |
| <span data-ttu-id="93592-141">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="93592-141">creationDateTime</span></span>      | <span data-ttu-id="93592-142">日期时间</span><span class="sxs-lookup"><span data-stu-id="93592-142">DateTime</span></span>                                      | <span data-ttu-id="93592-143">会议创建时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="93592-143">The meeting creation time in UTC.</span></span> <span data-ttu-id="93592-144">只读。</span><span class="sxs-lookup"><span data-stu-id="93592-144">Read-only.</span></span>                                                                               |
| <span data-ttu-id="93592-145">endDateTime</span><span class="sxs-lookup"><span data-stu-id="93592-145">endDateTime</span></span>           | <span data-ttu-id="93592-146">日期时间</span><span class="sxs-lookup"><span data-stu-id="93592-146">DateTime</span></span>                                      | <span data-ttu-id="93592-147">会议结束时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="93592-147">The meeting end time in UTC.</span></span>                                                                                               |
| <span data-ttu-id="93592-148">id</span><span class="sxs-lookup"><span data-stu-id="93592-148">id</span></span>                    | <span data-ttu-id="93592-149">String</span><span class="sxs-lookup"><span data-stu-id="93592-149">String</span></span>                                        | <span data-ttu-id="93592-150">与联机会议关联的默认 ID。</span><span class="sxs-lookup"><span data-stu-id="93592-150">The default ID associated with the online meeting.</span></span> <span data-ttu-id="93592-151">只读。</span><span class="sxs-lookup"><span data-stu-id="93592-151">Read-only.</span></span>                                                              |
| <span data-ttu-id="93592-152">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="93592-152">isEntryExitAnnounced</span></span>  | <span data-ttu-id="93592-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="93592-153">Boolean</span></span>                                       | <span data-ttu-id="93592-154">呼叫者加入或离开时是否宣布。</span><span class="sxs-lookup"><span data-stu-id="93592-154">Whether or not to announce when callers join or leave.</span></span>                                                                     |
| <span data-ttu-id="93592-155">joinInformation</span><span class="sxs-lookup"><span data-stu-id="93592-155">joinInformation</span></span>       | [<span data-ttu-id="93592-156">itemBody</span><span class="sxs-lookup"><span data-stu-id="93592-156">itemBody</span></span>](itembody.md)                       | <span data-ttu-id="93592-157">请求 HTTP 标头中指定的语言和区域设置变量中的 `Accept-Language` 联接信息。</span><span class="sxs-lookup"><span data-stu-id="93592-157">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="93592-158">只读。</span><span class="sxs-lookup"><span data-stu-id="93592-158">Read-only.</span></span> |
| <span data-ttu-id="93592-159">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="93592-159">joinWebUrl</span></span>            | <span data-ttu-id="93592-160">String</span><span class="sxs-lookup"><span data-stu-id="93592-160">String</span></span>                                        | <span data-ttu-id="93592-161">联机会议加入 URL。</span><span class="sxs-lookup"><span data-stu-id="93592-161">The join URL of the online meeting.</span></span> <span data-ttu-id="93592-162">只读。</span><span class="sxs-lookup"><span data-stu-id="93592-162">Read-only.</span></span>                                                                             |
| <span data-ttu-id="93592-163">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="93592-163">lobbyBypassSettings</span></span>   | [<span data-ttu-id="93592-164">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="93592-164">lobbyBypassSettings</span></span>](lobbyBypassSettings.md) | <span data-ttu-id="93592-165">指定哪些参与者可以绕过会议厅。</span><span class="sxs-lookup"><span data-stu-id="93592-165">Specifies which participants can bypass the meeting   lobby.</span></span>                                                               |
| <span data-ttu-id="93592-166">participants</span><span class="sxs-lookup"><span data-stu-id="93592-166">participants</span></span>          | [<span data-ttu-id="93592-167">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="93592-167">meetingParticipants</span></span>](meetingparticipants.md) | <span data-ttu-id="93592-168">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="93592-168">The participants associated with the online meeting.</span></span>  <span data-ttu-id="93592-169">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="93592-169">This includes the organizer and the attendees.</span></span>                       |
| <span data-ttu-id="93592-170">startDateTime</span><span class="sxs-lookup"><span data-stu-id="93592-170">startDateTime</span></span>         | <span data-ttu-id="93592-171">日期时间</span><span class="sxs-lookup"><span data-stu-id="93592-171">DateTime</span></span>                                      | <span data-ttu-id="93592-172">会议开始时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="93592-172">The meeting start time in UTC.</span></span>                                                                                             |
| <span data-ttu-id="93592-173">subject</span><span class="sxs-lookup"><span data-stu-id="93592-173">subject</span></span>               | <span data-ttu-id="93592-174">String</span><span class="sxs-lookup"><span data-stu-id="93592-174">String</span></span>                                        | <span data-ttu-id="93592-175">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="93592-175">The subject of the online meeting.</span></span>                                                                                         |
| <span data-ttu-id="93592-176">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="93592-176">videoTeleconferenceId</span></span> | <span data-ttu-id="93592-177">String</span><span class="sxs-lookup"><span data-stu-id="93592-177">String</span></span>                                        | <span data-ttu-id="93592-178">视频电话会议 ID。</span><span class="sxs-lookup"><span data-stu-id="93592-178">The video teleconferencing ID.</span></span> <span data-ttu-id="93592-179">只读。</span><span class="sxs-lookup"><span data-stu-id="93592-179">Read-only.</span></span>                                                                                  |

### <a name="onlinemeetingpresenters-values"></a><span data-ttu-id="93592-180">onlineMeetingPresenters 值</span><span class="sxs-lookup"><span data-stu-id="93592-180">onlineMeetingPresenters values</span></span>

| <span data-ttu-id="93592-181">值</span><span class="sxs-lookup"><span data-stu-id="93592-181">Value</span></span>              | <span data-ttu-id="93592-182">说明</span><span class="sxs-lookup"><span data-stu-id="93592-182">Description</span></span>                                                   |
| ------------------ | ------------------------------------------------------------- |
| <span data-ttu-id="93592-183">everyone</span><span class="sxs-lookup"><span data-stu-id="93592-183">everyone</span></span>           | <span data-ttu-id="93592-184">每个人都是演示者 (这是默认选项) 。</span><span class="sxs-lookup"><span data-stu-id="93592-184">Everyone is a presenter (This is default option).</span></span>             |
| <span data-ttu-id="93592-185">组织</span><span class="sxs-lookup"><span data-stu-id="93592-185">organization</span></span>       | <span data-ttu-id="93592-186">组织者组织中的每个人都是演示者。</span><span class="sxs-lookup"><span data-stu-id="93592-186">Everyone in organizer’s organization is a presenter.</span></span>          |
| <span data-ttu-id="93592-187">roleIsPresenter</span><span class="sxs-lookup"><span data-stu-id="93592-187">roleIsPresenter</span></span>    | <span data-ttu-id="93592-188">只有其角色为演示者的参与者是演示者。</span><span class="sxs-lookup"><span data-stu-id="93592-188">Only the participants whose role is presenter are presenters.</span></span> |
| <span data-ttu-id="93592-189">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="93592-189">organizer</span></span>          | <span data-ttu-id="93592-190">只有组织者是演示者。</span><span class="sxs-lookup"><span data-stu-id="93592-190">Only the organizer  is a presenter.</span></span>                           |
| <span data-ttu-id="93592-191">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="93592-191">unknownFutureValue</span></span> | <span data-ttu-id="93592-192">不知情未来值。</span><span class="sxs-lookup"><span data-stu-id="93592-192">Unknow future value.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="93592-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93592-193">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "audioConferencing": {"@odata.type": "microsoft.graph.audioConferencing"},
  "chatInfo": {"@odata.type": "microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "participants": {"@odata.type": "microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "microsoft.graph.lobbyBypassSettings"},
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

