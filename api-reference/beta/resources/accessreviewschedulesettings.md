---
title: accessReviewScheduleSettings 资源类型
description: 在 Azure AD 访问评审功能中，表示与访问 `accessReviewScheduleSettings` 评审系列关联的设置。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 77ea7d8601df36525aad7a3448aa3b6f031d98d3
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469316"
---
# <a name="accessreviewschedulesettings-resource-type"></a><span data-ttu-id="64578-103">accessReviewScheduleSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="64578-103">accessReviewScheduleSettings resource type</span></span>

<span data-ttu-id="64578-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64578-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="64578-105">**accessReviewScheduleSettings** 定义 [accessReviewScheduleDefinition 的设置](accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="64578-105">The **accessReviewScheduleSettings** defines the settings of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="64578-106">属性</span><span class="sxs-lookup"><span data-stu-id="64578-106">Properties</span></span>
| <span data-ttu-id="64578-107">属性</span><span class="sxs-lookup"><span data-stu-id="64578-107">Property</span></span>    | <span data-ttu-id="64578-108">类型</span><span class="sxs-lookup"><span data-stu-id="64578-108">Type</span></span>   | <span data-ttu-id="64578-109">说明</span><span class="sxs-lookup"><span data-stu-id="64578-109">Description</span></span> |
| :---------------| :---------- | :---------- |
| <span data-ttu-id="64578-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="64578-110">mailNotificationsEnabled</span></span>|<span data-ttu-id="64578-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="64578-111">Boolean</span></span> | <span data-ttu-id="64578-112">指示电子邮件是否已启用/禁用的标志。</span><span class="sxs-lookup"><span data-stu-id="64578-112">Flag to indicate whether emails are enabled/disabled.</span></span>                |
| <span data-ttu-id="64578-113">reminderNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="64578-113">reminderNotificationsEnabled</span></span>|<span data-ttu-id="64578-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="64578-114">Boolean</span></span>  | <span data-ttu-id="64578-115">指示是否启用/禁用提醒的标志。</span><span class="sxs-lookup"><span data-stu-id="64578-115">Flag to indicate whether reminders are enabled/disabled.</span></span>   |
| <span data-ttu-id="64578-116">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="64578-116">justificationRequiredOnApproval</span></span>|<span data-ttu-id="64578-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="64578-117">Boolean</span></span> | <span data-ttu-id="64578-118">用于指示是否需要审阅者提供其决策的理由的标志。</span><span class="sxs-lookup"><span data-stu-id="64578-118">Flag to indicate whether reviewers are required to provide justification with their decision.</span></span> |
| <span data-ttu-id="64578-119">defaultDecisionEnabled</span><span class="sxs-lookup"><span data-stu-id="64578-119">defaultDecisionEnabled</span></span>|<span data-ttu-id="64578-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="64578-120">Boolean</span></span> | <span data-ttu-id="64578-121">指示在审阅者未响应时是否启用/禁用默认决策的标志。</span><span class="sxs-lookup"><span data-stu-id="64578-121">Flag to indicate whether default decision is enabled/disabled when reviewers do not respond.</span></span> |
| <span data-ttu-id="64578-122">defaultDecision</span><span class="sxs-lookup"><span data-stu-id="64578-122">defaultDecision</span></span>|<span data-ttu-id="64578-123">String</span><span class="sxs-lookup"><span data-stu-id="64578-123">String</span></span> | <span data-ttu-id="64578-124">如果已启用， `defaultDecisionEnabled` 则选择决策。</span><span class="sxs-lookup"><span data-stu-id="64578-124">Decision chosen if `defaultDecisionEnabled` is enabled.</span></span> <span data-ttu-id="64578-125">可以是"批准"、"拒绝"或"建议"之一。</span><span class="sxs-lookup"><span data-stu-id="64578-125">Can be one of "Approve", "Deny", or "Recommendation".</span></span> |
| <span data-ttu-id="64578-126">instanceDurationInDays</span><span class="sxs-lookup"><span data-stu-id="64578-126">instanceDurationInDays</span></span>|<span data-ttu-id="64578-127">Int32</span><span class="sxs-lookup"><span data-stu-id="64578-127">Int32</span></span> | <span data-ttu-id="64578-128">每次重复审阅的持续时间 () `accessReviewInstance` 天数表示。</span><span class="sxs-lookup"><span data-stu-id="64578-128">Duration of each recurrence of review (`accessReviewInstance`) in number of days.</span></span> |
| <span data-ttu-id="64578-129">定期</span><span class="sxs-lookup"><span data-stu-id="64578-129">recurrence</span></span>|[<span data-ttu-id="64578-130">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="64578-130">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) | <span data-ttu-id="64578-131">定期的详细设置。</span><span class="sxs-lookup"><span data-stu-id="64578-131">Detailed settings for recurrence.</span></span> <span data-ttu-id="64578-132">使用标准 Outlook 定期对象。</span><span class="sxs-lookup"><span data-stu-id="64578-132">Using standard Outlook recurrence object.</span></span> <span data-ttu-id="64578-133">请注意，dayOfMonth 不受支持 - 在 recurrenceRange 上使用属性 startDate 确定评价开始的那一天。</span><span class="sxs-lookup"><span data-stu-id="64578-133">Note that dayOfMonth is not supported - use property startDate on recurrenceRange to determine the day the review will start on.</span></span> |
| <span data-ttu-id="64578-134">autoApplyDecisionsEnabled</span><span class="sxs-lookup"><span data-stu-id="64578-134">autoApplyDecisionsEnabled</span></span>|<span data-ttu-id="64578-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="64578-135">Boolean</span></span> | <span data-ttu-id="64578-136">指示是否已启用自动应用功能的标志。</span><span class="sxs-lookup"><span data-stu-id="64578-136">Flag to indicate whether auto-apply feature is enabled.</span></span> |
| <span data-ttu-id="64578-137">applyActions</span><span class="sxs-lookup"><span data-stu-id="64578-137">applyActions</span></span>|<span data-ttu-id="64578-138">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="64578-138">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection</span></span> | <span data-ttu-id="64578-139">可选字段。</span><span class="sxs-lookup"><span data-stu-id="64578-139">Optional field.</span></span> <span data-ttu-id="64578-140">介绍审阅完成后要采取的操作。</span><span class="sxs-lookup"><span data-stu-id="64578-140">Describes the  actions to take once a review is complete.</span></span> <span data-ttu-id="64578-141">目前支持两种类型：默认 (`removeAccessApplyAction` 和) `disableAndDeleteUserApplyAction` 。</span><span class="sxs-lookup"><span data-stu-id="64578-141">There are two types that are currently supported: `removeAccessApplyAction` (default) and `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="64578-142">只需在 的情况下指定字段 `disableAndDeleteUserApplyAction` 。</span><span class="sxs-lookup"><span data-stu-id="64578-142">Field only needs to be specified in the case of `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="64578-143">请参阅 [accessReviewApplyAction](accessreviewapplyaction.md)。</span><span class="sxs-lookup"><span data-stu-id="64578-143">See [accessReviewApplyAction](accessreviewapplyaction.md).</span></span> |
| <span data-ttu-id="64578-144">recommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="64578-144">recommendationsEnabled</span></span>|<span data-ttu-id="64578-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="64578-145">Boolean</span></span> | <span data-ttu-id="64578-146">指示是否启用/禁用决策建议的标志。</span><span class="sxs-lookup"><span data-stu-id="64578-146">Flag to indicate whether decision recommendations are enabled/disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="64578-147">关系</span><span class="sxs-lookup"><span data-stu-id="64578-147">Relationships</span></span>
<span data-ttu-id="64578-148">无。</span><span class="sxs-lookup"><span data-stu-id="64578-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="64578-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64578-149">JSON representation</span></span>
<span data-ttu-id="64578-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64578-150">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleSettings",
  "mailNotificationsEnabled": "Boolean",
  "reminderNotificationsEnabled": "Boolean",
  "justificationRequiredOnApproval": "Boolean",
  "defaultDecisionEnabled": "Boolean",
  "defaultDecision": "String",
  "instanceDurationInDays": "Integer",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "autoApplyDecisionsEnabled": "Boolean",
  "applyActions": [
    {
      "@odata.type": "microsoft.graph.removeAccessApplyAction"
    }
  ],
  "recommendationsEnabled": "Boolean"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScheduleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
