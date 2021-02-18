---
title: accessReviewSettings 资源类型
description: 在创建访问评审时提供其他设置。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fdc8d22639d098619ef7183ebe22fc9da7bc0287
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50293083"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="80f50-103">accessReviewSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="80f50-103">accessReviewSettings resource type</span></span>

<span data-ttu-id="80f50-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80f50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

<span data-ttu-id="80f50-105">在创建访问评审时提供其他设置，以控制开始访问评审时的功能行为。</span><span class="sxs-lookup"><span data-stu-id="80f50-105">Provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>

## <a name="properties"></a><span data-ttu-id="80f50-106">属性</span><span class="sxs-lookup"><span data-stu-id="80f50-106">Properties</span></span>

| <span data-ttu-id="80f50-107">属性</span><span class="sxs-lookup"><span data-stu-id="80f50-107">Property</span></span> | <span data-ttu-id="80f50-108">类型</span><span class="sxs-lookup"><span data-stu-id="80f50-108">Type</span></span> | <span data-ttu-id="80f50-109">说明</span><span class="sxs-lookup"><span data-stu-id="80f50-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="80f50-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="80f50-110">mailNotificationsEnabled</span></span> | <span data-ttu-id="80f50-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="80f50-111">Boolean</span></span> | <span data-ttu-id="80f50-112">指示是否已启用向审阅者和审阅创建者发送邮件。</span><span class="sxs-lookup"><span data-stu-id="80f50-112">Indicates whether sending mails to reviewers and the review creator is enabled.</span></span> |
| <span data-ttu-id="80f50-113">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="80f50-113">remindersEnabled</span></span> | <span data-ttu-id="80f50-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="80f50-114">Boolean</span></span> | <span data-ttu-id="80f50-115">指示是否已启用向审阅者发送提醒电子邮件。</span><span class="sxs-lookup"><span data-stu-id="80f50-115">Indicates whether sending reminder emails to reviewers is enabled.</span></span> |
| <span data-ttu-id="80f50-116">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="80f50-116">justificationRequiredOnApproval</span></span> | <span data-ttu-id="80f50-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="80f50-117">Boolean</span></span> | <span data-ttu-id="80f50-118">指示审阅者在审阅访问权限时是否需要提供理由。</span><span class="sxs-lookup"><span data-stu-id="80f50-118">Indicates whether reviewers are required to provide a justification when reviewing access.</span></span> |
| <span data-ttu-id="80f50-119">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="80f50-119">activityDurationInDays</span></span> | <span data-ttu-id="80f50-120">Int64</span><span class="sxs-lookup"><span data-stu-id="80f50-120">Int64</span></span> | <span data-ttu-id="80f50-121">要向审阅者显示的用户活动天数。</span><span class="sxs-lookup"><span data-stu-id="80f50-121">The number of days of user activities to show to reviewers.</span></span> |
| <span data-ttu-id="80f50-122">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="80f50-122">autoReviewEnabled</span></span> | <span data-ttu-id="80f50-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="80f50-123">Boolean</span></span> | <span data-ttu-id="80f50-124">指示如果审阅者未提供决策，是否应该设置决策。</span><span class="sxs-lookup"><span data-stu-id="80f50-124">Indicates whether a decision should be set if the reviewer did not supply one.</span></span> <span data-ttu-id="80f50-125">在启用自动应用时使用。</span><span class="sxs-lookup"><span data-stu-id="80f50-125">For use when auto-apply is enabled.</span></span> <span data-ttu-id="80f50-126">如果不希望记录审阅决定，除非审阅者做出明确选择，请设置为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="80f50-126">If you don't want to have a review decision recorded unless the reviewer makes an explicit choice, set it to `false`.</span></span>|
| <span data-ttu-id="80f50-127">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="80f50-127">autoReviewSettings</span></span> | [<span data-ttu-id="80f50-128">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="80f50-128">autoReviewSettings</span></span>](autoreviewsettings.md) | <span data-ttu-id="80f50-129">功能如何设置审阅决定的详细设置。</span><span class="sxs-lookup"><span data-stu-id="80f50-129">Detailed settings for how the feature should set the review decision.</span></span> <span data-ttu-id="80f50-130">在启用自动应用时使用。</span><span class="sxs-lookup"><span data-stu-id="80f50-130">For use when auto-apply is enabled.</span></span> |
| <span data-ttu-id="80f50-131">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="80f50-131">recurrenceSettings</span></span> | [<span data-ttu-id="80f50-132">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="80f50-132">accessReviewRecurrenceSettings</span></span>](accessreviewrecurrencesettings.md) | <span data-ttu-id="80f50-133">定期的详细设置。</span><span class="sxs-lookup"><span data-stu-id="80f50-133">Detailed settings for recurrence.</span></span> |
| <span data-ttu-id="80f50-134">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="80f50-134">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="80f50-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="80f50-135">Boolean</span></span> | <span data-ttu-id="80f50-136">指示是否启用自动应用功能以自动更改目标对象访问资源。</span><span class="sxs-lookup"><span data-stu-id="80f50-136">Indicates whether the auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="80f50-137">如果未启用，则用户必须在审阅完成后应用访问评审。</span><span class="sxs-lookup"><span data-stu-id="80f50-137">If not enabled, a user must, after the review completes, apply the access review.</span></span> |
| <span data-ttu-id="80f50-138">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="80f50-138">accessRecommendationsEnabled</span></span> | <span data-ttu-id="80f50-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="80f50-139">Boolean</span></span> | <span data-ttu-id="80f50-140">指示是否已启用向审阅者显示建议。</span><span class="sxs-lookup"><span data-stu-id="80f50-140">Indicates whether showing recommendations to reviewers is enabled.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="80f50-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80f50-141">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}-->
```json
{
  "mailNotificationsEnabled": true,
  "remindersEnabled": true,  
  "justificationRequiredOnApproval": true,
  "activityDurationInDays": 1024,
  "autoReviewEnabled": false,
  "autoReviewSettings": {"@odata.type": "microsoft.graph.autoReviewSettings"},
  "recurrenceSettings": {"@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"},
  "autoApplyReviewResultsEnabled": false,
  "accessRecommendationsEnabled": false
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
