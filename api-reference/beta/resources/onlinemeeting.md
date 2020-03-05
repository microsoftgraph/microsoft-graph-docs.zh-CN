---
title: onlineMeeting 资源类型
description: 包含有关会议的信息，包括联接 URL、与会者列表和说明。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: b6e0848b88427cf0929030f07b163204842c3cd7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522254"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="04aee-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="04aee-103">onlineMeeting resource type</span></span>

<span data-ttu-id="04aee-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="04aee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04aee-105">包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="04aee-105">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="04aee-106">方法</span><span class="sxs-lookup"><span data-stu-id="04aee-106">Methods</span></span>

| <span data-ttu-id="04aee-107">方法</span><span class="sxs-lookup"><span data-stu-id="04aee-107">Method</span></span>         | <span data-ttu-id="04aee-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="04aee-108">Return Type</span></span> | <span data-ttu-id="04aee-109">说明</span><span class="sxs-lookup"><span data-stu-id="04aee-109">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="04aee-110">创建 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="04aee-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="04aee-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="04aee-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="04aee-112">创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="04aee-112">Create an online meeting.</span></span> |
| [<span data-ttu-id="04aee-113">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="04aee-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="04aee-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="04aee-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="04aee-115">读取**onlineMeeting**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="04aee-115">Read the properties and relationships of an **onlineMeeting** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="04aee-116">属性</span><span class="sxs-lookup"><span data-stu-id="04aee-116">Properties</span></span>

| <span data-ttu-id="04aee-117">属性</span><span class="sxs-lookup"><span data-stu-id="04aee-117">Property</span></span>                  | <span data-ttu-id="04aee-118">类型</span><span class="sxs-lookup"><span data-stu-id="04aee-118">Type</span></span>                                                   | <span data-ttu-id="04aee-119">说明</span><span class="sxs-lookup"><span data-stu-id="04aee-119">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="04aee-120">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="04aee-120">autoAdmittedUsers</span></span>         | <span data-ttu-id="04aee-121">String</span><span class="sxs-lookup"><span data-stu-id="04aee-121">String</span></span>                                                 | <span data-ttu-id="04aee-122">指定将自动允许加入联机会议的参与者类型的设置。</span><span class="sxs-lookup"><span data-stu-id="04aee-122">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="04aee-123">可取值为：`everyone`、`everyoneInSameAndFederatedCompany`、`everyoneInCompany`、`invitedUsersInCompany`、`organizer`。</span><span class="sxs-lookup"><span data-stu-id="04aee-123">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span></span> <span data-ttu-id="04aee-124">只读。</span><span class="sxs-lookup"><span data-stu-id="04aee-124">Read-only.</span></span>|
| <span data-ttu-id="04aee-125">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="04aee-125">audioConferencing</span></span>         | [<span data-ttu-id="04aee-126">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="04aee-126">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="04aee-127">联机会议的电话访问（拨入）信息。</span><span class="sxs-lookup"><span data-stu-id="04aee-127">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="04aee-128">只读。</span><span class="sxs-lookup"><span data-stu-id="04aee-128">Read-only.</span></span> |
| <span data-ttu-id="04aee-129">chatInfo</span><span class="sxs-lookup"><span data-stu-id="04aee-129">chatInfo</span></span>                  | [<span data-ttu-id="04aee-130">chatInfo</span><span class="sxs-lookup"><span data-stu-id="04aee-130">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="04aee-131">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="04aee-131">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="04aee-132">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="04aee-132">creationDateTime</span></span>          | <span data-ttu-id="04aee-133">日期时间</span><span class="sxs-lookup"><span data-stu-id="04aee-133">DateTime</span></span>                                               | <span data-ttu-id="04aee-134">以 UTC 表示的会议创建时间。</span><span class="sxs-lookup"><span data-stu-id="04aee-134">The meeting creation time in UTC.</span></span> <span data-ttu-id="04aee-135">只读。</span><span class="sxs-lookup"><span data-stu-id="04aee-135">Read-only.</span></span> |
| <span data-ttu-id="04aee-136">startDateTime</span><span class="sxs-lookup"><span data-stu-id="04aee-136">startDateTime</span></span>             | <span data-ttu-id="04aee-137">日期时间</span><span class="sxs-lookup"><span data-stu-id="04aee-137">DateTime</span></span>                                               | <span data-ttu-id="04aee-138">以 UTC 表示的会议开始时间。</span><span class="sxs-lookup"><span data-stu-id="04aee-138">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="04aee-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="04aee-139">endDateTime</span></span>               | <span data-ttu-id="04aee-140">日期时间</span><span class="sxs-lookup"><span data-stu-id="04aee-140">DateTime</span></span>                                               | <span data-ttu-id="04aee-141">以 UTC 表示的会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="04aee-141">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="04aee-142">id</span><span class="sxs-lookup"><span data-stu-id="04aee-142">id</span></span>                        | <span data-ttu-id="04aee-143">字符串</span><span class="sxs-lookup"><span data-stu-id="04aee-143">String</span></span>                                                 | <span data-ttu-id="04aee-144">与联机会议关联的默认 ID。</span><span class="sxs-lookup"><span data-stu-id="04aee-144">The default ID associated with the online meeting.</span></span> <span data-ttu-id="04aee-145">只读。</span><span class="sxs-lookup"><span data-stu-id="04aee-145">Read-only.</span></span> |
| <span data-ttu-id="04aee-146">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="04aee-146">joinWebUrl</span></span>                   | <span data-ttu-id="04aee-147">String</span><span class="sxs-lookup"><span data-stu-id="04aee-147">String</span></span>                                                 | <span data-ttu-id="04aee-148">联机会议的加入 URL。</span><span class="sxs-lookup"><span data-stu-id="04aee-148">The join URL of the online meeting.</span></span> <span data-ttu-id="04aee-149">只读。</span><span class="sxs-lookup"><span data-stu-id="04aee-149">Read-only.</span></span>|
| <span data-ttu-id="04aee-150">participants</span><span class="sxs-lookup"><span data-stu-id="04aee-150">participants</span></span>              | [<span data-ttu-id="04aee-151">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="04aee-151">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="04aee-152">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="04aee-152">The participants associated with the online meeting.</span></span>  <span data-ttu-id="04aee-153">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="04aee-153">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="04aee-154">subject</span><span class="sxs-lookup"><span data-stu-id="04aee-154">subject</span></span>                   | <span data-ttu-id="04aee-155">String</span><span class="sxs-lookup"><span data-stu-id="04aee-155">String</span></span>                                                 | <span data-ttu-id="04aee-156">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="04aee-156">The subject of the online meeting.</span></span> |
| <span data-ttu-id="04aee-157">capabilities</span><span class="sxs-lookup"><span data-stu-id="04aee-157">capabilities</span></span>              | <span data-ttu-id="04aee-158">String 集合</span><span class="sxs-lookup"><span data-stu-id="04aee-158">String collection</span></span>                                      | <span data-ttu-id="04aee-159">会议功能的列表。</span><span class="sxs-lookup"><span data-stu-id="04aee-159">The list of meeting capabilities.</span></span> <span data-ttu-id="04aee-160">可能的值是`questionAndAnswer`：。</span><span class="sxs-lookup"><span data-stu-id="04aee-160">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="04aee-161">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="04aee-161">videoTeleconferenceId</span></span>     | <span data-ttu-id="04aee-162">String</span><span class="sxs-lookup"><span data-stu-id="04aee-162">String</span></span>                                                 | <span data-ttu-id="04aee-163">视频电话会议 ID。</span><span class="sxs-lookup"><span data-stu-id="04aee-163">The video teleconferencing ID.</span></span> <span data-ttu-id="04aee-164">只读。</span><span class="sxs-lookup"><span data-stu-id="04aee-164">Read-only.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="04aee-165">autoAdmittedUsers 值</span><span class="sxs-lookup"><span data-stu-id="04aee-165">autoAdmittedUsers values</span></span>
| <span data-ttu-id="04aee-166">值</span><span class="sxs-lookup"><span data-stu-id="04aee-166">Value</span></span> | <span data-ttu-id="04aee-167">说明</span><span class="sxs-lookup"><span data-stu-id="04aee-167">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="04aee-168">组织者</span><span class="sxs-lookup"><span data-stu-id="04aee-168">organizer</span></span> | <span data-ttu-id="04aee-169">仅会议组织者被直接承认。</span><span class="sxs-lookup"><span data-stu-id="04aee-169">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="04aee-170">其他人将在大厅中等待，直到组织者承认</span><span class="sxs-lookup"><span data-stu-id="04aee-170">Everyone else waits in the lobby, until admitted by the organizer</span></span>  |
| <span data-ttu-id="04aee-171">invitedUsersInCompany</span><span class="sxs-lookup"><span data-stu-id="04aee-171">invitedUsersInCompany</span></span> | <span data-ttu-id="04aee-172">会议组织者和组织者邀请的同一家公司中的用户直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="04aee-172">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="04aee-173">其他人在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="04aee-173">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="04aee-174">everyoneInCompany</span><span class="sxs-lookup"><span data-stu-id="04aee-174">everyoneInCompany</span></span> | <span data-ttu-id="04aee-175">与组织者在同一公司中的所有人都直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="04aee-175">Everyone in the same company as the organizer join the meeting directly.</span></span>  <span data-ttu-id="04aee-176">联合匿名用户在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="04aee-176">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="04aee-177">everyoneInSameAndFederatedCompany</span><span class="sxs-lookup"><span data-stu-id="04aee-177">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="04aee-178">与组织者和联合公司在同一公司中的所有人都直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="04aee-178">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="04aee-179">匿名用户在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="04aee-179">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="04aee-180">成员</span><span class="sxs-lookup"><span data-stu-id="04aee-180">everyone</span></span> | <span data-ttu-id="04aee-181">任何用户都是允许的，这意味着每个人（包括匿名用户）都可以直接加入会议，而无需在会议厅中等待。</span><span class="sxs-lookup"><span data-stu-id="04aee-181">Any user is allowed, which means that everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="04aee-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04aee-182">JSON representation</span></span>

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
