---
title: onlineMeeting 资源类型
description: 包含有关会议的信息。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 9f986bf0bd7871185673759a6e98e80d5d10b4b7
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2020
ms.locfileid: "48741927"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="64125-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="64125-103">onlineMeeting resource type</span></span>

<span data-ttu-id="64125-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64125-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64125-105">包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="64125-105">Contains information about a meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="64125-106">方法</span><span class="sxs-lookup"><span data-stu-id="64125-106">Methods</span></span>

| <span data-ttu-id="64125-107">方法</span><span class="sxs-lookup"><span data-stu-id="64125-107">Method</span></span>                                                             | <span data-ttu-id="64125-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="64125-108">Return Type</span></span>                       | <span data-ttu-id="64125-109">说明</span><span class="sxs-lookup"><span data-stu-id="64125-109">Description</span></span>                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="64125-110">创建 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="64125-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md)  | [<span data-ttu-id="64125-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="64125-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="64125-112">创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="64125-112">Create an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="64125-113">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="64125-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md)                   | [<span data-ttu-id="64125-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="64125-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="64125-115">读取 **onlineMeeting** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="64125-115">Read the properties and relationships of an **onlineMeeting** object.</span></span>                                        |
| [<span data-ttu-id="64125-116">删除 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="64125-116">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md)             | <span data-ttu-id="64125-117">无</span><span class="sxs-lookup"><span data-stu-id="64125-117">None</span></span>                              | <span data-ttu-id="64125-118">删除联机会议。</span><span class="sxs-lookup"><span data-stu-id="64125-118">Delete an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="64125-119">创建或获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="64125-119">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="64125-120">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="64125-120">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="64125-121">使用自定义外部 ID 创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="64125-121">Create an online meeting with a custom, external ID.</span></span> <span data-ttu-id="64125-122">如果会议已存在，请检索其属性。</span><span class="sxs-lookup"><span data-stu-id="64125-122">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="64125-123">属性</span><span class="sxs-lookup"><span data-stu-id="64125-123">Properties</span></span>

| <span data-ttu-id="64125-124">属性</span><span class="sxs-lookup"><span data-stu-id="64125-124">Property</span></span>              | <span data-ttu-id="64125-125">类型</span><span class="sxs-lookup"><span data-stu-id="64125-125">Type</span></span>                                          | <span data-ttu-id="64125-126">说明</span><span class="sxs-lookup"><span data-stu-id="64125-126">Description</span></span>                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="64125-127">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="64125-127">audioConferencing</span></span>     | [<span data-ttu-id="64125-128">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="64125-128">audioConferencing</span></span>](audioconferencing.md)     | <span data-ttu-id="64125-129">电话访问 (电话拨入) 联机会议的信息。</span><span class="sxs-lookup"><span data-stu-id="64125-129">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="64125-130">只读。</span><span class="sxs-lookup"><span data-stu-id="64125-130">Read-only.</span></span>                                                   |
| <span data-ttu-id="64125-131">chatInfo</span><span class="sxs-lookup"><span data-stu-id="64125-131">chatInfo</span></span>              | [<span data-ttu-id="64125-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="64125-132">chatInfo</span></span>](chatinfo.md)                       | <span data-ttu-id="64125-133">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="64125-133">The chat information associated with this online meeting.</span></span>                                                                  |
| <span data-ttu-id="64125-134">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="64125-134">creationDateTime</span></span>      | <span data-ttu-id="64125-135">日期时间</span><span class="sxs-lookup"><span data-stu-id="64125-135">DateTime</span></span>                                      | <span data-ttu-id="64125-136">以 UTC 表示的会议创建时间。</span><span class="sxs-lookup"><span data-stu-id="64125-136">The meeting creation time in UTC.</span></span> <span data-ttu-id="64125-137">只读。</span><span class="sxs-lookup"><span data-stu-id="64125-137">Read-only.</span></span>                                                                               |
| <span data-ttu-id="64125-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="64125-138">startDateTime</span></span>         | <span data-ttu-id="64125-139">日期时间</span><span class="sxs-lookup"><span data-stu-id="64125-139">DateTime</span></span>                                      | <span data-ttu-id="64125-140">以 UTC 表示的会议开始时间。</span><span class="sxs-lookup"><span data-stu-id="64125-140">The meeting start time in UTC.</span></span>                                                                                             |
| <span data-ttu-id="64125-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="64125-141">endDateTime</span></span>           | <span data-ttu-id="64125-142">日期时间</span><span class="sxs-lookup"><span data-stu-id="64125-142">DateTime</span></span>                                      | <span data-ttu-id="64125-143">以 UTC 表示的会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="64125-143">The meeting end time in UTC.</span></span>                                                                                               |
| <span data-ttu-id="64125-144">id</span><span class="sxs-lookup"><span data-stu-id="64125-144">id</span></span>                    | <span data-ttu-id="64125-145">String</span><span class="sxs-lookup"><span data-stu-id="64125-145">String</span></span>                                        | <span data-ttu-id="64125-146">与联机会议关联的默认 ID。</span><span class="sxs-lookup"><span data-stu-id="64125-146">The default ID associated with the online meeting.</span></span> <span data-ttu-id="64125-147">只读。</span><span class="sxs-lookup"><span data-stu-id="64125-147">Read-only.</span></span>                                                              |
| <span data-ttu-id="64125-148">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="64125-148">joinWebUrl</span></span>            | <span data-ttu-id="64125-149">String</span><span class="sxs-lookup"><span data-stu-id="64125-149">String</span></span>                                        | <span data-ttu-id="64125-150">联机会议的加入 URL。</span><span class="sxs-lookup"><span data-stu-id="64125-150">The join URL of the online meeting.</span></span> <span data-ttu-id="64125-151">只读。</span><span class="sxs-lookup"><span data-stu-id="64125-151">Read-only.</span></span>                                                                             |
| <span data-ttu-id="64125-152">participants</span><span class="sxs-lookup"><span data-stu-id="64125-152">participants</span></span>          | [<span data-ttu-id="64125-153">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="64125-153">meetingParticipants</span></span>](meetingparticipants.md) | <span data-ttu-id="64125-154">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="64125-154">The participants associated with the online meeting.</span></span>  <span data-ttu-id="64125-155">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="64125-155">This includes the organizer and the attendees.</span></span>                       |
| <span data-ttu-id="64125-156">subject</span><span class="sxs-lookup"><span data-stu-id="64125-156">subject</span></span>               | <span data-ttu-id="64125-157">String</span><span class="sxs-lookup"><span data-stu-id="64125-157">String</span></span>                                        | <span data-ttu-id="64125-158">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="64125-158">The subject of the online meeting.</span></span>                                                                                         |
| <span data-ttu-id="64125-159">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="64125-159">videoTeleconferenceId</span></span> | <span data-ttu-id="64125-160">String</span><span class="sxs-lookup"><span data-stu-id="64125-160">String</span></span>                                        | <span data-ttu-id="64125-161">视频电话会议 ID。</span><span class="sxs-lookup"><span data-stu-id="64125-161">The video teleconferencing ID.</span></span> <span data-ttu-id="64125-162">只读。</span><span class="sxs-lookup"><span data-stu-id="64125-162">Read-only.</span></span>                                                                                  |
| <span data-ttu-id="64125-163">joinInformation</span><span class="sxs-lookup"><span data-stu-id="64125-163">joinInformation</span></span>       | [<span data-ttu-id="64125-164">itemBody</span><span class="sxs-lookup"><span data-stu-id="64125-164">itemBody</span></span>](itembody.md)                       | <span data-ttu-id="64125-165">请求 HTTP 标头中指定的语言和区域设置变量中的联接信息 `Accept-Language` 。</span><span class="sxs-lookup"><span data-stu-id="64125-165">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="64125-166">只读。</span><span class="sxs-lookup"><span data-stu-id="64125-166">Read-only.</span></span> |
| <span data-ttu-id="64125-167">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="64125-167">isEntryExitAnnounced</span></span>  | <span data-ttu-id="64125-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="64125-168">Boolean</span></span>                                       | <span data-ttu-id="64125-169">当呼叫者加入或离开时是否发出通知。</span><span class="sxs-lookup"><span data-stu-id="64125-169">Whether or not to announce when callers join or leave.</span></span>                                                                     |
| <span data-ttu-id="64125-170">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="64125-170">lobbyBypassSettings</span></span>   | [<span data-ttu-id="64125-171">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="64125-171">lobbyBypassSettings</span></span>](lobbyBypassSettings.md) | <span data-ttu-id="64125-172">指定哪些参与者可以绕过会议厅。</span><span class="sxs-lookup"><span data-stu-id="64125-172">Specifies which participants can bypass the meeting   lobby.</span></span>                                                                 |
| <span data-ttu-id="64125-173">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="64125-173">allowedPresenters</span></span>     | <span data-ttu-id="64125-174">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="64125-174">onlineMeetingPresenters</span></span>                       | <span data-ttu-id="64125-175">指定谁可以成为会议中的演示者。</span><span class="sxs-lookup"><span data-stu-id="64125-175">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="64125-176">下表中列出了可能的值。</span><span class="sxs-lookup"><span data-stu-id="64125-176">Possible values are listed in the following table.</span></span>                                           |

### <a name="onlinemeetingpresenters-values"></a><span data-ttu-id="64125-177">onlineMeetingPresenters 值</span><span class="sxs-lookup"><span data-stu-id="64125-177">onlineMeetingPresenters values</span></span>

| <span data-ttu-id="64125-178">值</span><span class="sxs-lookup"><span data-stu-id="64125-178">Value</span></span>              | <span data-ttu-id="64125-179">说明</span><span class="sxs-lookup"><span data-stu-id="64125-179">Description</span></span>                                                   |
| ------------------ | ------------------------------------------------------------- |
| <span data-ttu-id="64125-180">成员</span><span class="sxs-lookup"><span data-stu-id="64125-180">everyone</span></span>           | <span data-ttu-id="64125-181">每个人都是演示者 (这是) 的默认选项。</span><span class="sxs-lookup"><span data-stu-id="64125-181">Everyone is a presenter (This is default option).</span></span>             |
| <span data-ttu-id="64125-182">组织</span><span class="sxs-lookup"><span data-stu-id="64125-182">organization</span></span>       | <span data-ttu-id="64125-183">组织者组织中的所有人都是演示者。</span><span class="sxs-lookup"><span data-stu-id="64125-183">Everyone in organizer’s organization is a presenter.</span></span>          |
| <span data-ttu-id="64125-184">roleIsPresenter</span><span class="sxs-lookup"><span data-stu-id="64125-184">roleIsPresenter</span></span>    | <span data-ttu-id="64125-185">只有其角色为演示者的参与者为演示者。</span><span class="sxs-lookup"><span data-stu-id="64125-185">Only the participants whose role is presenter are presenters.</span></span> |
| <span data-ttu-id="64125-186">组织者</span><span class="sxs-lookup"><span data-stu-id="64125-186">organizer</span></span>          | <span data-ttu-id="64125-187">只有组织者是演示者。</span><span class="sxs-lookup"><span data-stu-id="64125-187">Only the organizer  is a presenter.</span></span>                           |
| <span data-ttu-id="64125-188">向 unknownfuturevalue</span><span class="sxs-lookup"><span data-stu-id="64125-188">unknownFutureValue</span></span> | <span data-ttu-id="64125-189">Unknow 未来值。</span><span class="sxs-lookup"><span data-stu-id="64125-189">Unknow future value.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="64125-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64125-190">JSON representation</span></span>

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

