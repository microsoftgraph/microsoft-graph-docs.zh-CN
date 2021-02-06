---
title: accessReviewScheduleSettings 资源类型
description: 在 Azure AD 访问评审功能中，表示与访问 `accessReviewScheduleSettings` 评审系列关联的设置。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3a58ba9a682e443efbc159befaea61b15e3fdc81
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133442"
---
# <a name="accessreviewschedulesettings-resource-type"></a><span data-ttu-id="6437d-103">accessReviewScheduleSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="6437d-103">accessReviewScheduleSettings resource type</span></span>

<span data-ttu-id="6437d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6437d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6437d-105">**accessReviewScheduleSettings** 定义 [accessReviewScheduleDefinition 的设置](accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="6437d-105">The **accessReviewScheduleSettings** defines the settings of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="6437d-106">属性</span><span class="sxs-lookup"><span data-stu-id="6437d-106">Properties</span></span>
| <span data-ttu-id="6437d-107">属性</span><span class="sxs-lookup"><span data-stu-id="6437d-107">Property</span></span>    | <span data-ttu-id="6437d-108">类型</span><span class="sxs-lookup"><span data-stu-id="6437d-108">Type</span></span>   | <span data-ttu-id="6437d-109">说明</span><span class="sxs-lookup"><span data-stu-id="6437d-109">Description</span></span> |
| :---------------| :---------- | :---------- |
| <span data-ttu-id="6437d-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="6437d-110">mailNotificationsEnabled</span></span>|<span data-ttu-id="6437d-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="6437d-111">Boolean</span></span> | <span data-ttu-id="6437d-112">指示电子邮件是否已启用/禁用的标志。</span><span class="sxs-lookup"><span data-stu-id="6437d-112">Flag to indicate whether emails are enabled/disabled.</span></span>                |
| <span data-ttu-id="6437d-113">reminderNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="6437d-113">reminderNotificationsEnabled</span></span>|<span data-ttu-id="6437d-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="6437d-114">Boolean</span></span>  | <span data-ttu-id="6437d-115">指示是否启用/禁用提醒的标志。</span><span class="sxs-lookup"><span data-stu-id="6437d-115">Flag to indicate whether reminders are enabled/disabled.</span></span>   |
| <span data-ttu-id="6437d-116">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="6437d-116">justificationRequiredOnApproval</span></span>|<span data-ttu-id="6437d-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="6437d-117">Boolean</span></span> | <span data-ttu-id="6437d-118">用于指示是否需要审阅者提供其决策理由的标志。</span><span class="sxs-lookup"><span data-stu-id="6437d-118">Flag to indicate whether reviewers are required to provide justification with their decision.</span></span> |
| <span data-ttu-id="6437d-119">defaultDecisionEnabled</span><span class="sxs-lookup"><span data-stu-id="6437d-119">defaultDecisionEnabled</span></span>|<span data-ttu-id="6437d-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="6437d-120">Boolean</span></span> | <span data-ttu-id="6437d-121">指示在审阅者未响应时是否启用/禁用默认决策的标志。</span><span class="sxs-lookup"><span data-stu-id="6437d-121">Flag to indicate whether default decision is enabled/disabled when reviewers do not respond.</span></span> |
| <span data-ttu-id="6437d-122">defaultDecision</span><span class="sxs-lookup"><span data-stu-id="6437d-122">defaultDecision</span></span>|<span data-ttu-id="6437d-123">字符串</span><span class="sxs-lookup"><span data-stu-id="6437d-123">String</span></span> | <span data-ttu-id="6437d-124">如果已启用， `defaultDecisionEnabled` 则选择决策。</span><span class="sxs-lookup"><span data-stu-id="6437d-124">Decision chosen if `defaultDecisionEnabled` is enabled.</span></span> <span data-ttu-id="6437d-125">可以是"批准"、"拒绝"或"建议"之一。</span><span class="sxs-lookup"><span data-stu-id="6437d-125">Can be one of "Approve", "Deny", or "Recommendation".</span></span> |
| <span data-ttu-id="6437d-126">instanceDurationInDays</span><span class="sxs-lookup"><span data-stu-id="6437d-126">instanceDurationInDays</span></span>|<span data-ttu-id="6437d-127">Int32</span><span class="sxs-lookup"><span data-stu-id="6437d-127">Int32</span></span> | <span data-ttu-id="6437d-128">每次重复审阅的持续时间 `accessReviewInstance` () 天数。</span><span class="sxs-lookup"><span data-stu-id="6437d-128">Duration of each recurrence of review (`accessReviewInstance`) in number of days.</span></span> |
| <span data-ttu-id="6437d-129">recurrence</span><span class="sxs-lookup"><span data-stu-id="6437d-129">recurrence</span></span>|[<span data-ttu-id="6437d-130">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="6437d-130">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) | <span data-ttu-id="6437d-131">定期的详细设置。</span><span class="sxs-lookup"><span data-stu-id="6437d-131">Detailed settings for recurrence.</span></span> <span data-ttu-id="6437d-132">使用标准 Outlook 定期对象。</span><span class="sxs-lookup"><span data-stu-id="6437d-132">Using standard Outlook recurrence object.</span></span>  |
| <span data-ttu-id="6437d-133">autoApplyDecisionsEnabled</span><span class="sxs-lookup"><span data-stu-id="6437d-133">autoApplyDecisionsEnabled</span></span>|<span data-ttu-id="6437d-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="6437d-134">Boolean</span></span> | <span data-ttu-id="6437d-135">用于指示是否已启用自动应用功能的标志。</span><span class="sxs-lookup"><span data-stu-id="6437d-135">Flag to indicate whether auto-apply feature is enabled.</span></span> |
| <span data-ttu-id="6437d-136">applyActions</span><span class="sxs-lookup"><span data-stu-id="6437d-136">applyActions</span></span>|<span data-ttu-id="6437d-137">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6437d-137">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection</span></span> | <span data-ttu-id="6437d-138">可选字段。</span><span class="sxs-lookup"><span data-stu-id="6437d-138">Optional field.</span></span> <span data-ttu-id="6437d-139">介绍在审阅完成后要采取的操作。</span><span class="sxs-lookup"><span data-stu-id="6437d-139">Describes the  actions to take once a review is complete.</span></span> <span data-ttu-id="6437d-140">目前支持两种类型：默认 (`removeAccessApplyAction` 和 `disableAndDeleteUserApplyAction`) 。</span><span class="sxs-lookup"><span data-stu-id="6437d-140">There are two types that are currently supported: `removeAccessApplyAction` (default) and `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="6437d-141">字段只需要在 . `disableAndDeleteUserApplyAction`</span><span class="sxs-lookup"><span data-stu-id="6437d-141">Field only needs to be specified in the case of `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="6437d-142">请参阅 [accessReviewApplyAction](accessreviewapplyaction.md)。</span><span class="sxs-lookup"><span data-stu-id="6437d-142">See [accessReviewApplyAction](accessreviewapplyaction.md).</span></span> |
| <span data-ttu-id="6437d-143">recommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="6437d-143">recommendationsEnabled</span></span>|<span data-ttu-id="6437d-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="6437d-144">Boolean</span></span> | <span data-ttu-id="6437d-145">指示是否启用/禁用决策建议的标志。</span><span class="sxs-lookup"><span data-stu-id="6437d-145">Flag to indicate whether decision recommendations are enabled/disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6437d-146">关系</span><span class="sxs-lookup"><span data-stu-id="6437d-146">Relationships</span></span>
<span data-ttu-id="6437d-147">无。</span><span class="sxs-lookup"><span data-stu-id="6437d-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6437d-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6437d-148">JSON representation</span></span>
<span data-ttu-id="6437d-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6437d-149">The following is a JSON representation of the resource.</span></span>
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
