---
title: accessReviewScheduleSettings 资源类型
description: 在 Azure AD access 评论功能中， `accessReviewScheduleSettings` 表示与访问审阅系列相关联的设置。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7cca1fa7fd0da05719c22728dd472087d9737d4e
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000833"
---
# <a name="accessreviewschedulesettings-resource-type"></a><span data-ttu-id="6749c-103">accessReviewScheduleSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="6749c-103">accessReviewScheduleSettings resource type</span></span>

<span data-ttu-id="6749c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6749c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6749c-105">**AccessReviewScheduleSettings** 定义 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)的设置。</span><span class="sxs-lookup"><span data-stu-id="6749c-105">The **accessReviewScheduleSettings** defines the settings of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="6749c-106">属性</span><span class="sxs-lookup"><span data-stu-id="6749c-106">Properties</span></span>
| <span data-ttu-id="6749c-107">属性</span><span class="sxs-lookup"><span data-stu-id="6749c-107">Property</span></span>    | <span data-ttu-id="6749c-108">类型</span><span class="sxs-lookup"><span data-stu-id="6749c-108">Type</span></span>   | <span data-ttu-id="6749c-109">说明</span><span class="sxs-lookup"><span data-stu-id="6749c-109">Description</span></span> |
| :---------------| :---------- | :---------- |
| <span data-ttu-id="6749c-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="6749c-110">mailNotificationsEnabled</span></span>|<span data-ttu-id="6749c-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="6749c-111">Boolean</span></span> | <span data-ttu-id="6749c-112">用于指示是否启用/禁用电子邮件的标志。</span><span class="sxs-lookup"><span data-stu-id="6749c-112">Flag to indicate whether emails are enabled/disabled.</span></span>                |
| <span data-ttu-id="6749c-113">reminderNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="6749c-113">reminderNotificationsEnabled</span></span>|<span data-ttu-id="6749c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="6749c-114">Boolean</span></span>  | <span data-ttu-id="6749c-115">指示是否启用/禁用提醒的标志。</span><span class="sxs-lookup"><span data-stu-id="6749c-115">Flag to indicate whether reminders are enabled/disabled.</span></span>   |
| <span data-ttu-id="6749c-116">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="6749c-116">justificationRequiredOnApproval</span></span>|<span data-ttu-id="6749c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="6749c-117">Boolean</span></span> | <span data-ttu-id="6749c-118">指示是否需要审阅者根据自己的决定提供理由的标志。</span><span class="sxs-lookup"><span data-stu-id="6749c-118">Flag to indicate whether reviewers are required to provide justification with their decision.</span></span> |
| <span data-ttu-id="6749c-119">defaultDecisionEnabled</span><span class="sxs-lookup"><span data-stu-id="6749c-119">defaultDecisionEnabled</span></span>|<span data-ttu-id="6749c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="6749c-120">Boolean</span></span> | <span data-ttu-id="6749c-121">指示在审阅者不响应时是否启用/禁用默认决定的标志。</span><span class="sxs-lookup"><span data-stu-id="6749c-121">Flag to indicate whether default decision is enabled/disabled when reviewers do not respond.</span></span> |
| <span data-ttu-id="6749c-122">defaultDecision</span><span class="sxs-lookup"><span data-stu-id="6749c-122">defaultDecision</span></span>|<span data-ttu-id="6749c-123">字符串</span><span class="sxs-lookup"><span data-stu-id="6749c-123">String</span></span> | <span data-ttu-id="6749c-124">`defaultDecisionEnabled`已启用决策选择。</span><span class="sxs-lookup"><span data-stu-id="6749c-124">Decision chosen if `defaultDecisionEnabled` is enabled.</span></span> <span data-ttu-id="6749c-125">可以是 "批准"、"拒绝" 或 "建议" 之一。</span><span class="sxs-lookup"><span data-stu-id="6749c-125">Can be one of "Approve", "Deny", or "Recommendation".</span></span> |
| <span data-ttu-id="6749c-126">instanceDurationInDays</span><span class="sxs-lookup"><span data-stu-id="6749c-126">instanceDurationInDays</span></span>|<span data-ttu-id="6749c-127">Int32</span><span class="sxs-lookup"><span data-stu-id="6749c-127">Int32</span></span> | <span data-ttu-id="6749c-128">每次重复检查的持续时间 (`accessReviewInstance`) 的天数。</span><span class="sxs-lookup"><span data-stu-id="6749c-128">Duration of each recurrence of review (`accessReviewInstance`) in number of days.</span></span> |
| <span data-ttu-id="6749c-129">recurrence</span><span class="sxs-lookup"><span data-stu-id="6749c-129">recurrence</span></span>|[<span data-ttu-id="6749c-130">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="6749c-130">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) | <span data-ttu-id="6749c-131">定期的详细设置。</span><span class="sxs-lookup"><span data-stu-id="6749c-131">Detailed settings for recurrence.</span></span> <span data-ttu-id="6749c-132">使用标准的 Outlook 定期对象。</span><span class="sxs-lookup"><span data-stu-id="6749c-132">Using standard Outlook recurrence object.</span></span>  |
| <span data-ttu-id="6749c-133">autoApplyDecisionsEnabled</span><span class="sxs-lookup"><span data-stu-id="6749c-133">autoApplyDecisionsEnabled</span></span>|<span data-ttu-id="6749c-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="6749c-134">Boolean</span></span> | <span data-ttu-id="6749c-135">用于指示是否启用自动应用功能的标志。</span><span class="sxs-lookup"><span data-stu-id="6749c-135">Flag to indicate whether auto-apply feature is enabled.</span></span> |
| <span data-ttu-id="6749c-136">applyActions</span><span class="sxs-lookup"><span data-stu-id="6749c-136">applyActions</span></span>|<span data-ttu-id="6749c-137">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6749c-137">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection</span></span> | <span data-ttu-id="6749c-138">可选字段。</span><span class="sxs-lookup"><span data-stu-id="6749c-138">Optional field.</span></span> <span data-ttu-id="6749c-139">介绍完成审阅后要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="6749c-139">Describes the  actions to take once a review is complete.</span></span> <span data-ttu-id="6749c-140">当前支持以下两种类型： `removeAccessApplyAction` (默认) 和 `disableAndDeleteUserApplyAction` 。</span><span class="sxs-lookup"><span data-stu-id="6749c-140">There are two types that are currently supported: `removeAccessApplyAction` (default) and `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="6749c-141">只需在的情况下指定字段 `disableAndDeleteUserApplyAction` 。</span><span class="sxs-lookup"><span data-stu-id="6749c-141">Field only needs to be specified in the case of `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="6749c-142">请参阅 [accessReviewApplyAction](accessreviewapplyaction.md)。</span><span class="sxs-lookup"><span data-stu-id="6749c-142">See [accessReviewApplyAction](accessreviewapplyaction.md).</span></span> |
| <span data-ttu-id="6749c-143">recommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="6749c-143">recommendationsEnabled</span></span>|<span data-ttu-id="6749c-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="6749c-144">Boolean</span></span> | <span data-ttu-id="6749c-145">指示是否启用/禁用决策建议的标志。</span><span class="sxs-lookup"><span data-stu-id="6749c-145">Flag to indicate whether decision recommendations are enabled/disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6749c-146">关系</span><span class="sxs-lookup"><span data-stu-id="6749c-146">Relationships</span></span>
<span data-ttu-id="6749c-147">无。</span><span class="sxs-lookup"><span data-stu-id="6749c-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6749c-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6749c-148">JSON representation</span></span>
<span data-ttu-id="6749c-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6749c-149">The following is a JSON representation of the resource.</span></span>
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
