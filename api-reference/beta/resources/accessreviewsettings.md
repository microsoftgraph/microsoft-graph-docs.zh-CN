---
title: accessReviewSettings 资源类型
description: ''
localization_priority: Normal
ms.openlocfilehash: b19db8add3143f02f51cc0ef9d38d483d54438e1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348352"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="82f67-102">accessReviewSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="82f67-102">accessReviewSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="82f67-103">属性</span><span class="sxs-lookup"><span data-stu-id="82f67-103">Properties</span></span>
|<span data-ttu-id="82f67-104">属性</span><span class="sxs-lookup"><span data-stu-id="82f67-104">Property</span></span>|<span data-ttu-id="82f67-105">类型</span><span class="sxs-lookup"><span data-stu-id="82f67-105">Type</span></span>|<span data-ttu-id="82f67-106">说明</span><span class="sxs-lookup"><span data-stu-id="82f67-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="82f67-107">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="82f67-107">mailNotificationsEnabled</span></span> | <span data-ttu-id="82f67-108">布尔</span><span class="sxs-lookup"><span data-stu-id="82f67-108">boolean</span></span> |  |
| <span data-ttu-id="82f67-109">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="82f67-109">remindersEnabled</span></span> | <span data-ttu-id="82f67-110">布尔</span><span class="sxs-lookup"><span data-stu-id="82f67-110">boolean</span></span> |  |
| <span data-ttu-id="82f67-111">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="82f67-111">justificationRequiredOnApproval</span></span> | <span data-ttu-id="82f67-112">布尔</span><span class="sxs-lookup"><span data-stu-id="82f67-112">boolean</span></span> |  |
| <span data-ttu-id="82f67-113">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="82f67-113">recurrenceSettings</span></span> | <span data-ttu-id="82f67-114">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="82f67-114">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="82f67-115">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="82f67-115">autoReviewEnabled</span></span> | <span data-ttu-id="82f67-116">布尔</span><span class="sxs-lookup"><span data-stu-id="82f67-116">boolean</span></span> |  |
| <span data-ttu-id="82f67-117">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="82f67-117">activityDurationInDays</span></span> | <span data-ttu-id="82f67-118">Int32</span><span class="sxs-lookup"><span data-stu-id="82f67-118">Int32</span></span> |  |
| <span data-ttu-id="82f67-119">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="82f67-119">autoReviewSettings</span></span> | <span data-ttu-id="82f67-120">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="82f67-120">autoReviewSettings</span></span> |  |
| <span data-ttu-id="82f67-121">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="82f67-121">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="82f67-122">布尔</span><span class="sxs-lookup"><span data-stu-id="82f67-122">boolean</span></span> |  |
| <span data-ttu-id="82f67-123">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="82f67-123">accessRecommendationsEnabled</span></span> | <span data-ttu-id="82f67-124">布尔</span><span class="sxs-lookup"><span data-stu-id="82f67-124">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="82f67-125">关系</span><span class="sxs-lookup"><span data-stu-id="82f67-125">Relationships</span></span>
<span data-ttu-id="82f67-126">无</span><span class="sxs-lookup"><span data-stu-id="82f67-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="82f67-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82f67-127">JSON Representation</span></span>
<span data-ttu-id="82f67-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82f67-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}-->
``` json
{
    "mailNotificationsEnabled":"boolean",
    "remindersEnabled":"boolean",
    "justificationRequiredOnApproval":"boolean",
    "recurrenceSettings":"microsoft.graph.accessReviewRecurrenceSettings",
    "autoReviewEnabled":"boolean",
    "activityDurationInDays":"Int32",
    "autoReviewSettings":"microsoft.graph.autoReviewSettings",
    "autoApplyReviewResultsEnabled":"boolean",
    "accessRecommendationsEnabled":"boolean"
}
```



