---
title: accessReviewSettings 资源类型
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: ''
ms.openlocfilehash: 2c51d94b3143d9929c03093cfb1a6625d6a9e3db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974519"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="89c47-102">accessReviewSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="89c47-102">accessReviewSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="89c47-103">属性</span><span class="sxs-lookup"><span data-stu-id="89c47-103">Properties</span></span>
|<span data-ttu-id="89c47-104">属性</span><span class="sxs-lookup"><span data-stu-id="89c47-104">Property</span></span>|<span data-ttu-id="89c47-105">类型</span><span class="sxs-lookup"><span data-stu-id="89c47-105">Type</span></span>|<span data-ttu-id="89c47-106">说明</span><span class="sxs-lookup"><span data-stu-id="89c47-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="89c47-107">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="89c47-107">mailNotificationsEnabled</span></span> | <span data-ttu-id="89c47-108">boolean</span><span class="sxs-lookup"><span data-stu-id="89c47-108">boolean</span></span> |  |
| <span data-ttu-id="89c47-109">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="89c47-109">remindersEnabled</span></span> | <span data-ttu-id="89c47-110">boolean</span><span class="sxs-lookup"><span data-stu-id="89c47-110">boolean</span></span> |  |
| <span data-ttu-id="89c47-111">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="89c47-111">justificationRequiredOnApproval</span></span> | <span data-ttu-id="89c47-112">boolean</span><span class="sxs-lookup"><span data-stu-id="89c47-112">boolean</span></span> |  |
| <span data-ttu-id="89c47-113">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="89c47-113">recurrenceSettings</span></span> | <span data-ttu-id="89c47-114">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="89c47-114">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="89c47-115">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="89c47-115">autoReviewEnabled</span></span> | <span data-ttu-id="89c47-116">boolean</span><span class="sxs-lookup"><span data-stu-id="89c47-116">boolean</span></span> |  |
| <span data-ttu-id="89c47-117">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="89c47-117">activityDurationInDays</span></span> | <span data-ttu-id="89c47-118">Int32</span><span class="sxs-lookup"><span data-stu-id="89c47-118">Int32</span></span> |  |
| <span data-ttu-id="89c47-119">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="89c47-119">autoReviewSettings</span></span> | <span data-ttu-id="89c47-120">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="89c47-120">autoReviewSettings</span></span> |  |
| <span data-ttu-id="89c47-121">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="89c47-121">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="89c47-122">boolean</span><span class="sxs-lookup"><span data-stu-id="89c47-122">boolean</span></span> |  |
| <span data-ttu-id="89c47-123">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="89c47-123">accessRecommendationsEnabled</span></span> | <span data-ttu-id="89c47-124">boolean</span><span class="sxs-lookup"><span data-stu-id="89c47-124">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="89c47-125">关系</span><span class="sxs-lookup"><span data-stu-id="89c47-125">Relationships</span></span>
<span data-ttu-id="89c47-126">无</span><span class="sxs-lookup"><span data-stu-id="89c47-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="89c47-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89c47-127">JSON Representation</span></span>
<span data-ttu-id="89c47-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89c47-128">Here is a JSON representation of the resource.</span></span>
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



