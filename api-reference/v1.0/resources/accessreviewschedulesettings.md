---
title: accessReviewScheduleSettings 资源类型
description: 表示与访问评审系列关联的设置。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8120d5b9b40f5e2ad744b65dcf927516e1d868b8
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031041"
---
# <a name="accessreviewschedulesettings-resource-type"></a><span data-ttu-id="0f3ea-103">accessReviewScheduleSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f3ea-103">accessReviewScheduleSettings resource type</span></span>

<span data-ttu-id="0f3ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f3ea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f3ea-105">**accessReviewScheduleSettings** 定义 [accessReviewScheduleDefinition 的设置](accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-105">The **accessReviewScheduleSettings** defines the settings of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="0f3ea-106">属性</span><span class="sxs-lookup"><span data-stu-id="0f3ea-106">Properties</span></span>
|<span data-ttu-id="0f3ea-107">属性</span><span class="sxs-lookup"><span data-stu-id="0f3ea-107">Property</span></span>|<span data-ttu-id="0f3ea-108">类型</span><span class="sxs-lookup"><span data-stu-id="0f3ea-108">Type</span></span>|<span data-ttu-id="0f3ea-109">说明</span><span class="sxs-lookup"><span data-stu-id="0f3ea-109">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="0f3ea-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="0f3ea-110">mailNotificationsEnabled</span></span>|<span data-ttu-id="0f3ea-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f3ea-111">Boolean</span></span> | <span data-ttu-id="0f3ea-112">指示是启用还是禁用电子邮件。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-112">Indicates whether emails are enabled or disabled.</span></span> <span data-ttu-id="0f3ea-113">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-113">Default value is `false`.</span></span>               |
| <span data-ttu-id="0f3ea-114">reminderNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="0f3ea-114">reminderNotificationsEnabled</span></span>|<span data-ttu-id="0f3ea-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f3ea-115">Boolean</span></span>  | <span data-ttu-id="0f3ea-116">指示是启用还是禁用提醒。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-116">Indicates whether reminders are enabled or disabled.</span></span> <span data-ttu-id="0f3ea-117">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-117">Default value is `false`.</span></span>  |
| <span data-ttu-id="0f3ea-118">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="0f3ea-118">justificationRequiredOnApproval</span></span>|<span data-ttu-id="0f3ea-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f3ea-119">Boolean</span></span> | <span data-ttu-id="0f3ea-120">指示是否要求审阅者提供其决策的理由。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-120">Indicates whether reviewers are required to provide justification with their decision.</span></span> <span data-ttu-id="0f3ea-121">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-121">Default value is `false`.</span></span> |
| <span data-ttu-id="0f3ea-122">defaultDecisionEnabled</span><span class="sxs-lookup"><span data-stu-id="0f3ea-122">defaultDecisionEnabled</span></span>|<span data-ttu-id="0f3ea-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f3ea-123">Boolean</span></span> | <span data-ttu-id="0f3ea-124">指示在审阅者未响应时是启用还是禁用默认决策。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-124">Indicates whether the default decision is enabled or disabled when reviewers do not respond.</span></span> <span data-ttu-id="0f3ea-125">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-125">Default value is `false`.</span></span> |
| <span data-ttu-id="0f3ea-126">defaultDecision</span><span class="sxs-lookup"><span data-stu-id="0f3ea-126">defaultDecision</span></span>|<span data-ttu-id="0f3ea-127">String</span><span class="sxs-lookup"><span data-stu-id="0f3ea-127">String</span></span> | <span data-ttu-id="0f3ea-128">如果 **defaultDecisionEnabled** 为 ，则选择决策 `true` 。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-128">Decision chosen if **defaultDecisionEnabled** is `true`.</span></span> <span data-ttu-id="0f3ea-129">可以是 、 `Approve` `Deny` 或 `Recommendation` 之一。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-129">Can be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |
| <span data-ttu-id="0f3ea-130">instanceDurationInDays</span><span class="sxs-lookup"><span data-stu-id="0f3ea-130">instanceDurationInDays</span></span>|<span data-ttu-id="0f3ea-131">Int32</span><span class="sxs-lookup"><span data-stu-id="0f3ea-131">Int32</span></span> | <span data-ttu-id="0f3ea-132">每次定期检查的持续时间 (**accessReviewInstance**) 天数表示。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-132">Duration of each recurrence of review (**accessReviewInstance**) in number of days.</span></span> |
| <span data-ttu-id="0f3ea-133">recurrence</span><span class="sxs-lookup"><span data-stu-id="0f3ea-133">recurrence</span></span>|[<span data-ttu-id="0f3ea-134">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="0f3ea-134">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) | <span data-ttu-id="0f3ea-135">使用标准定期对象定期Outlook设置。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-135">Detailed settings for recurrence using the standard Outlook recurrence object.</span></span> <span data-ttu-id="0f3ea-136">仅 `weekly` 支持 `absoluteMonthly` **recurrencePattern 和 recurrencePattern。**</span><span class="sxs-lookup"><span data-stu-id="0f3ea-136">Only `weekly` and `absoluteMonthly` on **recurrencePattern** are supported.</span></span> <span data-ttu-id="0f3ea-137">使用 **recurrenceRange 上的 属性 startDate** 确定审阅开始的一天。 </span><span class="sxs-lookup"><span data-stu-id="0f3ea-137">Use the property **startDate** on **recurrenceRange** to determine the day the review starts.</span></span> |
| <span data-ttu-id="0f3ea-138">autoApplyDecisionsEnabled</span><span class="sxs-lookup"><span data-stu-id="0f3ea-138">autoApplyDecisionsEnabled</span></span>|<span data-ttu-id="0f3ea-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f3ea-139">Boolean</span></span> | <span data-ttu-id="0f3ea-140">指示是否自动应用决策。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-140">Indicates whether decisions are automatically applied.</span></span> <span data-ttu-id="0f3ea-141">设置为 时，用户必须在审阅者完成访问评审后 `false` 手动应用决策。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-141">When set to `false`, a user must apply the decisions manually once the reviewer completes the access review.</span></span> <span data-ttu-id="0f3ea-142">设置为 时，会在访问评审实例持续时间结束后自动应用决策，无论审阅 `true` 者是否已回复。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-142">When set to `true`, decisions are applied automatically after the access review instance duration ends, whether or not the reviewers have responded.</span></span> <span data-ttu-id="0f3ea-143">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-143">Default value is `false`.</span></span> |
| <span data-ttu-id="0f3ea-144">applyActions</span><span class="sxs-lookup"><span data-stu-id="0f3ea-144">applyActions</span></span>|<span data-ttu-id="0f3ea-145">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0f3ea-145">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection</span></span> | <span data-ttu-id="0f3ea-146">可选字段。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-146">Optional field.</span></span> <span data-ttu-id="0f3ea-147">介绍审阅完成后要采取的操作。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-147">Describes the  actions to take once a review is complete.</span></span> <span data-ttu-id="0f3ea-148">目前支持两种类型：默认 (`removeAccessApplyAction` 和) `disableAndDeleteUserApplyAction` 。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-148">There are two types that are currently supported: `removeAccessApplyAction` (default) and `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="0f3ea-149">只需在 的情况下指定字段 `disableAndDeleteUserApplyAction` 。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-149">Field only needs to be specified in the case of `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="0f3ea-150">请参阅 [accessReviewApplyAction](accessreviewapplyaction.md)。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-150">See [accessReviewApplyAction](accessreviewapplyaction.md).</span></span> |
| <span data-ttu-id="0f3ea-151">recommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="0f3ea-151">recommendationsEnabled</span></span>|<span data-ttu-id="0f3ea-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f3ea-152">Boolean</span></span> | <span data-ttu-id="0f3ea-153">指示是启用还是禁用决策建议。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-153">Indicates whether decision recommendations are enabled or disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0f3ea-154">关系</span><span class="sxs-lookup"><span data-stu-id="0f3ea-154">Relationships</span></span>
<span data-ttu-id="0f3ea-155">无。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f3ea-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f3ea-156">JSON representation</span></span>
<span data-ttu-id="0f3ea-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f3ea-157">The following is a JSON representation of the resource.</span></span>
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
