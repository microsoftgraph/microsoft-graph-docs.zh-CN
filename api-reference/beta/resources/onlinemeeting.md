---
title: onlineMeeting 资源类型
description: 包含有关会议的信息，包括联接 URL、与会者列表和说明。
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: e7cae71f220a2a519908e3af890029a2da555577
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866684"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="157ca-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="157ca-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="157ca-104">包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="157ca-104">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="157ca-105">方法</span><span class="sxs-lookup"><span data-stu-id="157ca-105">Methods</span></span>

| <span data-ttu-id="157ca-106">方法</span><span class="sxs-lookup"><span data-stu-id="157ca-106">Method</span></span>         | <span data-ttu-id="157ca-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="157ca-107">Return Type</span></span> | <span data-ttu-id="157ca-108">说明</span><span class="sxs-lookup"><span data-stu-id="157ca-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="157ca-109">创建 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="157ca-109">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="157ca-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="157ca-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="157ca-111">创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="157ca-111">Create an online meeting.</span></span> |
| [<span data-ttu-id="157ca-112">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="157ca-112">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="157ca-113">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="157ca-113">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="157ca-114">读取**onlineMeeting**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="157ca-114">Read the properties and relationships of an **onlineMeeting** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="157ca-115">属性</span><span class="sxs-lookup"><span data-stu-id="157ca-115">Properties</span></span>

| <span data-ttu-id="157ca-116">属性</span><span class="sxs-lookup"><span data-stu-id="157ca-116">Property</span></span>                  | <span data-ttu-id="157ca-117">类型</span><span class="sxs-lookup"><span data-stu-id="157ca-117">Type</span></span>                                                   | <span data-ttu-id="157ca-118">说明</span><span class="sxs-lookup"><span data-stu-id="157ca-118">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="157ca-119">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="157ca-119">autoAdmittedUsers</span></span>         | <span data-ttu-id="157ca-120">String</span><span class="sxs-lookup"><span data-stu-id="157ca-120">String</span></span>                                                 | <span data-ttu-id="157ca-121">指定将自动允许加入联机会议的参与者类型的设置。</span><span class="sxs-lookup"><span data-stu-id="157ca-121">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="157ca-122">可取值为：`everyone`、`everyoneInSameAndFederatedCompany`、`everyoneInCompany`、`invitedUsersInCompany`、`organizer`。</span><span class="sxs-lookup"><span data-stu-id="157ca-122">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span></span> <span data-ttu-id="157ca-123">只读。</span><span class="sxs-lookup"><span data-stu-id="157ca-123">Read-only.</span></span>|
| <span data-ttu-id="157ca-124">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="157ca-124">audioConferencing</span></span>         | [<span data-ttu-id="157ca-125">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="157ca-125">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="157ca-126">联机会议的电话访问（拨入）信息。</span><span class="sxs-lookup"><span data-stu-id="157ca-126">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="157ca-127">只读。</span><span class="sxs-lookup"><span data-stu-id="157ca-127">Read-only.</span></span> |
| <span data-ttu-id="157ca-128">chatInfo</span><span class="sxs-lookup"><span data-stu-id="157ca-128">chatInfo</span></span>                  | [<span data-ttu-id="157ca-129">chatInfo</span><span class="sxs-lookup"><span data-stu-id="157ca-129">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="157ca-130">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="157ca-130">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="157ca-131">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="157ca-131">creationDateTime</span></span>          | <span data-ttu-id="157ca-132">日期时间</span><span class="sxs-lookup"><span data-stu-id="157ca-132">DateTime</span></span>                                               | <span data-ttu-id="157ca-133">以 UTC 表示的会议创建时间。</span><span class="sxs-lookup"><span data-stu-id="157ca-133">The meeting creation time in UTC.</span></span> <span data-ttu-id="157ca-134">只读。</span><span class="sxs-lookup"><span data-stu-id="157ca-134">Read-only.</span></span> |
| <span data-ttu-id="157ca-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="157ca-135">startDateTime</span></span>             | <span data-ttu-id="157ca-136">日期时间</span><span class="sxs-lookup"><span data-stu-id="157ca-136">DateTime</span></span>                                               | <span data-ttu-id="157ca-137">以 UTC 表示的会议开始时间。</span><span class="sxs-lookup"><span data-stu-id="157ca-137">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="157ca-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="157ca-138">endDateTime</span></span>               | <span data-ttu-id="157ca-139">日期时间</span><span class="sxs-lookup"><span data-stu-id="157ca-139">DateTime</span></span>                                               | <span data-ttu-id="157ca-140">以 UTC 表示的会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="157ca-140">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="157ca-141">id</span><span class="sxs-lookup"><span data-stu-id="157ca-141">id</span></span>                        | <span data-ttu-id="157ca-142">字符串</span><span class="sxs-lookup"><span data-stu-id="157ca-142">String</span></span>                                                 | <span data-ttu-id="157ca-143">与联机会议关联的默认 ID。</span><span class="sxs-lookup"><span data-stu-id="157ca-143">The default ID associated with the online meeting.</span></span> <span data-ttu-id="157ca-144">只读。</span><span class="sxs-lookup"><span data-stu-id="157ca-144">Read-only.</span></span> |
| <span data-ttu-id="157ca-145">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="157ca-145">joinWebUrl</span></span>                   | <span data-ttu-id="157ca-146">String</span><span class="sxs-lookup"><span data-stu-id="157ca-146">String</span></span>                                                 | <span data-ttu-id="157ca-147">联机会议的加入 URL。</span><span class="sxs-lookup"><span data-stu-id="157ca-147">The join URL of the online meeting.</span></span> <span data-ttu-id="157ca-148">只读。</span><span class="sxs-lookup"><span data-stu-id="157ca-148">Read-only.</span></span>|
| <span data-ttu-id="157ca-149">participants</span><span class="sxs-lookup"><span data-stu-id="157ca-149">participants</span></span>              | [<span data-ttu-id="157ca-150">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="157ca-150">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="157ca-151">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="157ca-151">The participants associated with the online meeting.</span></span>  <span data-ttu-id="157ca-152">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="157ca-152">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="157ca-153">subject</span><span class="sxs-lookup"><span data-stu-id="157ca-153">subject</span></span>                   | <span data-ttu-id="157ca-154">String</span><span class="sxs-lookup"><span data-stu-id="157ca-154">String</span></span>                                                 | <span data-ttu-id="157ca-155">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="157ca-155">The subject of the online meeting.</span></span> |
| <span data-ttu-id="157ca-156">capabilities</span><span class="sxs-lookup"><span data-stu-id="157ca-156">capabilities</span></span>              | <span data-ttu-id="157ca-157">String collection</span><span class="sxs-lookup"><span data-stu-id="157ca-157">String collection</span></span>                                      | <span data-ttu-id="157ca-158">会议功能的列表。</span><span class="sxs-lookup"><span data-stu-id="157ca-158">The list of meeting capabilities.</span></span> <span data-ttu-id="157ca-159">可能的值是`questionAndAnswer`：。</span><span class="sxs-lookup"><span data-stu-id="157ca-159">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="157ca-160">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="157ca-160">videoTeleconferenceId</span></span>     | <span data-ttu-id="157ca-161">String</span><span class="sxs-lookup"><span data-stu-id="157ca-161">String</span></span>                                                 | <span data-ttu-id="157ca-162">视频电话会议 ID。</span><span class="sxs-lookup"><span data-stu-id="157ca-162">The video teleconferencing ID.</span></span> <span data-ttu-id="157ca-163">只读。</span><span class="sxs-lookup"><span data-stu-id="157ca-163">Read-only.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="157ca-164">autoAdmittedUsers 值</span><span class="sxs-lookup"><span data-stu-id="157ca-164">autoAdmittedUsers values</span></span>
| <span data-ttu-id="157ca-165">值</span><span class="sxs-lookup"><span data-stu-id="157ca-165">Value</span></span> | <span data-ttu-id="157ca-166">说明</span><span class="sxs-lookup"><span data-stu-id="157ca-166">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="157ca-167">组织者</span><span class="sxs-lookup"><span data-stu-id="157ca-167">organizer</span></span> | <span data-ttu-id="157ca-168">仅会议组织者被直接承认。</span><span class="sxs-lookup"><span data-stu-id="157ca-168">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="157ca-169">其他人将在大厅中等待，直到组织者承认</span><span class="sxs-lookup"><span data-stu-id="157ca-169">Everyone else waits in the lobby, until admitted by the organizer</span></span>  |
| <span data-ttu-id="157ca-170">invitedUsersInCompany</span><span class="sxs-lookup"><span data-stu-id="157ca-170">invitedUsersInCompany</span></span> | <span data-ttu-id="157ca-171">会议组织者和组织者邀请的同一家公司中的用户直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="157ca-171">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="157ca-172">其他人在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="157ca-172">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="157ca-173">everyoneInCompany</span><span class="sxs-lookup"><span data-stu-id="157ca-173">everyoneInCompany</span></span> | <span data-ttu-id="157ca-174">与组织者在同一公司中的所有人都直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="157ca-174">Everyone in the same company as the organizer join the meeting directly.</span></span>  <span data-ttu-id="157ca-175">联合匿名用户在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="157ca-175">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="157ca-176">everyoneInSameAndFederatedCompany</span><span class="sxs-lookup"><span data-stu-id="157ca-176">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="157ca-177">与组织者和联合公司在同一公司中的所有人都直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="157ca-177">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="157ca-178">匿名用户在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="157ca-178">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="157ca-179">成员</span><span class="sxs-lookup"><span data-stu-id="157ca-179">everyone</span></span> | <span data-ttu-id="157ca-180">任何用户都是允许的，这意味着每个人（包括匿名用户）都可以直接加入会议，而无需在会议厅中等待。</span><span class="sxs-lookup"><span data-stu-id="157ca-180">Any user is allowed, which means that everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="157ca-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="157ca-181">JSON representation</span></span>

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
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
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
