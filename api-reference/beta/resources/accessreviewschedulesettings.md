---
title: accessReviewScheduleSettings 资源类型
description: 在 Azure AD 访问评审功能中，表示与访问 `accessReviewScheduleSettings` 评审系列关联的设置。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b354ebfc2b5e6c8093f65c8712516421f0b1d332
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579730"
---
# <a name="accessreviewschedulesettings-resource-type"></a><span data-ttu-id="4d183-103">accessReviewScheduleSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d183-103">accessReviewScheduleSettings resource type</span></span>

<span data-ttu-id="4d183-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d183-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="4d183-105">**accessReviewScheduleSettings** 定义 [accessReviewScheduleDefinition 的设置](accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="4d183-105">The **accessReviewScheduleSettings** defines the settings of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="4d183-106">属性</span><span class="sxs-lookup"><span data-stu-id="4d183-106">Properties</span></span>
| <span data-ttu-id="4d183-107">属性</span><span class="sxs-lookup"><span data-stu-id="4d183-107">Property</span></span>    | <span data-ttu-id="4d183-108">类型</span><span class="sxs-lookup"><span data-stu-id="4d183-108">Type</span></span>   | <span data-ttu-id="4d183-109">说明</span><span class="sxs-lookup"><span data-stu-id="4d183-109">Description</span></span> |
| :---------------| :---------- | :---------- |
| <span data-ttu-id="4d183-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="4d183-110">mailNotificationsEnabled</span></span>|<span data-ttu-id="4d183-111">布尔</span><span class="sxs-lookup"><span data-stu-id="4d183-111">Boolean</span></span> | <span data-ttu-id="4d183-112">指示是启用还是禁用电子邮件。</span><span class="sxs-lookup"><span data-stu-id="4d183-112">Indicates whether emails are enabled or disabled.</span></span> <span data-ttu-id="4d183-113">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="4d183-113">Default value is `false`.</span></span>               |
| <span data-ttu-id="4d183-114">reminderNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="4d183-114">reminderNotificationsEnabled</span></span>|<span data-ttu-id="4d183-115">布尔</span><span class="sxs-lookup"><span data-stu-id="4d183-115">Boolean</span></span>  | <span data-ttu-id="4d183-116">指示是启用还是禁用提醒。</span><span class="sxs-lookup"><span data-stu-id="4d183-116">Indicates whether reminders are enabled or disabled.</span></span> <span data-ttu-id="4d183-117">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="4d183-117">Default value is `false`.</span></span>  |
| <span data-ttu-id="4d183-118">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="4d183-118">justificationRequiredOnApproval</span></span>|<span data-ttu-id="4d183-119">布尔</span><span class="sxs-lookup"><span data-stu-id="4d183-119">Boolean</span></span> | <span data-ttu-id="4d183-120">指示是否要求审阅者提供其决策的理由。</span><span class="sxs-lookup"><span data-stu-id="4d183-120">Indicates whether reviewers are required to provide justification with their decision.</span></span> <span data-ttu-id="4d183-121">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="4d183-121">Default value is `false`.</span></span> |
| <span data-ttu-id="4d183-122">defaultDecisionEnabled</span><span class="sxs-lookup"><span data-stu-id="4d183-122">defaultDecisionEnabled</span></span>|<span data-ttu-id="4d183-123">布尔</span><span class="sxs-lookup"><span data-stu-id="4d183-123">Boolean</span></span> | <span data-ttu-id="4d183-124">指示在审阅者未响应时是启用还是禁用默认决策。</span><span class="sxs-lookup"><span data-stu-id="4d183-124">Indicates whether the default decision is enabled or disabled when reviewers do not respond.</span></span> <span data-ttu-id="4d183-125">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="4d183-125">Default value is `false`.</span></span> |
| <span data-ttu-id="4d183-126">defaultDecision</span><span class="sxs-lookup"><span data-stu-id="4d183-126">defaultDecision</span></span>|<span data-ttu-id="4d183-127">String</span><span class="sxs-lookup"><span data-stu-id="4d183-127">String</span></span> | <span data-ttu-id="4d183-128">如果已启用， `defaultDecisionEnabled` 则选择决策。</span><span class="sxs-lookup"><span data-stu-id="4d183-128">Decision chosen if `defaultDecisionEnabled` is enabled.</span></span> <span data-ttu-id="4d183-129">可以是 、 `Approve` `Deny` 或 `Recommendation` 之一。</span><span class="sxs-lookup"><span data-stu-id="4d183-129">Can be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |
| <span data-ttu-id="4d183-130">instanceDurationInDays</span><span class="sxs-lookup"><span data-stu-id="4d183-130">instanceDurationInDays</span></span>|<span data-ttu-id="4d183-131">Int32</span><span class="sxs-lookup"><span data-stu-id="4d183-131">Int32</span></span> | <span data-ttu-id="4d183-132">每次重复审阅的持续时间 () `accessReviewInstance` 天数表示。</span><span class="sxs-lookup"><span data-stu-id="4d183-132">Duration of each recurrence of review (`accessReviewInstance`) in number of days.</span></span> |
| <span data-ttu-id="4d183-133">recurrence</span><span class="sxs-lookup"><span data-stu-id="4d183-133">recurrence</span></span>|[<span data-ttu-id="4d183-134">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="4d183-134">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) | <span data-ttu-id="4d183-135">使用标准定期对象定期Outlook设置。</span><span class="sxs-lookup"><span data-stu-id="4d183-135">Detailed settings for recurrence using the standard Outlook recurrence object.</span></span> <span data-ttu-id="4d183-136">仅 `weekly` 支持 `absoluteMonthly` **recurrencePattern 和 recurrencePattern。**</span><span class="sxs-lookup"><span data-stu-id="4d183-136">Only `weekly` and `absoluteMonthly` on **recurrencePattern** are supported.</span></span> <span data-ttu-id="4d183-137">使用 **recurrenceRange 上的 属性 startDate** 确定审阅开始的一天。 </span><span class="sxs-lookup"><span data-stu-id="4d183-137">Use the property **startDate** on **recurrenceRange** to determine the day the review starts.</span></span> |
| <span data-ttu-id="4d183-138">autoApplyDecisionsEnabled</span><span class="sxs-lookup"><span data-stu-id="4d183-138">autoApplyDecisionsEnabled</span></span>|<span data-ttu-id="4d183-139">布尔</span><span class="sxs-lookup"><span data-stu-id="4d183-139">Boolean</span></span> | <span data-ttu-id="4d183-140">指示是否自动应用决策。</span><span class="sxs-lookup"><span data-stu-id="4d183-140">Indicates whether decisions are automatically applied.</span></span> <span data-ttu-id="4d183-141">设置为 时，用户必须在审阅者完成访问评审后 `false` 手动应用决策。</span><span class="sxs-lookup"><span data-stu-id="4d183-141">When set to `false`, a user must apply the decisions manually once the reviewer completes the access review.</span></span> <span data-ttu-id="4d183-142">设置为 时，会在访问评审实例持续时间结束后自动应用决策，无论审阅 `true` 者是否已回复。</span><span class="sxs-lookup"><span data-stu-id="4d183-142">When set to `true`, decisions are applied automatically after the access review instance duration ends, whether or not the reviewers have responded.</span></span> <span data-ttu-id="4d183-143">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="4d183-143">Default value is `false`.</span></span> |
| <span data-ttu-id="4d183-144">applyActions</span><span class="sxs-lookup"><span data-stu-id="4d183-144">applyActions</span></span>|<span data-ttu-id="4d183-145">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4d183-145">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection</span></span> | <span data-ttu-id="4d183-146">可选字段。</span><span class="sxs-lookup"><span data-stu-id="4d183-146">Optional field.</span></span> <span data-ttu-id="4d183-147">介绍审阅完成后要采取的操作。</span><span class="sxs-lookup"><span data-stu-id="4d183-147">Describes the  actions to take once a review is complete.</span></span> <span data-ttu-id="4d183-148">目前支持两种类型：默认 (`removeAccessApplyAction` 和) `disableAndDeleteUserApplyAction` 。</span><span class="sxs-lookup"><span data-stu-id="4d183-148">There are two types that are currently supported: `removeAccessApplyAction` (default) and `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="4d183-149">只需在 的情况下指定字段 `disableAndDeleteUserApplyAction` 。</span><span class="sxs-lookup"><span data-stu-id="4d183-149">Field only needs to be specified in the case of `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="4d183-150">请参阅 [accessReviewApplyAction](accessreviewapplyaction.md)。</span><span class="sxs-lookup"><span data-stu-id="4d183-150">See [accessReviewApplyAction](accessreviewapplyaction.md).</span></span> |
| <span data-ttu-id="4d183-151">recommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="4d183-151">recommendationsEnabled</span></span>|<span data-ttu-id="4d183-152">布尔</span><span class="sxs-lookup"><span data-stu-id="4d183-152">Boolean</span></span> | <span data-ttu-id="4d183-153">指示是否启用/禁用决策建议。</span><span class="sxs-lookup"><span data-stu-id="4d183-153">Indicates whether decision recommendations are enabled/disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4d183-154">关系</span><span class="sxs-lookup"><span data-stu-id="4d183-154">Relationships</span></span>
<span data-ttu-id="4d183-155">无。</span><span class="sxs-lookup"><span data-stu-id="4d183-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d183-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d183-156">JSON representation</span></span>
<span data-ttu-id="4d183-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d183-157">The following is a JSON representation of the resource.</span></span>
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
