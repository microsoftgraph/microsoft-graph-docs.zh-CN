---
title: broadcastMeetingSettings 资源类型
description: 设置实时事件相关的事件
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1de814ee520d1dbf8d0ea6ba1270c6893a07d2cd
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896688"
---
# <a name="broadcastmeetingsettings-resource-type"></a><span data-ttu-id="dec63-103">broadcastMeetingSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="dec63-103">broadcastMeetingSettings resource type</span></span>

<span data-ttu-id="dec63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dec63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dec63-105">设置实时事件相关。</span><span class="sxs-lookup"><span data-stu-id="dec63-105">Settings related to a live event.</span></span>

> [!CAUTION]
> <span data-ttu-id="dec63-106">此 API 不验证由策略 管理的活动 [事件设置](/microsoftteams/teams-live-events/set-teams-live-events-policies-using-powershell)。</span><span class="sxs-lookup"><span data-stu-id="dec63-106">This API does not validate live event settings that are managed by [policy](/microsoftteams/teams-live-events/set-teams-live-events-policies-using-powershell).</span></span>
> <span data-ttu-id="dec63-107">例如，如果管理员使用 设置实时事件策略，用户将被阻止在 Teams 客户端中设置实时事件权限，但能够通过 `Set-CsTeamsMeetingBroadcastPolicy -Identity Global -BroadcastAttendeeVisibility EveryoneInCompany` `public` 将 **allowedAudience** 设置为 ，通过 Microsoft Graph 创建实时事件 `everyone` 。</span><span class="sxs-lookup"><span data-stu-id="dec63-107">For example, if an admin sets a live event policy using `Set-CsTeamsMeetingBroadcastPolicy -Identity Global -BroadcastAttendeeVisibility EveryoneInCompany`, users will be prevented from setting live event permissions to `public` in their Teams client, but will be able to create a live event via Microsoft Graph by setting **allowedAudience** to `everyone`.</span></span>

## <a name="properties"></a><span data-ttu-id="dec63-108">属性</span><span class="sxs-lookup"><span data-stu-id="dec63-108">Properties</span></span>

