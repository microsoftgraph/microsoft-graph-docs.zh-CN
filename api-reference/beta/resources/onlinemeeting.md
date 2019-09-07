---
title: onlineMeeting 资源类型
description: 捕获有关会议的信息，包括联接 URL、与会者列表和说明。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 611731673d932d6c5135c0115d735e4d642b1bfe
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792784"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="7a943-103">onlineMeeting 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a943-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a943-104">捕获有关会议的信息，包括联接 URL、与会者列表和说明。</span><span class="sxs-lookup"><span data-stu-id="7a943-104">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="7a943-105">方法</span><span class="sxs-lookup"><span data-stu-id="7a943-105">Methods</span></span>

| <span data-ttu-id="7a943-106">方法</span><span class="sxs-lookup"><span data-stu-id="7a943-106">Method</span></span>         | <span data-ttu-id="7a943-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="7a943-107">Return Type</span></span> | <span data-ttu-id="7a943-108">说明</span><span class="sxs-lookup"><span data-stu-id="7a943-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="7a943-109">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="7a943-109">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="7a943-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="7a943-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="7a943-111">读取 onlineMeeting 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7a943-111">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7a943-112">属性</span><span class="sxs-lookup"><span data-stu-id="7a943-112">Properties</span></span>

| <span data-ttu-id="7a943-113">属性</span><span class="sxs-lookup"><span data-stu-id="7a943-113">Property</span></span>                  | <span data-ttu-id="7a943-114">类型</span><span class="sxs-lookup"><span data-stu-id="7a943-114">Type</span></span>                                                   | <span data-ttu-id="7a943-115">说明</span><span class="sxs-lookup"><span data-stu-id="7a943-115">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7a943-116">accessLevel</span><span class="sxs-lookup"><span data-stu-id="7a943-116">accessLevel</span></span>               | <span data-ttu-id="7a943-117">String</span><span class="sxs-lookup"><span data-stu-id="7a943-117">String</span></span>                                                 | <span data-ttu-id="7a943-118">控制联机会议的许可的访问级别。</span><span class="sxs-lookup"><span data-stu-id="7a943-118">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="7a943-119">可取值为：`everyone`、`invited`、`locked`、`sameEnterprise`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="7a943-119">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="7a943-120">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="7a943-120">audioConferencing</span></span>         | [<span data-ttu-id="7a943-121">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="7a943-121">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="7a943-122">表示 onlineMeeting 的电话访问信息。</span><span class="sxs-lookup"><span data-stu-id="7a943-122">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="7a943-123">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="7a943-123">canceledDateTime</span></span>          | <span data-ttu-id="7a943-124">日期时间</span><span class="sxs-lookup"><span data-stu-id="7a943-124">DateTime</span></span>                                               | <span data-ttu-id="7a943-125">取消会议的时间。</span><span class="sxs-lookup"><span data-stu-id="7a943-125">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="7a943-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="7a943-126">chatInfo</span></span>                  | [<span data-ttu-id="7a943-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="7a943-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="7a943-128">与此会议关联的聊天。</span><span class="sxs-lookup"><span data-stu-id="7a943-128">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="7a943-129">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="7a943-129">creationDateTime</span></span>          | <span data-ttu-id="7a943-130">日期时间</span><span class="sxs-lookup"><span data-stu-id="7a943-130">DateTime</span></span>                                               | <span data-ttu-id="7a943-131">会议的创建时间。</span><span class="sxs-lookup"><span data-stu-id="7a943-131">The time when the meeting was created.</span></span> <span data-ttu-id="7a943-132">只读。</span><span class="sxs-lookup"><span data-stu-id="7a943-132">Read-only.</span></span>
| <span data-ttu-id="7a943-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7a943-133">endDateTime</span></span>               | <span data-ttu-id="7a943-134">日期时间</span><span class="sxs-lookup"><span data-stu-id="7a943-134">DateTime</span></span>                                               | <span data-ttu-id="7a943-135">会议的结束时间。</span><span class="sxs-lookup"><span data-stu-id="7a943-135">End time of the meeting.</span></span> |
| <span data-ttu-id="7a943-136">entryExitAnnouncement</span><span class="sxs-lookup"><span data-stu-id="7a943-136">entryExitAnnouncement</span></span>     | <span data-ttu-id="7a943-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a943-137">Boolean</span></span>                                                | <span data-ttu-id="7a943-138">联机会议的出席通知状态。</span><span class="sxs-lookup"><span data-stu-id="7a943-138">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="7a943-139">启用出席通知后，联机会议将通知通过音频加入会议的参与者的姓名。</span><span class="sxs-lookup"><span data-stu-id="7a943-139">When attendance announcements are enabled, the online meeting will announce the names of the participants who join the meeting through audio.</span></span> |
| <span data-ttu-id="7a943-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7a943-140">expirationDateTime</span></span>        | <span data-ttu-id="7a943-141">日期时间</span><span class="sxs-lookup"><span data-stu-id="7a943-141">DateTime</span></span>                                               | <span data-ttu-id="7a943-142">可在其后删除联机会议的绝对协调通用时间（UTC）日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7a943-142">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="7a943-143">日期和时间必须在服务器上的当前日期和时间之后的一年前一年和之后10年。</span><span class="sxs-lookup"><span data-stu-id="7a943-143">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="7a943-144">id</span><span class="sxs-lookup"><span data-stu-id="7a943-144">id</span></span>                        | <span data-ttu-id="7a943-145">字符串</span><span class="sxs-lookup"><span data-stu-id="7a943-145">String</span></span>                                                 | <span data-ttu-id="7a943-146">与联机会议相关联的 ID。</span><span class="sxs-lookup"><span data-stu-id="7a943-146">The ID associated with the online meeting.</span></span> <span data-ttu-id="7a943-147">在 GET HTTP 请求中用作 ID。</span><span class="sxs-lookup"><span data-stu-id="7a943-147">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="7a943-148">只读。</span><span class="sxs-lookup"><span data-stu-id="7a943-148">Read-only.</span></span> <span data-ttu-id="7a943-149">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="7a943-149">Server generated.</span></span> |
| <span data-ttu-id="7a943-150">isCancelled</span><span class="sxs-lookup"><span data-stu-id="7a943-150">isCancelled</span></span>               | <span data-ttu-id="7a943-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a943-151">Boolean</span></span>                                                | <span data-ttu-id="7a943-152">会议是否已被取消。</span><span class="sxs-lookup"><span data-stu-id="7a943-152">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="7a943-153">joinUrl</span><span class="sxs-lookup"><span data-stu-id="7a943-153">joinUrl</span></span>                   | <span data-ttu-id="7a943-154">String</span><span class="sxs-lookup"><span data-stu-id="7a943-154">String</span></span>                                                 | <span data-ttu-id="7a943-155">从 web 加入联机会议时使用的 URL。</span><span class="sxs-lookup"><span data-stu-id="7a943-155">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="7a943-156">meetingType</span><span class="sxs-lookup"><span data-stu-id="7a943-156">meetingType</span></span>               | <span data-ttu-id="7a943-157">String</span><span class="sxs-lookup"><span data-stu-id="7a943-157">String</span></span>                                                 | <span data-ttu-id="7a943-158">可能的值为`meetNow`： `scheduled`、 `recurring`、 `broadcast` 、（注意： [create onlineMeeting](../api/application-post-onlinemeetings.md)仅`meetNow`支持）。</span><span class="sxs-lookup"><span data-stu-id="7a943-158">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast` (Note: [create onlineMeeting](../api/application-post-onlinemeetings.md) only supports `meetNow`).</span></span> |
| <span data-ttu-id="7a943-159">participants</span><span class="sxs-lookup"><span data-stu-id="7a943-159">participants</span></span>              | [<span data-ttu-id="7a943-160">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="7a943-160">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="7a943-161">与联机会议关联的参与者。</span><span class="sxs-lookup"><span data-stu-id="7a943-161">The participants associated with the online meeting.</span></span>  <span data-ttu-id="7a943-162">这包括组织者和与会者。</span><span class="sxs-lookup"><span data-stu-id="7a943-162">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="7a943-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7a943-163">startDateTime</span></span>             | <span data-ttu-id="7a943-164">日期时间</span><span class="sxs-lookup"><span data-stu-id="7a943-164">DateTime</span></span>                                               | <span data-ttu-id="7a943-165">会议的开始时间。</span><span class="sxs-lookup"><span data-stu-id="7a943-165">Start time of the meeting.</span></span> |
| <span data-ttu-id="7a943-166">subject</span><span class="sxs-lookup"><span data-stu-id="7a943-166">subject</span></span>                   | <span data-ttu-id="7a943-167">String</span><span class="sxs-lookup"><span data-stu-id="7a943-167">String</span></span>                                                 | <span data-ttu-id="7a943-168">联机会议的主题。</span><span class="sxs-lookup"><span data-stu-id="7a943-168">The subject of the online meeting.</span></span> |
| <span data-ttu-id="7a943-169">capabilities</span><span class="sxs-lookup"><span data-stu-id="7a943-169">capabilities</span></span>              | <span data-ttu-id="7a943-170">String collection</span><span class="sxs-lookup"><span data-stu-id="7a943-170">String collection</span></span>                                      | <span data-ttu-id="7a943-171">会议功能的列表。</span><span class="sxs-lookup"><span data-stu-id="7a943-171">The list of meeting capabilities.</span></span> <span data-ttu-id="7a943-172">可能的值是`questionAndAnswer`：。</span><span class="sxs-lookup"><span data-stu-id="7a943-172">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="7a943-173">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="7a943-173">videoTeleconferenceId</span></span>     | <span data-ttu-id="7a943-174">String</span><span class="sxs-lookup"><span data-stu-id="7a943-174">String</span></span>                                                 | <span data-ttu-id="7a943-175">视频电话会议 id。</span><span class="sxs-lookup"><span data-stu-id="7a943-175">The video teleconferencing id.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7a943-176">关系</span><span class="sxs-lookup"><span data-stu-id="7a943-176">Relationships</span></span>
<span data-ttu-id="7a943-177">无</span><span class="sxs-lookup"><span data-stu-id="7a943-177">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a943-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a943-178">JSON representation</span></span>

<span data-ttu-id="7a943-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a943-179">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "accessLevel": "everyone | invited | locked | sameEnterprise",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "entryExitAnnouncement": true,
  "expirationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCancelled": false,
  "joinUrl": "String",
  "meetingType": "meetNow | scheduled | recurring | broadcast",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "capabilities": [ "questionAndAnswer" ],
  "videoTeleconferenceId": "String"
}
```