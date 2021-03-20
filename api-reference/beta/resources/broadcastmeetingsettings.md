---
title: broadcastMeetingSettings 资源类型
description: 与实时事件相关的设置
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: def9276d97ddbe1fd812083cc17e547ae7ce53c5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953754"
---
# <a name="broadcastmeetingsettings-resource-type"></a><span data-ttu-id="e262c-103">broadcastMeetingSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="e262c-103">broadcastMeetingSettings resource type</span></span>

<span data-ttu-id="e262c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e262c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e262c-105">与实时事件相关的设置。</span><span class="sxs-lookup"><span data-stu-id="e262c-105">Settings related to a live event.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e262c-106">此 API 不验证由策略 管理的活动 [事件设置](/microsoftteams/teams-live-events/set-teams-live-events-policies-using-powershell)。</span><span class="sxs-lookup"><span data-stu-id="e262c-106">This API does not validate live event settings that are managed by [policy](/microsoftteams/teams-live-events/set-teams-live-events-policies-using-powershell).</span></span>
> <span data-ttu-id="e262c-107">例如，如果管理员使用 设置实时事件策略，将阻止用户设置 Teams 客户端中的实时事件权限，但可通过 Microsoft Graph 将 `Set-CsTeamsMeetingBroadcastPolicy -Identity Global -BroadcastAttendeeVisibility EveryoneInCompany` `public` **allowedAudience** 设置为 来创建实时事件 `everyone` 。</span><span class="sxs-lookup"><span data-stu-id="e262c-107">For example, if an admin sets a live event policy using `Set-CsTeamsMeetingBroadcastPolicy -Identity Global -BroadcastAttendeeVisibility EveryoneInCompany`, users will be prevented from setting live event permissions to `public` in their Teams client, but will be able to create a live event via Microsoft Graph by setting **allowedAudience** to `everyone`.</span></span> 

## <a name="properties"></a><span data-ttu-id="e262c-108">属性</span><span class="sxs-lookup"><span data-stu-id="e262c-108">Properties</span></span>

