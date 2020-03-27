---
title: onlineMeeting 资源类型
description: 包含有关会议的信息，包括联接 URL、与会者列表和说明。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: c0a1bac4fa0a80435d381d62aaa4b90df3352c33
ms.sourcegitcommit: 2ac179fb774a15c9e9c01502e59c76efb57803a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/27/2020
ms.locfileid: "42986101"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="0906f-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="0906f-103">onlineMeeting resource type</span></span>

<span data-ttu-id="0906f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0906f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0906f-105">包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="0906f-105">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="0906f-106">方法</span><span class="sxs-lookup"><span data-stu-id="0906f-106">Methods</span></span>

| <span data-ttu-id="0906f-107">方法</span><span class="sxs-lookup"><span data-stu-id="0906f-107">Method</span></span>         | <span data-ttu-id="0906f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="0906f-108">Return Type</span></span> | <span data-ttu-id="0906f-109">说明</span><span class="sxs-lookup"><span data-stu-id="0906f-109">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="0906f-110">创建 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="0906f-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="0906f-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="0906f-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="0906f-112">创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="0906f-112">Create an online meeting.</span></span> |
| [<span data-ttu-id="0906f-113">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="0906f-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="0906f-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="0906f-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="0906f-115">读取**onlineMeeting**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0906f-115">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="0906f-116">创建或获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="0906f-116">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="0906f-117">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="0906f-117">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="0906f-118">使用自定义外部 ID 创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="0906f-118">Create an online meeting with a custom, external ID.</span></span> <span data-ttu-id="0906f-119">如果会议已存在，请检索其 propertie。</span><span class="sxs-lookup"><span data-stu-id="0906f-119">If the meeting already exists, retrieve its propertie.</span></span> |

## <a name="properties"></a><span data-ttu-id="0906f-120">属性</span><span class="sxs-lookup"><span data-stu-id="0906f-120">Properties</span></span>

| <span data-ttu-id="0906f-121">属性</span><span class="sxs-lookup"><span data-stu-id="0906f-121">Property</span></span>                  | <span data-ttu-id="0906f-122">类型</span><span class="sxs-lookup"><span data-stu-id="0906f-122">Type</span></span>                                                   | <span data-ttu-id="0906f-123">说明</span><span class="sxs-lookup"><span data-stu-id="0906f-123">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="0906f-124">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="0906f-124">autoAdmittedUsers</span></span>         | <span data-ttu-id="0906f-125">String</span><span class="sxs-lookup"><span data-stu-id="0906f-125">String</span></span>                                                 | <span data-ttu-id="0906f-126">指定将自动允许加入联机会议的参与者类型的设置。</span><span class="sxs-lookup"><span data-stu-id="0906f-126">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="0906f-127">可取值为：`everyone`、`everyoneInSameAndFederatedCompany`、`everyoneInCompany`、`invitedUsersInCompany`、`organizer`。</span><span class="sxs-lookup"><span data-stu-id="0906f-127">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span></span> <span data-ttu-id="0906f-128">只读。</span><span class="sxs-lookup"><span data-stu-id="0906f-128">Read-only.</span></span>|
| <span data-ttu-id="0906f-129">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="0906f-129">audioConferencing</span></span>         | [<span data-ttu-id="0906f-130">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="0906f-130">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="0906f-131">联机会议的电话访问（拨入）信息。</span><span class="sxs-lookup"><span data-stu-id="0906f-131">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="0906f-132">只读。</span><span class="sxs-lookup"><span data-stu-id="0906f-132">Read-only.</span></span> |
| <span data-ttu-id="0906f-133">chatInfo</span><span class="sxs-lookup"><span data-stu-id="0906f-133">chatInfo</span></span>                  | [<span data-ttu-id="0906f-134">chatInfo</span><span class="sxs-lookup"><span data-stu-id="0906f-134">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="0906f-135">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="0906f-135">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="0906f-136">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="0906f-136">creationDateTime</span></span>          | <span data-ttu-id="0906f-137">日期时间</span><span class="sxs-lookup"><span data-stu-id="0906f-137">DateTime</span></span>                                               | <span data-ttu-id="0906f-138">以 UTC 表示的会议创建时间。</span><span class="sxs-lookup"><span data-stu-id="0906f-138">The meeting creation time in UTC.</span></span> <span data-ttu-id="0906f-139">只读。</span><span class="sxs-lookup"><span data-stu-id="0906f-139">Read-only.</span></span> |
| <span data-ttu-id="0906f-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0906f-140">startDateTime</span></span>             | <span data-ttu-id="0906f-141">日期时间</span><span class="sxs-lookup"><span data-stu-id="0906f-141">DateTime</span></span>                                               | <span data-ttu-id="0906f-142">以 UTC 表示的会议开始时间。</span><span class="sxs-lookup"><span data-stu-id="0906f-142">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="0906f-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0906f-143">endDateTime</span></span>               | <span data-ttu-id="0906f-144">日期时间</span><span class="sxs-lookup"><span data-stu-id="0906f-144">DateTime</span></span>                                               | <span data-ttu-id="0906f-145">以 UTC 表示的会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="0906f-145">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="0906f-146">id</span><span class="sxs-lookup"><span data-stu-id="0906f-146">id</span></span>                        | <span data-ttu-id="0906f-147">字符串</span><span class="sxs-lookup"><span data-stu-id="0906f-147">String</span></span>                                                 | <span data-ttu-id="0906f-148">与联机会议关联的默认 ID。</span><span class="sxs-lookup"><span data-stu-id="0906f-148">The default ID associated with the online meeting.</span></span> <span data-ttu-id="0906f-149">只读。</span><span class="sxs-lookup"><span data-stu-id="0906f-149">Read-only.</span></span> |
| <span data-ttu-id="0906f-150">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="0906f-150">joinWebUrl</span></span>                   | <span data-ttu-id="0906f-151">String</span><span class="sxs-lookup"><span data-stu-id="0906f-151">String</span></span>                                                 | <span data-ttu-id="0906f-152">联机会议的加入 URL。</span><span class="sxs-lookup"><span data-stu-id="0906f-152">The join URL of the online meeting.</span></span> <span data-ttu-id="0906f-153">只读。</span><span class="sxs-lookup"><span data-stu-id="0906f-153">Read-only.</span></span>|
| <span data-ttu-id="0906f-154">participants</span><span class="sxs-lookup"><span data-stu-id="0906f-154">participants</span></span>              | [<span data-ttu-id="0906f-155">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="0906f-155">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="0906f-156">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="0906f-156">The participants associated with the online meeting.</span></span>  <span data-ttu-id="0906f-157">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="0906f-157">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="0906f-158">subject</span><span class="sxs-lookup"><span data-stu-id="0906f-158">subject</span></span>                   | <span data-ttu-id="0906f-159">String</span><span class="sxs-lookup"><span data-stu-id="0906f-159">String</span></span>                                                 | <span data-ttu-id="0906f-160">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="0906f-160">The subject of the online meeting.</span></span> |
| <span data-ttu-id="0906f-161">capabilities</span><span class="sxs-lookup"><span data-stu-id="0906f-161">capabilities</span></span>              | <span data-ttu-id="0906f-162">String collection</span><span class="sxs-lookup"><span data-stu-id="0906f-162">String collection</span></span>                                      | <span data-ttu-id="0906f-163">会议功能的列表。</span><span class="sxs-lookup"><span data-stu-id="0906f-163">The list of meeting capabilities.</span></span> <span data-ttu-id="0906f-164">可能的值是`questionAndAnswer`：。</span><span class="sxs-lookup"><span data-stu-id="0906f-164">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="0906f-165">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="0906f-165">videoTeleconferenceId</span></span>     | <span data-ttu-id="0906f-166">String</span><span class="sxs-lookup"><span data-stu-id="0906f-166">String</span></span>                                                 | <span data-ttu-id="0906f-167">视频电话会议 ID。</span><span class="sxs-lookup"><span data-stu-id="0906f-167">The video teleconferencing ID.</span></span> <span data-ttu-id="0906f-168">只读。</span><span class="sxs-lookup"><span data-stu-id="0906f-168">Read-only.</span></span> |
| <span data-ttu-id="0906f-169">joinInformation</span><span class="sxs-lookup"><span data-stu-id="0906f-169">joinInformation</span></span> | [<span data-ttu-id="0906f-170">itemBody</span><span class="sxs-lookup"><span data-stu-id="0906f-170">itemBody</span></span>](itembody.md) | <span data-ttu-id="0906f-171">在 "Accept-Language" 请求 HTTP 标头中指定的语言和区域设置变量形式的联接信息。</span><span class="sxs-lookup"><span data-stu-id="0906f-171">The join information in the language and locale variant specified in 'Accept-Language' request HTTP header.</span></span> <span data-ttu-id="0906f-172">只读</span><span class="sxs-lookup"><span data-stu-id="0906f-172">Read-only</span></span> |
| <span data-ttu-id="0906f-173">externalId</span><span class="sxs-lookup"><span data-stu-id="0906f-173">externalId</span></span>                | <span data-ttu-id="0906f-174">String</span><span class="sxs-lookup"><span data-stu-id="0906f-174">String</span></span>                                                 | <span data-ttu-id="0906f-175">外部 ID。</span><span class="sxs-lookup"><span data-stu-id="0906f-175">The external ID.</span></span> <span data-ttu-id="0906f-176">自定义 ID。</span><span class="sxs-lookup"><span data-stu-id="0906f-176">A custom ID.</span></span> <span data-ttu-id="0906f-177">可选。</span><span class="sxs-lookup"><span data-stu-id="0906f-177">Optional.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="0906f-178">autoAdmittedUsers 值</span><span class="sxs-lookup"><span data-stu-id="0906f-178">autoAdmittedUsers values</span></span>
| <span data-ttu-id="0906f-179">值</span><span class="sxs-lookup"><span data-stu-id="0906f-179">Value</span></span> | <span data-ttu-id="0906f-180">说明</span><span class="sxs-lookup"><span data-stu-id="0906f-180">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- |
| <span data-ttu-id="0906f-181">组织者</span><span class="sxs-lookup"><span data-stu-id="0906f-181">organizer</span></span> | <span data-ttu-id="0906f-182">仅会议组织者被直接承认。</span><span class="sxs-lookup"><span data-stu-id="0906f-182">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="0906f-183">其他人将在大厅中等待，直到组织者承认</span><span class="sxs-lookup"><span data-stu-id="0906f-183">Everyone else waits in the lobby, until admitted by the organizer</span></span>  |
| <span data-ttu-id="0906f-184">invitedUsersInCompany</span><span class="sxs-lookup"><span data-stu-id="0906f-184">invitedUsersInCompany</span></span> | <span data-ttu-id="0906f-185">会议组织者和组织者邀请的同一家公司中的用户直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="0906f-185">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="0906f-186">其他人在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="0906f-186">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="0906f-187">everyoneInCompany</span><span class="sxs-lookup"><span data-stu-id="0906f-187">everyoneInCompany</span></span> | <span data-ttu-id="0906f-188">与组织者在同一公司中的所有人都直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="0906f-188">Everyone in the same company as the organizer join the meeting directly.</span></span>  <span data-ttu-id="0906f-189">联合匿名用户在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="0906f-189">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="0906f-190">everyoneInSameAndFederatedCompany</span><span class="sxs-lookup"><span data-stu-id="0906f-190">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="0906f-191">与组织者和联合公司在同一公司中的所有人都直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="0906f-191">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="0906f-192">匿名用户在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="0906f-192">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="0906f-193">成员</span><span class="sxs-lookup"><span data-stu-id="0906f-193">everyone</span></span> | <span data-ttu-id="0906f-194">任何用户都是允许的，这意味着每个人（包括匿名用户）都可以直接加入会议，而无需在会议厅中等待。</span><span class="sxs-lookup"><span data-stu-id="0906f-194">Any user is allowed, which means that everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="0906f-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0906f-195">JSON representation</span></span>

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
