---
title: onlineMeeting 资源类型
description: 捕获有关会议的信息，包括联接 URL、与会者列表和说明。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-cloud communications
doc_type: resourcePageType
ms.openlocfilehash: 5cc62c4caa564aa071ffc6b206d5494814b0cb53
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37969799"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="d64a7-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="d64a7-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d64a7-104">包含有关会议的信息，包括联接 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="d64a7-104">Contains information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="d64a7-105">方法</span><span class="sxs-lookup"><span data-stu-id="d64a7-105">Methods</span></span>

| <span data-ttu-id="d64a7-106">方法</span><span class="sxs-lookup"><span data-stu-id="d64a7-106">Method</span></span>         | <span data-ttu-id="d64a7-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="d64a7-107">Return Type</span></span> | <span data-ttu-id="d64a7-108">说明</span><span class="sxs-lookup"><span data-stu-id="d64a7-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="d64a7-109">创建 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="d64a7-109">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="d64a7-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="d64a7-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="d64a7-111">创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="d64a7-111">Create an online meeting.</span></span> |
| [<span data-ttu-id="d64a7-112">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="d64a7-112">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="d64a7-113">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="d64a7-113">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="d64a7-114">读取**onlineMeeting**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d64a7-114">Read the properties and relationships of an **onlineMeeting** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d64a7-115">属性</span><span class="sxs-lookup"><span data-stu-id="d64a7-115">Properties</span></span>

| <span data-ttu-id="d64a7-116">属性</span><span class="sxs-lookup"><span data-stu-id="d64a7-116">Property</span></span>                  | <span data-ttu-id="d64a7-117">类型</span><span class="sxs-lookup"><span data-stu-id="d64a7-117">Type</span></span>                                                   | <span data-ttu-id="d64a7-118">说明</span><span class="sxs-lookup"><span data-stu-id="d64a7-118">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d64a7-119">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="d64a7-119">autoAdmittedUsers</span></span>         | <span data-ttu-id="d64a7-120">String</span><span class="sxs-lookup"><span data-stu-id="d64a7-120">String</span></span>                                                 | <span data-ttu-id="d64a7-121">指定将自动允许加入联机会议的参与者类型的设置。</span><span class="sxs-lookup"><span data-stu-id="d64a7-121">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="d64a7-122">只读。</span><span class="sxs-lookup"><span data-stu-id="d64a7-122">Read-only.</span></span> <span data-ttu-id="d64a7-123">可能的值为`everyone`： `everyoneInSameAndFederatedCompany`、 `everyoneInCompany`、 `invitedUsersInCompany`、`organizer`</span><span class="sxs-lookup"><span data-stu-id="d64a7-123">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`</span></span>|
| <span data-ttu-id="d64a7-124">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="d64a7-124">audioConferencing</span></span>         | [<span data-ttu-id="d64a7-125">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="d64a7-125">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="d64a7-126">联机会议的电话访问（拨入）信息。</span><span class="sxs-lookup"><span data-stu-id="d64a7-126">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="d64a7-127">只读。</span><span class="sxs-lookup"><span data-stu-id="d64a7-127">Read-only.</span></span> |
| <span data-ttu-id="d64a7-128">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="d64a7-128">canceledDateTime</span></span>          | <span data-ttu-id="d64a7-129">日期时间</span><span class="sxs-lookup"><span data-stu-id="d64a7-129">DateTime</span></span>                                               | <span data-ttu-id="d64a7-130">取消会议时的 UTC 时间（以 UTC 为单位）。</span><span class="sxs-lookup"><span data-stu-id="d64a7-130">The time in UTC when the meeting was canceled.</span></span> <span data-ttu-id="d64a7-131">只读。</span><span class="sxs-lookup"><span data-stu-id="d64a7-131">Read-only.</span></span> |
| <span data-ttu-id="d64a7-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="d64a7-132">chatInfo</span></span>                  | [<span data-ttu-id="d64a7-133">chatInfo</span><span class="sxs-lookup"><span data-stu-id="d64a7-133">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="d64a7-134">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="d64a7-134">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="d64a7-135">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="d64a7-135">creationDateTime</span></span>          | <span data-ttu-id="d64a7-136">日期时间</span><span class="sxs-lookup"><span data-stu-id="d64a7-136">DateTime</span></span>                                               | <span data-ttu-id="d64a7-137">以 UTC 表示的会议创建时间。</span><span class="sxs-lookup"><span data-stu-id="d64a7-137">The meeting creation time in UTC.</span></span> <span data-ttu-id="d64a7-138">只读。</span><span class="sxs-lookup"><span data-stu-id="d64a7-138">Read-only.</span></span> |
| <span data-ttu-id="d64a7-139">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d64a7-139">startDateTime</span></span>             | <span data-ttu-id="d64a7-140">日期时间</span><span class="sxs-lookup"><span data-stu-id="d64a7-140">DateTime</span></span>                                               | <span data-ttu-id="d64a7-141">以 UTC 表示的会议开始时间。</span><span class="sxs-lookup"><span data-stu-id="d64a7-141">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="d64a7-142">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d64a7-142">endDateTime</span></span>               | <span data-ttu-id="d64a7-143">日期时间</span><span class="sxs-lookup"><span data-stu-id="d64a7-143">DateTime</span></span>                                               | <span data-ttu-id="d64a7-144">以 UTC 表示的会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="d64a7-144">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="d64a7-145">id</span><span class="sxs-lookup"><span data-stu-id="d64a7-145">id</span></span>                        | <span data-ttu-id="d64a7-146">字符串</span><span class="sxs-lookup"><span data-stu-id="d64a7-146">String</span></span>                                                 | <span data-ttu-id="d64a7-147">与联机会议关联的默认 ID。</span><span class="sxs-lookup"><span data-stu-id="d64a7-147">The default ID associated with the online meeting.</span></span> <span data-ttu-id="d64a7-148">只读。</span><span class="sxs-lookup"><span data-stu-id="d64a7-148">Read-only.</span></span> |
| <span data-ttu-id="d64a7-149">isCanceled</span><span class="sxs-lookup"><span data-stu-id="d64a7-149">isCanceled</span></span>                | <span data-ttu-id="d64a7-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="d64a7-150">Boolean</span></span>                                                | <span data-ttu-id="d64a7-151">指示是否已取消会议。</span><span class="sxs-lookup"><span data-stu-id="d64a7-151">Indicates whether the meeting has been canceled.</span></span> <span data-ttu-id="d64a7-152">只读。</span><span class="sxs-lookup"><span data-stu-id="d64a7-152">Read-only.</span></span> |
| <span data-ttu-id="d64a7-153">joinUrl</span><span class="sxs-lookup"><span data-stu-id="d64a7-153">joinUrl</span></span>                   | <span data-ttu-id="d64a7-154">String</span><span class="sxs-lookup"><span data-stu-id="d64a7-154">String</span></span>                                                 | <span data-ttu-id="d64a7-155">联机会议的加入 URL。</span><span class="sxs-lookup"><span data-stu-id="d64a7-155">The join URL of the online meeting.</span></span> <span data-ttu-id="d64a7-156">只读。</span><span class="sxs-lookup"><span data-stu-id="d64a7-156">Read-only.</span></span>|
| <span data-ttu-id="d64a7-157">isBroadcast</span><span class="sxs-lookup"><span data-stu-id="d64a7-157">isBroadcast</span></span>               | <span data-ttu-id="d64a7-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="d64a7-158">Boolean</span></span>                                                | <span data-ttu-id="d64a7-159">用于确定是否为广播会议的标志。</span><span class="sxs-lookup"><span data-stu-id="d64a7-159">The flag to determine whether it's a broadcast meeting.</span></span> |
| <span data-ttu-id="d64a7-160">participants</span><span class="sxs-lookup"><span data-stu-id="d64a7-160">participants</span></span>              | [<span data-ttu-id="d64a7-161">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="d64a7-161">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="d64a7-162">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="d64a7-162">The participants associated with the online meeting.</span></span>  <span data-ttu-id="d64a7-163">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="d64a7-163">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="d64a7-164">subject</span><span class="sxs-lookup"><span data-stu-id="d64a7-164">subject</span></span>                   | <span data-ttu-id="d64a7-165">String</span><span class="sxs-lookup"><span data-stu-id="d64a7-165">String</span></span>                                                 | <span data-ttu-id="d64a7-166">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="d64a7-166">The subject of the online meeting.</span></span> |
| <span data-ttu-id="d64a7-167">capabilities</span><span class="sxs-lookup"><span data-stu-id="d64a7-167">capabilities</span></span>              | <span data-ttu-id="d64a7-168">String collection</span><span class="sxs-lookup"><span data-stu-id="d64a7-168">String collection</span></span>                                      | <span data-ttu-id="d64a7-169">会议功能的列表。</span><span class="sxs-lookup"><span data-stu-id="d64a7-169">The list of meeting capabilities.</span></span> <span data-ttu-id="d64a7-170">可能的值是`questionAndAnswer`：。</span><span class="sxs-lookup"><span data-stu-id="d64a7-170">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="d64a7-171">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="d64a7-171">videoTeleconferenceId</span></span>     | <span data-ttu-id="d64a7-172">String</span><span class="sxs-lookup"><span data-stu-id="d64a7-172">String</span></span>                                                 | <span data-ttu-id="d64a7-173">Videio 电话会议 ID。</span><span class="sxs-lookup"><span data-stu-id="d64a7-173">The videio teleconferencing ID.</span></span> <span data-ttu-id="d64a7-174">只读。</span><span class="sxs-lookup"><span data-stu-id="d64a7-174">Read-only.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="d64a7-175">autoAdmittedUsers 值</span><span class="sxs-lookup"><span data-stu-id="d64a7-175">autoAdmittedUsers values</span></span>
| <span data-ttu-id="d64a7-176">值</span><span class="sxs-lookup"><span data-stu-id="d64a7-176">Value</span></span> | <span data-ttu-id="d64a7-177">Description</span><span class="sxs-lookup"><span data-stu-id="d64a7-177">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d64a7-178">组织者</span><span class="sxs-lookup"><span data-stu-id="d64a7-178">organizer</span></span> | <span data-ttu-id="d64a7-179">仅会议组织者被直接承认。</span><span class="sxs-lookup"><span data-stu-id="d64a7-179">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="d64a7-180">其他人将在大厅中等待，直到组织者承认。</span><span class="sxs-lookup"><span data-stu-id="d64a7-180">Everyone else waits in the lobby, until admitted by the organizer.</span></span>  |
| <span data-ttu-id="d64a7-181">invitedUsersInCompany</span><span class="sxs-lookup"><span data-stu-id="d64a7-181">invitedUsersInCompany</span></span> | <span data-ttu-id="d64a7-182">会议组织者和组织者邀请的同一家公司中的用户直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="d64a7-182">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="d64a7-183">其他人在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="d64a7-183">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="d64a7-184">everyoneInCompany</span><span class="sxs-lookup"><span data-stu-id="d64a7-184">everyoneInCompany</span></span> | <span data-ttu-id="d64a7-185">与组织者在同一公司中的所有人都直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="d64a7-185">Everyone in the same company as the organizer join the meeting directly.</span></span> <span data-ttu-id="d64a7-186">联合匿名用户在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="d64a7-186">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="d64a7-187">everyoneInSameAndFederatedCompany</span><span class="sxs-lookup"><span data-stu-id="d64a7-187">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="d64a7-188">与组织者和联合公司在同一公司中的所有人都直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="d64a7-188">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="d64a7-189">匿名用户在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="d64a7-189">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="d64a7-190">成员</span><span class="sxs-lookup"><span data-stu-id="d64a7-190">everyone</span></span> | <span data-ttu-id="d64a7-191">允许任何用户。</span><span class="sxs-lookup"><span data-stu-id="d64a7-191">Any user is allowed.</span></span> <span data-ttu-id="d64a7-192">任何人（包括匿名用户）都可以直接加入会议，而无需在会议厅中等待。</span><span class="sxs-lookup"><span data-stu-id="d64a7-192">Everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="d64a7-193">关系</span><span class="sxs-lookup"><span data-stu-id="d64a7-193">Relationships</span></span>
<span data-ttu-id="d64a7-194">无。</span><span class="sxs-lookup"><span data-stu-id="d64a7-194">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d64a7-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d64a7-195">JSON representation</span></span>

<span data-ttu-id="d64a7-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d64a7-196">The following is a JSON representation of the resource.</span></span>

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