| <span data-ttu-id="e262c-109">属性</span><span class="sxs-lookup"><span data-stu-id="e262c-109">Property</span></span>                   | <span data-ttu-id="e262c-110">类型</span><span class="sxs-lookup"><span data-stu-id="e262c-110">Type</span></span>                     | <span data-ttu-id="e262c-111">说明</span><span class="sxs-lookup"><span data-stu-id="e262c-111">Description</span></span>                                                                     |
| -------------------------- | ------------------------ | ------------------------------------------------------------------------------- |
| <span data-ttu-id="e262c-112">allowedAudience</span><span class="sxs-lookup"><span data-stu-id="e262c-112">allowedAudience</span></span>            | [<span data-ttu-id="e262c-113">broadcastMeetingAudience</span><span class="sxs-lookup"><span data-stu-id="e262c-113">broadcastMeetingAudience</span></span>](#broadcastmeetingaudience-values) | <span data-ttu-id="e262c-114">定义可加入实时事件的人。</span><span class="sxs-lookup"><span data-stu-id="e262c-114">Defines who can join the live event.</span></span> <span data-ttu-id="e262c-115">下表列出了可能的值。</span><span class="sxs-lookup"><span data-stu-id="e262c-115">Possible values are listed in the following table.</span></span> |
| <span data-ttu-id="e262c-116">isRecordingEnabled</span><span class="sxs-lookup"><span data-stu-id="e262c-116">isRecordingEnabled</span></span>         | <span data-ttu-id="e262c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="e262c-117">Boolean</span></span>                  | <span data-ttu-id="e262c-118">指示是否为此实时事件启用录制。</span><span class="sxs-lookup"><span data-stu-id="e262c-118">Indicates whether recording is enabled for this live event.</span></span> <span data-ttu-id="e262c-119">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="e262c-119">Default value is `false`.</span></span>          |
| <span data-ttu-id="e262c-120">isAttendeeReportEnabled</span><span class="sxs-lookup"><span data-stu-id="e262c-120">isAttendeeReportEnabled</span></span>    | <span data-ttu-id="e262c-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="e262c-121">Boolean</span></span>                  | <span data-ttu-id="e262c-122">指示是否为此实时事件启用与会者报告。</span><span class="sxs-lookup"><span data-stu-id="e262c-122">Indicates whether attendee report is enabled for this live event.</span></span> <span data-ttu-id="e262c-123">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="e262c-123">Default value is `false`.</span></span>    |
| <span data-ttu-id="e262c-124">isQuestionAndAnswerEnabled</span><span class="sxs-lookup"><span data-stu-id="e262c-124">isQuestionAndAnswerEnabled</span></span> | <span data-ttu-id="e262c-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="e262c-125">Boolean</span></span>                  | <span data-ttu-id="e262c-126">指示是否为此&事件启用了问答。</span><span class="sxs-lookup"><span data-stu-id="e262c-126">Indicates whether Q&A is enabled for this live event.</span></span> <span data-ttu-id="e262c-127">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="e262c-127">Default value is `false`.</span></span>                |
| <span data-ttu-id="e262c-128">isVideoOnDemandEnabled</span><span class="sxs-lookup"><span data-stu-id="e262c-128">isVideoOnDemandEnabled</span></span>     | <span data-ttu-id="e262c-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="e262c-129">Boolean</span></span>                  | <span data-ttu-id="e262c-130">指示是否为此实时事件启用视频按需。</span><span class="sxs-lookup"><span data-stu-id="e262c-130">Indicates whether video on demand is enabled for this live event.</span></span> <span data-ttu-id="e262c-131">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="e262c-131">Default value is `false`.</span></span>    |

### <a name="broadcastmeetingaudience-values"></a><span data-ttu-id="e262c-132">broadcastMeetingAudience 值</span><span class="sxs-lookup"><span data-stu-id="e262c-132">broadcastMeetingAudience values</span></span>

| <span data-ttu-id="e262c-133">值</span><span class="sxs-lookup"><span data-stu-id="e262c-133">Value</span></span>              | <span data-ttu-id="e262c-134">说明</span><span class="sxs-lookup"><span data-stu-id="e262c-134">Description</span></span>                                                       |
| ------------------ | ----------------------------------------------------------------- |
| <span data-ttu-id="e262c-135">everyone</span><span class="sxs-lookup"><span data-stu-id="e262c-135">everyone</span></span>           | <span data-ttu-id="e262c-136">实时事件将向任何人开放。</span><span class="sxs-lookup"><span data-stu-id="e262c-136">The live event will be open to anyone.</span></span> <span data-ttu-id="e262c-137">此值为默认值。</span><span class="sxs-lookup"><span data-stu-id="e262c-137">This is the default value.</span></span> |
| <span data-ttu-id="e262c-138">组织</span><span class="sxs-lookup"><span data-stu-id="e262c-138">organization</span></span>       | <span data-ttu-id="e262c-139">组织中的每个人都可以加入实时事件。</span><span class="sxs-lookup"><span data-stu-id="e262c-139">Everyone in your org can join the live event.</span></span>                     |
| <span data-ttu-id="e262c-140">roleIsAttendee</span><span class="sxs-lookup"><span data-stu-id="e262c-140">roleIsAttendee</span></span>     | <span data-ttu-id="e262c-141">只有指定的人员才能加入实时事件。</span><span class="sxs-lookup"><span data-stu-id="e262c-141">Only the specified people can join the live event.</span></span>                |
| <span data-ttu-id="e262c-142">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="e262c-142">unknownFutureValue</span></span> | <span data-ttu-id="e262c-143">未知未来值。</span><span class="sxs-lookup"><span data-stu-id="e262c-143">Unknown future value.</span></span>                                             |

## <a name="json-representation"></a><span data-ttu-id="e262c-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e262c-144">JSON representation</span></span>

<span data-ttu-id="e262c-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e262c-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.broadcastMeetingSettings"
}-->
```json
{
  "allowedAudience": "String",
  "isRecordingEnabled": "Boolean",
  "isAttendeeReportEnabled": "Boolean",
  "isQuestionAndAnswerEnabled": "Boolean",
  "isVideoOnDemandEnabled": "Boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "broadcastSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
