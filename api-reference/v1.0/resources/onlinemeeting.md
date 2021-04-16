---
title: onlineMeeting 资源类型
description: 包含有关会议的信息。
author: jsandoval-msft
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 4e04e9f6d40be4e4ed9a432be6cc449c690790a7
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869853"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="f28f4-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="f28f4-103">onlineMeeting resource type</span></span>

<span data-ttu-id="f28f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f28f4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f28f4-105">包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="f28f4-105">Contains information about a meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="f28f4-106">方法</span><span class="sxs-lookup"><span data-stu-id="f28f4-106">Methods</span></span>

| <span data-ttu-id="f28f4-107">方法</span><span class="sxs-lookup"><span data-stu-id="f28f4-107">Method</span></span>                                                             | <span data-ttu-id="f28f4-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f28f4-108">Return Type</span></span>                       | <span data-ttu-id="f28f4-109">说明</span><span class="sxs-lookup"><span data-stu-id="f28f4-109">Description</span></span>                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="f28f4-110">创建 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f28f4-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md)  | [<span data-ttu-id="f28f4-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f28f4-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="f28f4-112">创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="f28f4-112">Create an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="f28f4-113">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f28f4-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md)                   | [<span data-ttu-id="f28f4-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f28f4-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="f28f4-115">读取 **onlineMeeting 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="f28f4-115">Read the properties and relationships of an **onlineMeeting** object.</span></span>                                        |
| [<span data-ttu-id="f28f4-116">更新</span><span class="sxs-lookup"><span data-stu-id="f28f4-116">Update</span></span>](../api/onlinemeeting-update.md)                           | [<span data-ttu-id="f28f4-117">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f28f4-117">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="f28f4-118">更新 **onlineMeeting 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="f28f4-118">Update the properties of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="f28f4-119">删除 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f28f4-119">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md)             | <span data-ttu-id="f28f4-120">无</span><span class="sxs-lookup"><span data-stu-id="f28f4-120">None</span></span>                              | <span data-ttu-id="f28f4-121">删除 **onlineMeeting** 对象。</span><span class="sxs-lookup"><span data-stu-id="f28f4-121">Delete an **onlineMeeting** object.</span></span>                                                                                    |
| [<span data-ttu-id="f28f4-122">创建或获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f28f4-122">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="f28f4-123">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f28f4-123">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="f28f4-124">创建具有自定义外部 ID 的 **onlineMeeting** 对象。</span><span class="sxs-lookup"><span data-stu-id="f28f4-124">Create an **onlineMeeting** object with a custom, external ID.</span></span> <span data-ttu-id="f28f4-125">如果会议已存在，请检索其属性。</span><span class="sxs-lookup"><span data-stu-id="f28f4-125">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="f28f4-126">属性</span><span class="sxs-lookup"><span data-stu-id="f28f4-126">Properties</span></span>

| <span data-ttu-id="f28f4-127">属性</span><span class="sxs-lookup"><span data-stu-id="f28f4-127">Property</span></span>              | <span data-ttu-id="f28f4-128">类型</span><span class="sxs-lookup"><span data-stu-id="f28f4-128">Type</span></span>                                          | <span data-ttu-id="f28f4-129">说明</span><span class="sxs-lookup"><span data-stu-id="f28f4-129">Description</span></span>                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f28f4-130">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="f28f4-130">allowedPresenters</span></span>     | [<span data-ttu-id="f28f4-131">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="f28f4-131">onlineMeetingPresenters</span></span>](#onlinemeetingpresenters-values)                       | <span data-ttu-id="f28f4-132">指定可在会议中成为演示者的人。</span><span class="sxs-lookup"><span data-stu-id="f28f4-132">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="f28f4-133">下表列出了可能的值。</span><span class="sxs-lookup"><span data-stu-id="f28f4-133">Possible values are listed in the following table.</span></span>                          |
| <span data-ttu-id="f28f4-134">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="f28f4-134">audioConferencing</span></span>     | [<span data-ttu-id="f28f4-135">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="f28f4-135">audioConferencing</span></span>](audioconferencing.md)     | <span data-ttu-id="f28f4-136">电话访问 (拨入) 联机会议的信息。</span><span class="sxs-lookup"><span data-stu-id="f28f4-136">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="f28f4-137">只读。</span><span class="sxs-lookup"><span data-stu-id="f28f4-137">Read-only.</span></span>                                                   |
| <span data-ttu-id="f28f4-138">chatInfo</span><span class="sxs-lookup"><span data-stu-id="f28f4-138">chatInfo</span></span>              | [<span data-ttu-id="f28f4-139">chatInfo</span><span class="sxs-lookup"><span data-stu-id="f28f4-139">chatInfo</span></span>](chatinfo.md)                       | <span data-ttu-id="f28f4-140">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="f28f4-140">The chat information associated with this online meeting.</span></span>                                                                  |
| <span data-ttu-id="f28f4-141">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="f28f4-141">creationDateTime</span></span>      | <span data-ttu-id="f28f4-142">日期时间</span><span class="sxs-lookup"><span data-stu-id="f28f4-142">DateTime</span></span>                                      | <span data-ttu-id="f28f4-143">会议创建时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="f28f4-143">The meeting creation time in UTC.</span></span> <span data-ttu-id="f28f4-144">只读。</span><span class="sxs-lookup"><span data-stu-id="f28f4-144">Read-only.</span></span>                                                                               |
| <span data-ttu-id="f28f4-145">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f28f4-145">endDateTime</span></span>           | <span data-ttu-id="f28f4-146">日期时间</span><span class="sxs-lookup"><span data-stu-id="f28f4-146">DateTime</span></span>                                      | <span data-ttu-id="f28f4-147">会议结束时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="f28f4-147">The meeting end time in UTC.</span></span>                                                                                               |
| <span data-ttu-id="f28f4-148">id</span><span class="sxs-lookup"><span data-stu-id="f28f4-148">id</span></span>                    | <span data-ttu-id="f28f4-149">String</span><span class="sxs-lookup"><span data-stu-id="f28f4-149">String</span></span>                                        | <span data-ttu-id="f28f4-150">与联机会议关联的默认 ID。</span><span class="sxs-lookup"><span data-stu-id="f28f4-150">The default ID associated with the online meeting.</span></span> <span data-ttu-id="f28f4-151">只读。</span><span class="sxs-lookup"><span data-stu-id="f28f4-151">Read-only.</span></span>                                                              |
| <span data-ttu-id="f28f4-152">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="f28f4-152">isEntryExitAnnounced</span></span>  | <span data-ttu-id="f28f4-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="f28f4-153">Boolean</span></span>                                       | <span data-ttu-id="f28f4-154">呼叫者加入或离开时是否宣布。</span><span class="sxs-lookup"><span data-stu-id="f28f4-154">Whether or not to announce when callers join or leave.</span></span>                                                                     |
| <span data-ttu-id="f28f4-155">joinInformation</span><span class="sxs-lookup"><span data-stu-id="f28f4-155">joinInformation</span></span>       | [<span data-ttu-id="f28f4-156">itemBody</span><span class="sxs-lookup"><span data-stu-id="f28f4-156">itemBody</span></span>](itembody.md)                       | <span data-ttu-id="f28f4-157">请求 HTTP 标头中指定的语言和区域设置变量中的 `Accept-Language` 联接信息。</span><span class="sxs-lookup"><span data-stu-id="f28f4-157">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="f28f4-158">只读。</span><span class="sxs-lookup"><span data-stu-id="f28f4-158">Read-only.</span></span> |
| <span data-ttu-id="f28f4-159">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="f28f4-159">joinWebUrl</span></span>            | <span data-ttu-id="f28f4-160">String</span><span class="sxs-lookup"><span data-stu-id="f28f4-160">String</span></span>                                        | <span data-ttu-id="f28f4-161">联机会议加入 URL。</span><span class="sxs-lookup"><span data-stu-id="f28f4-161">The join URL of the online meeting.</span></span> <span data-ttu-id="f28f4-162">只读。</span><span class="sxs-lookup"><span data-stu-id="f28f4-162">Read-only.</span></span>                                                                             |
| <span data-ttu-id="f28f4-163">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="f28f4-163">lobbyBypassSettings</span></span>   | [<span data-ttu-id="f28f4-164">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="f28f4-164">lobbyBypassSettings</span></span>](lobbyBypassSettings.md) | <span data-ttu-id="f28f4-165">指定哪些参与者可以绕过会议厅。</span><span class="sxs-lookup"><span data-stu-id="f28f4-165">Specifies which participants can bypass the meeting   lobby.</span></span>                                                               |
| <span data-ttu-id="f28f4-166">participants</span><span class="sxs-lookup"><span data-stu-id="f28f4-166">participants</span></span>          | [<span data-ttu-id="f28f4-167">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="f28f4-167">meetingParticipants</span></span>](meetingparticipants.md) | <span data-ttu-id="f28f4-168">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="f28f4-168">The participants associated with the online meeting.</span></span>  <span data-ttu-id="f28f4-169">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="f28f4-169">This includes the organizer and the attendees.</span></span>                       |
| <span data-ttu-id="f28f4-170">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f28f4-170">startDateTime</span></span>         | <span data-ttu-id="f28f4-171">日期时间</span><span class="sxs-lookup"><span data-stu-id="f28f4-171">DateTime</span></span>                                      | <span data-ttu-id="f28f4-172">会议开始时间（UTC）。</span><span class="sxs-lookup"><span data-stu-id="f28f4-172">The meeting start time in UTC.</span></span>                                                                                             |
| <span data-ttu-id="f28f4-173">subject</span><span class="sxs-lookup"><span data-stu-id="f28f4-173">subject</span></span>               | <span data-ttu-id="f28f4-174">String</span><span class="sxs-lookup"><span data-stu-id="f28f4-174">String</span></span>                                        | <span data-ttu-id="f28f4-175">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="f28f4-175">The subject of the online meeting.</span></span>                                                                                         |
| <span data-ttu-id="f28f4-176">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="f28f4-176">videoTeleconferenceId</span></span> | <span data-ttu-id="f28f4-177">String</span><span class="sxs-lookup"><span data-stu-id="f28f4-177">String</span></span>                                        | <span data-ttu-id="f28f4-178">视频电话会议 ID。</span><span class="sxs-lookup"><span data-stu-id="f28f4-178">The video teleconferencing ID.</span></span> <span data-ttu-id="f28f4-179">只读。</span><span class="sxs-lookup"><span data-stu-id="f28f4-179">Read-only.</span></span>                                                                                  |

### <a name="onlinemeetingpresenters-values"></a><span data-ttu-id="f28f4-180">onlineMeetingPresenters 值</span><span class="sxs-lookup"><span data-stu-id="f28f4-180">onlineMeetingPresenters values</span></span>

| <span data-ttu-id="f28f4-181">值</span><span class="sxs-lookup"><span data-stu-id="f28f4-181">Value</span></span>              | <span data-ttu-id="f28f4-182">说明</span><span class="sxs-lookup"><span data-stu-id="f28f4-182">Description</span></span>                                                   |
| ------------------ | ------------------------------------------------------------- |
| <span data-ttu-id="f28f4-183">everyone</span><span class="sxs-lookup"><span data-stu-id="f28f4-183">everyone</span></span>           | <span data-ttu-id="f28f4-184">每个人都是演示者 (这是默认选项) 。</span><span class="sxs-lookup"><span data-stu-id="f28f4-184">Everyone is a presenter (This is default option).</span></span>             |
| <span data-ttu-id="f28f4-185">组织</span><span class="sxs-lookup"><span data-stu-id="f28f4-185">organization</span></span>       | <span data-ttu-id="f28f4-186">组织者组织中的每个人都是演示者。</span><span class="sxs-lookup"><span data-stu-id="f28f4-186">Everyone in organizer’s organization is a presenter.</span></span>          |
| <span data-ttu-id="f28f4-187">roleIsPresenter</span><span class="sxs-lookup"><span data-stu-id="f28f4-187">roleIsPresenter</span></span>    | <span data-ttu-id="f28f4-188">只有其角色为演示者的参与者是演示者。</span><span class="sxs-lookup"><span data-stu-id="f28f4-188">Only the participants whose role is presenter are presenters.</span></span> |
| <span data-ttu-id="f28f4-189">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="f28f4-189">organizer</span></span>          | <span data-ttu-id="f28f4-190">只有组织者是演示者。</span><span class="sxs-lookup"><span data-stu-id="f28f4-190">Only the organizer  is a presenter.</span></span>                           |
| <span data-ttu-id="f28f4-191">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="f28f4-191">unknownFutureValue</span></span> | <span data-ttu-id="f28f4-192">不知情未来值。</span><span class="sxs-lookup"><span data-stu-id="f28f4-192">Unknow future value.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="f28f4-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f28f4-193">JSON representation</span></span>

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

