---
title: onlineMeeting 资源类型
description: 包含有关会议的信息，包括联接 URL、与会者列表和说明。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: bfc1055b3e700b951957ffd1bce0fe7a541846b0
ms.sourcegitcommit: 93b6781adf2c889235022d34ab50e2a4d62760c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/07/2020
ms.locfileid: "46589254"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="4f664-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f664-103">onlineMeeting resource type</span></span>

<span data-ttu-id="4f664-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f664-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f664-105">包含有关会议的信息，包括用于加入会议的 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="4f664-105">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="4f664-106">方法</span><span class="sxs-lookup"><span data-stu-id="4f664-106">Methods</span></span>

| <span data-ttu-id="4f664-107">方法</span><span class="sxs-lookup"><span data-stu-id="4f664-107">Method</span></span>         | <span data-ttu-id="4f664-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4f664-108">Return Type</span></span> | <span data-ttu-id="4f664-109">说明</span><span class="sxs-lookup"><span data-stu-id="4f664-109">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="4f664-110">创建</span><span class="sxs-lookup"><span data-stu-id="4f664-110">Create</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="4f664-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="4f664-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="4f664-112">创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="4f664-112">Create an online meeting.</span></span> |
| [<span data-ttu-id="4f664-113">获取</span><span class="sxs-lookup"><span data-stu-id="4f664-113">Get</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="4f664-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="4f664-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="4f664-115">读取**onlineMeeting**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4f664-115">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="4f664-116">创建或获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="4f664-116">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="4f664-117">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="4f664-117">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="4f664-118">使用自定义外部 ID 创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="4f664-118">Create an online meeting with a custom, external ID.</span></span> <span data-ttu-id="4f664-119">如果会议已存在，请检索其属性。</span><span class="sxs-lookup"><span data-stu-id="4f664-119">If the meeting already exists, retrieve its properties.</span></span> |
| [<span data-ttu-id="4f664-120">更新</span><span class="sxs-lookup"><span data-stu-id="4f664-120">Update</span></span>](../api/onlinemeeting-update.md) | [<span data-ttu-id="4f664-121">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="4f664-121">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="4f664-122">更新联机会议的 " **startDateTime**"、" **endDateTime**"、"**主题**" 和 "**参与者**" 属性。</span><span class="sxs-lookup"><span data-stu-id="4f664-122">Update the **startDateTime**, **endDateTime**, **subject**, and **participants** properties of an online meeting.</span></span> |
| [<span data-ttu-id="4f664-123">删除</span><span class="sxs-lookup"><span data-stu-id="4f664-123">Delete</span></span>](../api/onlinemeeting-delete.md) | <span data-ttu-id="4f664-124">无</span><span class="sxs-lookup"><span data-stu-id="4f664-124">None</span></span> | <span data-ttu-id="4f664-125">删除**onlineMeeting**资源。</span><span class="sxs-lookup"><span data-stu-id="4f664-125">Delete an **onlineMeeting** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="4f664-126">属性</span><span class="sxs-lookup"><span data-stu-id="4f664-126">Properties</span></span>

| <span data-ttu-id="4f664-127">属性</span><span class="sxs-lookup"><span data-stu-id="4f664-127">Property</span></span>                  | <span data-ttu-id="4f664-128">类型</span><span class="sxs-lookup"><span data-stu-id="4f664-128">Type</span></span>                                                   | <span data-ttu-id="4f664-129">说明</span><span class="sxs-lookup"><span data-stu-id="4f664-129">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="4f664-130">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="4f664-130">autoAdmittedUsers</span></span>         | <span data-ttu-id="4f664-131">String</span><span class="sxs-lookup"><span data-stu-id="4f664-131">String</span></span>                                                 | <span data-ttu-id="4f664-132">指定将自动允许加入联机会议的参与者类型的设置。</span><span class="sxs-lookup"><span data-stu-id="4f664-132">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="4f664-133">可取值为：`everyone`、`everyoneInSameAndFederatedCompany`、`everyoneInCompany`、`invitedUsersInCompany`、`organizer`。</span><span class="sxs-lookup"><span data-stu-id="4f664-133">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span></span> <span data-ttu-id="4f664-134">只读。</span><span class="sxs-lookup"><span data-stu-id="4f664-134">Read-only.</span></span>|
| <span data-ttu-id="4f664-135">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="4f664-135">audioConferencing</span></span>         | [<span data-ttu-id="4f664-136">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="4f664-136">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="4f664-137">电话访问 (电话拨入) 联机会议的信息。</span><span class="sxs-lookup"><span data-stu-id="4f664-137">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="4f664-138">只读。</span><span class="sxs-lookup"><span data-stu-id="4f664-138">Read-only.</span></span> |
| <span data-ttu-id="4f664-139">chatInfo</span><span class="sxs-lookup"><span data-stu-id="4f664-139">chatInfo</span></span>                  | [<span data-ttu-id="4f664-140">chatInfo</span><span class="sxs-lookup"><span data-stu-id="4f664-140">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="4f664-141">与此联机会议关联的聊天信息。</span><span class="sxs-lookup"><span data-stu-id="4f664-141">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="4f664-142">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="4f664-142">creationDateTime</span></span>          | <span data-ttu-id="4f664-143">DateTime</span><span class="sxs-lookup"><span data-stu-id="4f664-143">DateTime</span></span>                                               | <span data-ttu-id="4f664-144">以 UTC 表示的会议创建时间。</span><span class="sxs-lookup"><span data-stu-id="4f664-144">The meeting creation time in UTC.</span></span> <span data-ttu-id="4f664-145">只读。</span><span class="sxs-lookup"><span data-stu-id="4f664-145">Read-only.</span></span> |
| <span data-ttu-id="4f664-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4f664-146">startDateTime</span></span>             | <span data-ttu-id="4f664-147">DateTime</span><span class="sxs-lookup"><span data-stu-id="4f664-147">DateTime</span></span>                                               | <span data-ttu-id="4f664-148">以 UTC 表示的会议开始时间。</span><span class="sxs-lookup"><span data-stu-id="4f664-148">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="4f664-149">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4f664-149">endDateTime</span></span>               | <span data-ttu-id="4f664-150">DateTime</span><span class="sxs-lookup"><span data-stu-id="4f664-150">DateTime</span></span>                                               | <span data-ttu-id="4f664-151">以 UTC 表示的会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="4f664-151">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="4f664-152">id</span><span class="sxs-lookup"><span data-stu-id="4f664-152">id</span></span>                        | <span data-ttu-id="4f664-153">String</span><span class="sxs-lookup"><span data-stu-id="4f664-153">String</span></span>                                                 | <span data-ttu-id="4f664-154">与联机会议关联的默认 ID。</span><span class="sxs-lookup"><span data-stu-id="4f664-154">The default ID associated with the online meeting.</span></span> <span data-ttu-id="4f664-155">只读。</span><span class="sxs-lookup"><span data-stu-id="4f664-155">Read-only.</span></span> |
| <span data-ttu-id="4f664-156">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="4f664-156">joinWebUrl</span></span>                   | <span data-ttu-id="4f664-157">String</span><span class="sxs-lookup"><span data-stu-id="4f664-157">String</span></span>                                                 | <span data-ttu-id="4f664-158">联机会议的加入 URL。</span><span class="sxs-lookup"><span data-stu-id="4f664-158">The join URL of the online meeting.</span></span> <span data-ttu-id="4f664-159">只读。</span><span class="sxs-lookup"><span data-stu-id="4f664-159">Read-only.</span></span>|
| <span data-ttu-id="4f664-160">participants</span><span class="sxs-lookup"><span data-stu-id="4f664-160">participants</span></span>              | [<span data-ttu-id="4f664-161">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="4f664-161">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="4f664-162">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="4f664-162">The participants associated with the online meeting.</span></span>  <span data-ttu-id="4f664-163">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="4f664-163">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="4f664-164">subject</span><span class="sxs-lookup"><span data-stu-id="4f664-164">subject</span></span>                   | <span data-ttu-id="4f664-165">String</span><span class="sxs-lookup"><span data-stu-id="4f664-165">String</span></span>                                                 | <span data-ttu-id="4f664-166">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="4f664-166">The subject of the online meeting.</span></span> |
| <span data-ttu-id="4f664-167">capabilities</span><span class="sxs-lookup"><span data-stu-id="4f664-167">capabilities</span></span>              | <span data-ttu-id="4f664-168">String collection</span><span class="sxs-lookup"><span data-stu-id="4f664-168">String collection</span></span>                                      | <span data-ttu-id="4f664-169">会议功能的列表。</span><span class="sxs-lookup"><span data-stu-id="4f664-169">The list of meeting capabilities.</span></span> <span data-ttu-id="4f664-170">可能的值是： `questionAndAnswer` 。</span><span class="sxs-lookup"><span data-stu-id="4f664-170">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="4f664-171">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="4f664-171">videoTeleconferenceId</span></span>     | <span data-ttu-id="4f664-172">String</span><span class="sxs-lookup"><span data-stu-id="4f664-172">String</span></span>                                                 | <span data-ttu-id="4f664-173">视频电话会议 ID。</span><span class="sxs-lookup"><span data-stu-id="4f664-173">The video teleconferencing ID.</span></span> <span data-ttu-id="4f664-174">只读。</span><span class="sxs-lookup"><span data-stu-id="4f664-174">Read-only.</span></span> |
| <span data-ttu-id="4f664-175">joinInformation</span><span class="sxs-lookup"><span data-stu-id="4f664-175">joinInformation</span></span> | [<span data-ttu-id="4f664-176">itemBody</span><span class="sxs-lookup"><span data-stu-id="4f664-176">itemBody</span></span>](itembody.md) | <span data-ttu-id="4f664-177">在 "Accept-Language" 请求 HTTP 标头中指定的语言和区域设置变量形式的联接信息。</span><span class="sxs-lookup"><span data-stu-id="4f664-177">The join information in the language and locale variant specified in 'Accept-Language' request HTTP header.</span></span> <span data-ttu-id="4f664-178">只读</span><span class="sxs-lookup"><span data-stu-id="4f664-178">Read-only</span></span> |
| <span data-ttu-id="4f664-179">externalId</span><span class="sxs-lookup"><span data-stu-id="4f664-179">externalId</span></span>                | <span data-ttu-id="4f664-180">String</span><span class="sxs-lookup"><span data-stu-id="4f664-180">String</span></span>                                                 | <span data-ttu-id="4f664-181">外部 ID。</span><span class="sxs-lookup"><span data-stu-id="4f664-181">The external ID.</span></span> <span data-ttu-id="4f664-182">自定义 ID。</span><span class="sxs-lookup"><span data-stu-id="4f664-182">A custom ID.</span></span> <span data-ttu-id="4f664-183">可选。</span><span class="sxs-lookup"><span data-stu-id="4f664-183">Optional.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="4f664-184">autoAdmittedUsers 值</span><span class="sxs-lookup"><span data-stu-id="4f664-184">autoAdmittedUsers values</span></span>
| <span data-ttu-id="4f664-185">值</span><span class="sxs-lookup"><span data-stu-id="4f664-185">Value</span></span> | <span data-ttu-id="4f664-186">说明</span><span class="sxs-lookup"><span data-stu-id="4f664-186">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- |
| <span data-ttu-id="4f664-187">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="4f664-187">organizer</span></span> | <span data-ttu-id="4f664-188">仅会议组织者被直接承认。</span><span class="sxs-lookup"><span data-stu-id="4f664-188">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="4f664-189">其他人将在大厅中等待，直到组织者承认</span><span class="sxs-lookup"><span data-stu-id="4f664-189">Everyone else waits in the lobby, until admitted by the organizer</span></span>  |
| <span data-ttu-id="4f664-190">invitedUsersInCompany</span><span class="sxs-lookup"><span data-stu-id="4f664-190">invitedUsersInCompany</span></span> | <span data-ttu-id="4f664-191">会议组织者和组织者邀请的同一家公司中的用户直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="4f664-191">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="4f664-192">其他人在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="4f664-192">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="4f664-193">everyoneInCompany</span><span class="sxs-lookup"><span data-stu-id="4f664-193">everyoneInCompany</span></span> | <span data-ttu-id="4f664-194">与组织者在同一公司中的所有人都直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="4f664-194">Everyone in the same company as the organizer join the meeting directly.</span></span>  <span data-ttu-id="4f664-195">联合匿名用户在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="4f664-195">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="4f664-196">everyoneInSameAndFederatedCompany</span><span class="sxs-lookup"><span data-stu-id="4f664-196">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="4f664-197">与组织者和联合公司在同一公司中的所有人都直接加入会议。</span><span class="sxs-lookup"><span data-stu-id="4f664-197">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="4f664-198">匿名用户在大厅等待，直到被许可。</span><span class="sxs-lookup"><span data-stu-id="4f664-198">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="4f664-199">成员</span><span class="sxs-lookup"><span data-stu-id="4f664-199">everyone</span></span> | <span data-ttu-id="4f664-200">允许任何用户，这意味着每个人 (包括匿名用户) 可以直接加入会议，而无需在会议厅中等待。</span><span class="sxs-lookup"><span data-stu-id="4f664-200">Any user is allowed, which means that everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="4f664-201">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f664-201">JSON representation</span></span>

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