| <span data-ttu-id="dec63-109">属性</span><span class="sxs-lookup"><span data-stu-id="dec63-109">Property</span></span>                   | <span data-ttu-id="dec63-110">类型</span><span class="sxs-lookup"><span data-stu-id="dec63-110">Type</span></span>                     | <span data-ttu-id="dec63-111">说明</span><span class="sxs-lookup"><span data-stu-id="dec63-111">Description</span></span>                                                                     |
| -------------------------- | ------------------------ | ------------------------------------------------------------------------------- |
| <span data-ttu-id="dec63-112">allowedAudience</span><span class="sxs-lookup"><span data-stu-id="dec63-112">allowedAudience</span></span>            | [<span data-ttu-id="dec63-113">broadcastMeetingAudience</span><span class="sxs-lookup"><span data-stu-id="dec63-113">broadcastMeetingAudience</span></span>](#broadcastmeetingaudience-values) | <span data-ttu-id="dec63-114">定义可加入实时事件的人。</span><span class="sxs-lookup"><span data-stu-id="dec63-114">Defines who can join the live event.</span></span> <span data-ttu-id="dec63-115">下表列出了可能的值。</span><span class="sxs-lookup"><span data-stu-id="dec63-115">Possible values are listed in the following table.</span></span> |
| <span data-ttu-id="dec63-116">isRecordingEnabled</span><span class="sxs-lookup"><span data-stu-id="dec63-116">isRecordingEnabled</span></span>         | <span data-ttu-id="dec63-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="dec63-117">Boolean</span></span>                  | <span data-ttu-id="dec63-118">指示是否为此实时事件启用录制。</span><span class="sxs-lookup"><span data-stu-id="dec63-118">Indicates whether recording is enabled for this live event.</span></span> <span data-ttu-id="dec63-119">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="dec63-119">Default value is `false`.</span></span>          |
| <span data-ttu-id="dec63-120">isAttendeeReportEnabled</span><span class="sxs-lookup"><span data-stu-id="dec63-120">isAttendeeReportEnabled</span></span>    | <span data-ttu-id="dec63-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="dec63-121">Boolean</span></span>                  | <span data-ttu-id="dec63-122">指示是否为此实时事件启用与会者报告。</span><span class="sxs-lookup"><span data-stu-id="dec63-122">Indicates whether attendee report is enabled for this live event.</span></span> <span data-ttu-id="dec63-123">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="dec63-123">Default value is `false`.</span></span>    |
| <span data-ttu-id="dec63-124">isQuestionAndAnswerEnabled</span><span class="sxs-lookup"><span data-stu-id="dec63-124">isQuestionAndAnswerEnabled</span></span> | <span data-ttu-id="dec63-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="dec63-125">Boolean</span></span>                  | <span data-ttu-id="dec63-126">指示是否为此&事件启用了问答。</span><span class="sxs-lookup"><span data-stu-id="dec63-126">Indicates whether Q&A is enabled for this live event.</span></span> <span data-ttu-id="dec63-127">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="dec63-127">Default value is `false`.</span></span>                |
| <span data-ttu-id="dec63-128">isVideoOnDemandEnabled</span><span class="sxs-lookup"><span data-stu-id="dec63-128">isVideoOnDemandEnabled</span></span>     | <span data-ttu-id="dec63-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="dec63-129">Boolean</span></span>                  | <span data-ttu-id="dec63-130">指示是否为此实时事件启用视频按需。</span><span class="sxs-lookup"><span data-stu-id="dec63-130">Indicates whether video on demand is enabled for this live event.</span></span> <span data-ttu-id="dec63-131">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="dec63-131">Default value is `false`.</span></span>    |

### <a name="broadcastmeetingaudience-values"></a><span data-ttu-id="dec63-132">broadcastMeetingAudience 值</span><span class="sxs-lookup"><span data-stu-id="dec63-132">broadcastMeetingAudience values</span></span>

| <span data-ttu-id="dec63-133">值</span><span class="sxs-lookup"><span data-stu-id="dec63-133">Value</span></span>              | <span data-ttu-id="dec63-134">说明</span><span class="sxs-lookup"><span data-stu-id="dec63-134">Description</span></span>                                                       |
| ------------------ | ----------------------------------------------------------------- |
| <span data-ttu-id="dec63-135">everyone</span><span class="sxs-lookup"><span data-stu-id="dec63-135">everyone</span></span>           | <span data-ttu-id="dec63-136">实时事件将向任何人开放。</span><span class="sxs-lookup"><span data-stu-id="dec63-136">The live event will be open to anyone.</span></span> <span data-ttu-id="dec63-137">此值为默认值。</span><span class="sxs-lookup"><span data-stu-id="dec63-137">This is the default value.</span></span> |
| <span data-ttu-id="dec63-138">组织</span><span class="sxs-lookup"><span data-stu-id="dec63-138">organization</span></span>       | <span data-ttu-id="dec63-139">组织中的每个人都可以加入实时事件。</span><span class="sxs-lookup"><span data-stu-id="dec63-139">Everyone in your org can join the live event.</span></span>                     |
| <span data-ttu-id="dec63-140">roleIsAttendee</span><span class="sxs-lookup"><span data-stu-id="dec63-140">roleIsAttendee</span></span>     | <span data-ttu-id="dec63-141">只有指定的人员才能加入实时事件。</span><span class="sxs-lookup"><span data-stu-id="dec63-141">Only the specified people can join the live event.</span></span>                |
| <span data-ttu-id="dec63-142">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="dec63-142">unknownFutureValue</span></span> | <span data-ttu-id="dec63-143">未知未来值。</span><span class="sxs-lookup"><span data-stu-id="dec63-143">Unknown future value.</span></span>                                             |

## <a name="json-representation"></a><span data-ttu-id="dec63-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dec63-144">JSON representation</span></span>

<span data-ttu-id="dec63-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dec63-145">The following is a JSON representation of the resource.</span></span>

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
