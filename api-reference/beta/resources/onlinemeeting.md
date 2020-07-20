---
title: onlineMeeting 资源类型
description: 包含有关会议的信息，包括联接 URL、与会者列表和说明。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 35759e9be3d2ea4aeade45f6e6b040a2b45f3be9
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183909"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="55616-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="55616-103">onlineMeeting resource type</span></span>

<span data-ttu-id="55616-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55616-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55616-105">包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="55616-105">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="55616-106">方法</span><span class="sxs-lookup"><span data-stu-id="55616-106">Methods</span></span>

| <span data-ttu-id="55616-107">方法</span><span class="sxs-lookup"><span data-stu-id="55616-107">Method</span></span>         | <span data-ttu-id="55616-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="55616-108">Return Type</span></span> | <span data-ttu-id="55616-109">说明</span><span class="sxs-lookup"><span data-stu-id="55616-109">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="55616-110">创建</span><span class="sxs-lookup"><span data-stu-id="55616-110">Create</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="55616-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="55616-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="55616-112">创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="55616-112">Create an online meeting.</span></span> |
| [<span data-ttu-id="55616-113">获取</span><span class="sxs-lookup"><span data-stu-id="55616-113">Get</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="55616-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="55616-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="55616-115">读取**onlineMeeting**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="55616-115">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="55616-116">创建或获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="55616-116">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="55616-117">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="55616-117">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="55616-118">使用自定义外部 ID 创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="55616-118">Create an online meeting with a custom, external ID.</span></span> <span data-ttu-id="55616-119">如果会议已存在，请检索其属性。</span><span class="sxs-lookup"><span data-stu-id="55616-119">If the meeting already exists, retrieve its properties.</span></span> |
| [<span data-ttu-id="55616-120">更新</span><span class="sxs-lookup"><span data-stu-id="55616-120">Update</span></span>](../api/onlinemeeting-update.md) | [<span data-ttu-id="55616-121">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="55616-121">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="55616-122">更新联机会议的 " **startDateTime**"、" **endDateTime**"、"**主题**" 和 "**参与者**" 属性。</span><span class="sxs-lookup"><span data-stu-id="55616-122">Update the **startDateTime**, **endDateTime**, **subject**, and **participants** properties of an online meeting.</span></span> |

## <a name="properties"></a><span data-ttu-id="55616-123">属性</span><span class="sxs-lookup"><span data-stu-id="55616-123">Properties</span></span>

| <span data-ttu-id="55616-124">属性</span><span class="sxs-lookup"><span data-stu-id="55616-124">Property</span></span>                  | <span data-ttu-id="55616-125">类型</span><span class="sxs-lookup"><span data-stu-id="55616-125">Type</span></span>                                                   | <span data-ttu-id="55616-126">说明</span><span class="sxs-lookup"><span data-stu-id="55616-126">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="55616-127">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="55616-127">autoAdmittedUsers</span></span>         | <span data-ttu-id="55616-128">String</span><span class="sxs-lookup"><span data-stu-id="55616-128">String</span></span>                                                 | <span data-ttu-id="55616-129">指定将自动允许加入联机会议的参与者类型的设置。</span><span class="sxs-lookup"><span data-stu-id="55616-129">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="55616-130">可取值为：`everyone`、`everyoneInSameAndFederatedCompany`、`everyoneInCompany`、`invitedUsersInCompany`、`organizer`。</span><span class="sxs-lookup"><span data-stu-id="55616-130">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span></span> <span data-ttu-id="55616-131">只读。</span><span class="sxs-lookup"><span data-stu-id="55616-131">Read-only.</span></span>|
| <span data-ttu-id="55616-132">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="55616-132">audioConferencing</span></span>         | [<span data-ttu-id="55616-133">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="55616-133">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="55616-134">联机会议的电话访问（拨入）信息。</span><span class="sxs-lookup"><span data-stu-id="55616-134">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="55616-135">只读。</span><span class="sxs-lookup"><span data-stu-id="55616-135">Read-only.</span></span> |
| <span data-ttu-id="55616-136">chatInfo</span><span class="sxs-lookup"><span data-stu-id="55616-136">chatInfo</span></span>                  | [<span data-ttu-id="55616-137">chatInfo</span><span class="sxs-lookup"><span data-stu-id="55616-137">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="55616-138">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="55616-138">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="55616-139">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="55616-139">creationDateTime</span></span>          | <span data-ttu-id="55616-140">DateTime</span><span class="sxs-lookup"><span data-stu-id="55616-140">DateTime</span></span>                                               | <span data-ttu-id="55616-141">以 UTC 表示的会议创建时间。</span><span class="sxs-lookup"><span data-stu-id="55616-141">The meeting creation time in UTC.</span></span> <span data-ttu-id="55616-142">只读。</span><span class="sxs-lookup"><span data-stu-id="55616-142">Read-only.</span></span> |
| <span data-ttu-id="55616-143">startDateTime</span><span class="sxs-lookup"><span data-stu-id="55616-143">startDateTime</span></span>             | <span data-ttu-id="55616-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="55616-144">DateTime</span></span>                                               | <span data-ttu-id="55616-145">以 UTC 表示的会议开始时间。</span><span class="sxs-lookup"><span data-stu-id="55616-145">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="55616-146">endDateTime</span><span class="sxs-lookup"><span data-stu-id="55616-146">endDateTime</span></span>               | <span data-ttu-id="55616-147">DateTime</span><span class="sxs-lookup"><span data-stu-id="55616-147">DateTime</span></span>                                               | <span data-ttu-id="55616-148">以 UTC 表示的会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="55616-148">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="55616-149">id</span><span class="sxs-lookup"><span data-stu-id="55616-149">id</span></span>                        | <span data-ttu-id="55616-150">字符串</span><span class="sxs-lookup"><span data-stu-id="55616-150">String</span></span>                                                 | <span data-ttu-id="55616-151">与联机会议关联的默认 ID。</span><span class="sxs-lookup"><span data-stu-id="55616-151">The default ID associated with the online meeting.</span></span> <span data-ttu-id="55616-152">只读。</span><span class="sxs-lookup"><span data-stu-id="55616-152">Read-only.</span></span> |
| <span data-ttu-id="55616-153">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="55616-153">joinWebUrl</span></span>                   | <span data-ttu-id="55616-154">String</span><span class="sxs-lookup"><span data-stu-id="55616-154">String</span></span>                                                 | <span data-ttu-id="55616-155">联机会议的加入 URL。</span><span class="sxs-lookup"><span data-stu-id="55616-155">The join URL of the online meeting.</span></span> <span data-ttu-id="55616-156">只读。</span><span class="sxs-lookup"><span data-stu-id="55616-156">Read-only.</span></span>|
| <span data-ttu-id="55616-157">participants</span><span class="sxs-lookup"><span data-stu-id="55616-157">participants</span></span>              | [<span data-ttu-id="55616-158">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="55616-158">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="55616-159">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="55616-159">The participants associated with the online meeting.</span></span>  <span data-ttu-id="55616-160">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="55616-160">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="55616-161">主题</span><span class="sxs-lookup"><span data-stu-id="55616-161">subject</span></span>                   | <span data-ttu-id="55616-162">String</span><span class="sxs-lookup"><span data-stu-id="55616-162">String</span></span>                                                 | <span data-ttu-id="55616-163">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="55616-163">The subject of the online meeting.</span></span> |
| <span data-ttu-id="55616-164">capabilities</span><span class="sxs-lookup"><span data-stu-id="55616-164">capabilities</span></span>              | <span data-ttu-id="55616-165">String 集合</span><span class="sxs-lookup"><span data-stu-id="55616-165">String collection</span></span>                                      | <span data-ttu-id="55616-166">会议功能的列表。</span><span class="sxs-lookup"><span data-stu-id="55616-166">The list of meeting capabilities.</span></span> <span data-ttu-id="55616-167">可能的值是： `questionAndAnswer` 。</span><span class="sxs-lookup"><span data-stu-id="55616-167">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="55616-168">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="55616-168">videoTeleconferenceId</span></span>     | <span data-ttu-id="55616-169">String</span><span class="sxs-lookup"><span data-stu-id="55616-169">String</span></span>                                                 | <span data-ttu-id="55616-170">视频电话会议 ID。</span><span class="sxs-lookup"><span data-stu-id="55616-170">The video teleconferencing ID.</span></span> <span data-ttu-id="55616-171">只读。</span><span class="sxs-lookup"><span data-stu-id="55616-171">Read-only.</span></span> |
| <span data-ttu-id="55616-172">joinInformation</span><span class="sxs-lookup"><span data-stu-id="55616-172">joinInformation</span></span> | [<span data-ttu-id="55616-173">itemBody</span><span class="sxs-lookup"><span data-stu-id="55616-173">itemBody</span></span>](itembody.md) | <span data-ttu-id="55616-174">在 "Accept-Language" 请求 HTTP 标头中指定的语言和区域设置变量形式的联接信息。</span><span class="sxs-lookup"><span data-stu-id="55616-174">The join information in the language and locale variant specified in 'Accept-Language' request HTTP header.</span></span> <span data-ttu-id="55616-175">只读</span><span class="sxs-lookup"><span data-stu-id="55616-175">Read-only</span></span> |
| <span data-ttu-id="55616-176">externalId</span><span class="sxs-lookup"><span data-stu-id="55616-176">externalId</span></span>                | <span data-ttu-id="55616-177">String</span><span class="sxs-lookup"><span data-stu-id="55616-177">String</span></span>                                                 | <span data-ttu-id="55616-178">外部 ID。</span><span class="sxs-lookup"><span data-stu-id="55616-178">The external ID.</span></span> <span data-ttu-id="55616-179">自定义 ID。</span><span class="sxs-lookup"><span data-stu-id="55616-179">A custom ID.</span></span> <span data-ttu-id="55616-180">可选。</span><span class="sxs-lookup"><span data-stu-id="55616-180">Optional.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="55616-181">autoAdmittedUsers 值</span><span class="sxs-lookup"><span data-stu-id="55616-181">autoAdmittedUsers values</span></span>
| <span data-ttu-id="55616-182">值</span><span class="sxs-lookup"><span data-stu-id="55616-182">Value</span></span> | <span data-ttu-id="55616-183">说明</span><span class="sxs-lookup"><span data-stu-id="55616-183">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- |
| <span data-ttu-id="55616-184">组织者</span><span class="sxs-lookup"><span data-stu-id="55616-184">organizer</span></span> | <span data-ttu-id="55616-185">仅会议组织者被直接承认。</span><span class="sxs-lookup"><span data-stu-id="55616-185">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="55616-186">其他人将在大厅中等待，直到组织者承认</span><span class="sxs-lookup"><span data-stu-id="55616-186">Everyone else waits in the lobby, until admitted by the organizer</span></span>  |
| <span data-ttu-id="55616-187">invitedUsersInCompany</span><span class="sxs-lookup"><span data-stu-id="55616-187">invitedUsersInCompany</span></span> | <span data-ttu-id="55616-188">会议组织者和组织者邀请的同一家公司中的用户直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="55616-188">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="55616-189">其他人在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="55616-189">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="55616-190">everyoneInCompany</span><span class="sxs-lookup"><span data-stu-id="55616-190">everyoneInCompany</span></span> | <span data-ttu-id="55616-191">与组织者在同一公司中的所有人都直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="55616-191">Everyone in the same company as the organizer join the meeting directly.</span></span>  <span data-ttu-id="55616-192">联合匿名用户在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="55616-192">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="55616-193">everyoneInSameAndFederatedCompany</span><span class="sxs-lookup"><span data-stu-id="55616-193">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="55616-194">与组织者和联合公司在同一公司中的所有人都直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="55616-194">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="55616-195">匿名用户在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="55616-195">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="55616-196">成员</span><span class="sxs-lookup"><span data-stu-id="55616-196">everyone</span></span> | <span data-ttu-id="55616-197">任何用户都是允许的，这意味着每个人（包括匿名用户）都可以直接加入会议，而无需在会议厅中等待。</span><span class="sxs-lookup"><span data-stu-id="55616-197">Any user is allowed, which means that everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="55616-198">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55616-198">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "externalId"
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
