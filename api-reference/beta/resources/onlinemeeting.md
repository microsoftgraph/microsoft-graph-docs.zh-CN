---
title: onlineMeeting 资源类型
description: 包含有关会议的信息，包括联接 URL、与会者列表和说明。
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 64b2c1880edafe1241367ac91889440a513964d9
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006611"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="516f2-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="516f2-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="516f2-104">包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="516f2-104">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="516f2-105">Methods</span><span class="sxs-lookup"><span data-stu-id="516f2-105">Methods</span></span>

| <span data-ttu-id="516f2-106">方法</span><span class="sxs-lookup"><span data-stu-id="516f2-106">Method</span></span>         | <span data-ttu-id="516f2-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="516f2-107">Return Type</span></span> | <span data-ttu-id="516f2-108">说明</span><span class="sxs-lookup"><span data-stu-id="516f2-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="516f2-109">创建 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="516f2-109">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="516f2-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="516f2-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="516f2-111">创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="516f2-111">Create an online meeting.</span></span> |
| [<span data-ttu-id="516f2-112">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="516f2-112">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="516f2-113">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="516f2-113">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="516f2-114">读取**onlineMeeting**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="516f2-114">Read the properties and relationships of an **onlineMeeting** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="516f2-115">属性</span><span class="sxs-lookup"><span data-stu-id="516f2-115">Properties</span></span>

| <span data-ttu-id="516f2-116">属性</span><span class="sxs-lookup"><span data-stu-id="516f2-116">Property</span></span>                  | <span data-ttu-id="516f2-117">类型</span><span class="sxs-lookup"><span data-stu-id="516f2-117">Type</span></span>                                                   | <span data-ttu-id="516f2-118">说明</span><span class="sxs-lookup"><span data-stu-id="516f2-118">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="516f2-119">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="516f2-119">autoAdmittedUsers</span></span>         | <span data-ttu-id="516f2-120">String</span><span class="sxs-lookup"><span data-stu-id="516f2-120">String</span></span>                                                 | <span data-ttu-id="516f2-121">指定将自动允许加入联机会议的参与者类型的设置。</span><span class="sxs-lookup"><span data-stu-id="516f2-121">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="516f2-122">只读。</span><span class="sxs-lookup"><span data-stu-id="516f2-122">Read-only.</span></span> <span data-ttu-id="516f2-123">可能的值为`everyone`： `everyoneInSameAndFederatedCompany`、 `everyoneInCompany`、 `invitedUsersInCompany`、`organizer`</span><span class="sxs-lookup"><span data-stu-id="516f2-123">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`</span></span>|
| <span data-ttu-id="516f2-124">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="516f2-124">audioConferencing</span></span>         | [<span data-ttu-id="516f2-125">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="516f2-125">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="516f2-126">联机会议的电话访问（拨入）信息。</span><span class="sxs-lookup"><span data-stu-id="516f2-126">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="516f2-127">只读。</span><span class="sxs-lookup"><span data-stu-id="516f2-127">Read-only.</span></span> |
| <span data-ttu-id="516f2-128">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="516f2-128">canceledDateTime</span></span>          | <span data-ttu-id="516f2-129">日期时间</span><span class="sxs-lookup"><span data-stu-id="516f2-129">DateTime</span></span>                                               | <span data-ttu-id="516f2-130">取消会议时的 UTC 时间（以 UTC 为单位）。</span><span class="sxs-lookup"><span data-stu-id="516f2-130">The time in UTC when the meeting was canceled.</span></span> <span data-ttu-id="516f2-131">只读。</span><span class="sxs-lookup"><span data-stu-id="516f2-131">Read-only.</span></span> |
| <span data-ttu-id="516f2-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="516f2-132">chatInfo</span></span>                  | [<span data-ttu-id="516f2-133">chatInfo</span><span class="sxs-lookup"><span data-stu-id="516f2-133">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="516f2-134">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="516f2-134">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="516f2-135">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="516f2-135">creationDateTime</span></span>          | <span data-ttu-id="516f2-136">日期时间</span><span class="sxs-lookup"><span data-stu-id="516f2-136">DateTime</span></span>                                               | <span data-ttu-id="516f2-137">以 UTC 表示的会议创建时间。</span><span class="sxs-lookup"><span data-stu-id="516f2-137">The meeting creation time in UTC.</span></span> <span data-ttu-id="516f2-138">只读。</span><span class="sxs-lookup"><span data-stu-id="516f2-138">Read-only.</span></span> |
| <span data-ttu-id="516f2-139">startDateTime</span><span class="sxs-lookup"><span data-stu-id="516f2-139">startDateTime</span></span>             | <span data-ttu-id="516f2-140">日期时间</span><span class="sxs-lookup"><span data-stu-id="516f2-140">DateTime</span></span>                                               | <span data-ttu-id="516f2-141">以 UTC 表示的会议开始时间。</span><span class="sxs-lookup"><span data-stu-id="516f2-141">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="516f2-142">endDateTime</span><span class="sxs-lookup"><span data-stu-id="516f2-142">endDateTime</span></span>               | <span data-ttu-id="516f2-143">日期时间</span><span class="sxs-lookup"><span data-stu-id="516f2-143">DateTime</span></span>                                               | <span data-ttu-id="516f2-144">以 UTC 表示的会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="516f2-144">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="516f2-145">id</span><span class="sxs-lookup"><span data-stu-id="516f2-145">id</span></span>                        | <span data-ttu-id="516f2-146">字符串</span><span class="sxs-lookup"><span data-stu-id="516f2-146">String</span></span>                                                 | <span data-ttu-id="516f2-147">与联机会议关联的默认 ID。</span><span class="sxs-lookup"><span data-stu-id="516f2-147">The default ID associated with the online meeting.</span></span> <span data-ttu-id="516f2-148">只读。</span><span class="sxs-lookup"><span data-stu-id="516f2-148">Read-only.</span></span> |
| <span data-ttu-id="516f2-149">isCanceled</span><span class="sxs-lookup"><span data-stu-id="516f2-149">isCanceled</span></span>                | <span data-ttu-id="516f2-150">布尔</span><span class="sxs-lookup"><span data-stu-id="516f2-150">Boolean</span></span>                                                | <span data-ttu-id="516f2-151">指示是否已取消会议。</span><span class="sxs-lookup"><span data-stu-id="516f2-151">Indicates whether the meeting has been canceled.</span></span> <span data-ttu-id="516f2-152">只读。</span><span class="sxs-lookup"><span data-stu-id="516f2-152">Read-only.</span></span> |
| <span data-ttu-id="516f2-153">joinUrl</span><span class="sxs-lookup"><span data-stu-id="516f2-153">joinUrl</span></span>                   | <span data-ttu-id="516f2-154">String</span><span class="sxs-lookup"><span data-stu-id="516f2-154">String</span></span>                                                 | <span data-ttu-id="516f2-155">联机会议的加入 URL。</span><span class="sxs-lookup"><span data-stu-id="516f2-155">The join URL of the online meeting.</span></span> <span data-ttu-id="516f2-156">只读。</span><span class="sxs-lookup"><span data-stu-id="516f2-156">Read-only.</span></span>|
| <span data-ttu-id="516f2-157">isBroadcast</span><span class="sxs-lookup"><span data-stu-id="516f2-157">isBroadcast</span></span>               | <span data-ttu-id="516f2-158">布尔</span><span class="sxs-lookup"><span data-stu-id="516f2-158">Boolean</span></span>                                                | <span data-ttu-id="516f2-159">指示会议是否为广播会议。</span><span class="sxs-lookup"><span data-stu-id="516f2-159">Indicates whether the meeting is a broadcast meeting.</span></span> |
| <span data-ttu-id="516f2-160">participants</span><span class="sxs-lookup"><span data-stu-id="516f2-160">participants</span></span>              | [<span data-ttu-id="516f2-161">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="516f2-161">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="516f2-162">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="516f2-162">The participants associated with the online meeting.</span></span>  <span data-ttu-id="516f2-163">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="516f2-163">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="516f2-164">subject</span><span class="sxs-lookup"><span data-stu-id="516f2-164">subject</span></span>                   | <span data-ttu-id="516f2-165">String</span><span class="sxs-lookup"><span data-stu-id="516f2-165">String</span></span>                                                 | <span data-ttu-id="516f2-166">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="516f2-166">The subject of the online meeting.</span></span> |
| <span data-ttu-id="516f2-167">capabilities</span><span class="sxs-lookup"><span data-stu-id="516f2-167">capabilities</span></span>              | <span data-ttu-id="516f2-168">String 集合</span><span class="sxs-lookup"><span data-stu-id="516f2-168">String collection</span></span>                                      | <span data-ttu-id="516f2-169">会议功能的列表。</span><span class="sxs-lookup"><span data-stu-id="516f2-169">The list of meeting capabilities.</span></span> <span data-ttu-id="516f2-170">可能的值是`questionAndAnswer`：。</span><span class="sxs-lookup"><span data-stu-id="516f2-170">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="516f2-171">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="516f2-171">videoTeleconferenceId</span></span>     | <span data-ttu-id="516f2-172">String</span><span class="sxs-lookup"><span data-stu-id="516f2-172">String</span></span>                                                 | <span data-ttu-id="516f2-173">Videio 电话会议 ID。</span><span class="sxs-lookup"><span data-stu-id="516f2-173">The videio teleconferencing ID.</span></span> <span data-ttu-id="516f2-174">只读。</span><span class="sxs-lookup"><span data-stu-id="516f2-174">Read-only.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="516f2-175">autoAdmittedUsers 值</span><span class="sxs-lookup"><span data-stu-id="516f2-175">autoAdmittedUsers values</span></span>
| <span data-ttu-id="516f2-176">值</span><span class="sxs-lookup"><span data-stu-id="516f2-176">Value</span></span> | <span data-ttu-id="516f2-177">说明</span><span class="sxs-lookup"><span data-stu-id="516f2-177">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="516f2-178">组织者</span><span class="sxs-lookup"><span data-stu-id="516f2-178">organizer</span></span> | <span data-ttu-id="516f2-179">仅会议组织者被直接承认。</span><span class="sxs-lookup"><span data-stu-id="516f2-179">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="516f2-180">其他人将在大厅中等待，直到组织者承认</span><span class="sxs-lookup"><span data-stu-id="516f2-180">Everyone else waits in the lobby, until admitted by the organizer</span></span>  |
| <span data-ttu-id="516f2-181">invitedUsersInCompany</span><span class="sxs-lookup"><span data-stu-id="516f2-181">invitedUsersInCompany</span></span> | <span data-ttu-id="516f2-182">会议组织者和组织者邀请的同一家公司中的用户直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="516f2-182">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="516f2-183">其他人在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="516f2-183">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="516f2-184">everyoneInCompany</span><span class="sxs-lookup"><span data-stu-id="516f2-184">everyoneInCompany</span></span> | <span data-ttu-id="516f2-185">与组织者在同一公司中的所有人都直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="516f2-185">Everyone in the same company as the organizer join the meeting directly.</span></span>  <span data-ttu-id="516f2-186">联合匿名用户在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="516f2-186">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="516f2-187">everyoneInSameAndFederatedCompany</span><span class="sxs-lookup"><span data-stu-id="516f2-187">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="516f2-188">与组织者和联合公司在同一公司中的所有人都直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="516f2-188">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="516f2-189">匿名用户在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="516f2-189">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="516f2-190">成员</span><span class="sxs-lookup"><span data-stu-id="516f2-190">everyone</span></span> | <span data-ttu-id="516f2-191">任何用户都是允许的，这意味着每个人（包括匿名用户）都可以直接加入会议，而无需在会议厅中等待。</span><span class="sxs-lookup"><span data-stu-id="516f2-191">Any user is allowed, which means that everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="516f2-192">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="516f2-192">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "autoAdmittedUsers": "everyone | everyoneInSameAndFederatedCompany | everyoneInCompany | invitedUsersInCompany | organizer",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCanceled": false,
  "joinUrl": "String",
  "isBroadcast": false,
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "capabilities": [ "questionAndAnswer" ],
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
