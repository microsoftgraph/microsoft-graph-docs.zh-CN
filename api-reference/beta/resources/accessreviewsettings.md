---
title: accessReviewSettings 资源类型
description: 在创建访问评审时提供其他设置。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4de925ecb2fac65e3ab339ba8d4e602fcdc2af3
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330352"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="b831b-103">accessReviewSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b831b-103">accessReviewSettings resource type</span></span>

<span data-ttu-id="b831b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b831b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b831b-105">在创建访问评审时提供其他设置，以在启动访问评审时控制功能行为。</span><span class="sxs-lookup"><span data-stu-id="b831b-105">Provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>

## <a name="properties"></a><span data-ttu-id="b831b-106">属性</span><span class="sxs-lookup"><span data-stu-id="b831b-106">Properties</span></span>

| <span data-ttu-id="b831b-107">属性</span><span class="sxs-lookup"><span data-stu-id="b831b-107">Property</span></span> | <span data-ttu-id="b831b-108">类型</span><span class="sxs-lookup"><span data-stu-id="b831b-108">Type</span></span> | <span data-ttu-id="b831b-109">说明</span><span class="sxs-lookup"><span data-stu-id="b831b-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="b831b-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="b831b-110">mailNotificationsEnabled</span></span> | <span data-ttu-id="b831b-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="b831b-111">Boolean</span></span> | <span data-ttu-id="b831b-112">指示是否已启用向审阅者发送邮件和审阅创建者。</span><span class="sxs-lookup"><span data-stu-id="b831b-112">Indicates whether sending mails to reviewers and the review creator is enabled.</span></span> |
| <span data-ttu-id="b831b-113">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="b831b-113">remindersEnabled</span></span> | <span data-ttu-id="b831b-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="b831b-114">Boolean</span></span> | <span data-ttu-id="b831b-115">指示是否启用了向审阅者发送提醒电子邮件。</span><span class="sxs-lookup"><span data-stu-id="b831b-115">Indicates whether sending reminder emails to reviewers is enabled.</span></span> |
| <span data-ttu-id="b831b-116">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="b831b-116">justificationRequiredOnApproval</span></span> | <span data-ttu-id="b831b-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="b831b-117">Boolean</span></span> | <span data-ttu-id="b831b-118">指示审阅 access 时是否需要审阅者提供理由。</span><span class="sxs-lookup"><span data-stu-id="b831b-118">Indicates whether reviewers are required to provide a justification when reviewing access.</span></span> |
| <span data-ttu-id="b831b-119">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="b831b-119">activityDurationInDays</span></span> | <span data-ttu-id="b831b-120">Int64</span><span class="sxs-lookup"><span data-stu-id="b831b-120">Int64</span></span> | <span data-ttu-id="b831b-121">向审阅者显示的用户活动的天数。</span><span class="sxs-lookup"><span data-stu-id="b831b-121">The number of days of user activities to show to reviewers.</span></span> |
| <span data-ttu-id="b831b-122">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="b831b-122">autoReviewEnabled</span></span> | <span data-ttu-id="b831b-123">布尔值</span><span class="sxs-lookup"><span data-stu-id="b831b-123">Boolean</span></span> | <span data-ttu-id="b831b-124">指示是否应在审阅者未提供某个决定时对其进行设置。</span><span class="sxs-lookup"><span data-stu-id="b831b-124">Indicates whether a decision should be set if the reviewer did not supply one.</span></span> <span data-ttu-id="b831b-125">在启用自动应用程序时使用。</span><span class="sxs-lookup"><span data-stu-id="b831b-125">For use when auto-apply is enabled.</span></span> <span data-ttu-id="b831b-126">如果您不希望在审阅者做出明确选择的情况下记录审阅决策，请将其设置为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="b831b-126">If you don't want to have a review decision recorded unless the reviewer makes an explicit choice, set it to `false`.</span></span>|
| <span data-ttu-id="b831b-127">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="b831b-127">autoReviewSettings</span></span> | [<span data-ttu-id="b831b-128">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="b831b-128">autoReviewSettings</span></span>](autoreviewsettings.md) | <span data-ttu-id="b831b-129">有关功能应如何设置评审决策的详细设置。</span><span class="sxs-lookup"><span data-stu-id="b831b-129">Detailed settings for how the feature should set the review decision.</span></span> <span data-ttu-id="b831b-130">在启用自动应用程序时使用。</span><span class="sxs-lookup"><span data-stu-id="b831b-130">For use when auto-apply is enabled.</span></span> |
| <span data-ttu-id="b831b-131">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="b831b-131">recurrenceSettings</span></span> | [<span data-ttu-id="b831b-132">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="b831b-132">accessReviewRecurrenceSettings</span></span>](accessreviewrecurrencesettings.md) | <span data-ttu-id="b831b-133">定期的详细设置。</span><span class="sxs-lookup"><span data-stu-id="b831b-133">Detailed settings for recurrence.</span></span> |
| <span data-ttu-id="b831b-134">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="b831b-134">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="b831b-135">布尔值</span><span class="sxs-lookup"><span data-stu-id="b831b-135">Boolean</span></span> | <span data-ttu-id="b831b-136">指示是否启用自动更改目标对象访问资源的自动应用功能。</span><span class="sxs-lookup"><span data-stu-id="b831b-136">Indicates whether the auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="b831b-137">如果未启用，则用户必须在评审完成后应用访问评审。</span><span class="sxs-lookup"><span data-stu-id="b831b-137">If not enabled, a user must, after the review completes, apply the access review.</span></span> |
| <span data-ttu-id="b831b-138">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="b831b-138">accessRecommendationsEnabled</span></span> | <span data-ttu-id="b831b-139">布尔值</span><span class="sxs-lookup"><span data-stu-id="b831b-139">Boolean</span></span> | <span data-ttu-id="b831b-140">指示是否已启用向审阅者显示建议。</span><span class="sxs-lookup"><span data-stu-id="b831b-140">Indicates whether showing recommendations to reviewers is enabled.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b831b-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b831b-141">JSON representation</span></span>
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