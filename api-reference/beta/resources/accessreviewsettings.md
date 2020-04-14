---
title: accessReviewSettings 资源类型
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 978b8f80b6a357ffeb2efced005e395787fedabf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457093"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="80ae6-102">accessReviewSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="80ae6-102">accessReviewSettings resource type</span></span>

<span data-ttu-id="80ae6-103">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80ae6-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="80ae6-104">属性</span><span class="sxs-lookup"><span data-stu-id="80ae6-104">Properties</span></span>
|<span data-ttu-id="80ae6-105">属性</span><span class="sxs-lookup"><span data-stu-id="80ae6-105">Property</span></span>|<span data-ttu-id="80ae6-106">类型</span><span class="sxs-lookup"><span data-stu-id="80ae6-106">Type</span></span>|<span data-ttu-id="80ae6-107">说明</span><span class="sxs-lookup"><span data-stu-id="80ae6-107">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="80ae6-108">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="80ae6-108">mailNotificationsEnabled</span></span> | <span data-ttu-id="80ae6-109">boolean</span><span class="sxs-lookup"><span data-stu-id="80ae6-109">boolean</span></span> |  |
| <span data-ttu-id="80ae6-110">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="80ae6-110">remindersEnabled</span></span> | <span data-ttu-id="80ae6-111">boolean</span><span class="sxs-lookup"><span data-stu-id="80ae6-111">boolean</span></span> |  |
| <span data-ttu-id="80ae6-112">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="80ae6-112">justificationRequiredOnApproval</span></span> | <span data-ttu-id="80ae6-113">boolean</span><span class="sxs-lookup"><span data-stu-id="80ae6-113">boolean</span></span> |  |
| <span data-ttu-id="80ae6-114">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="80ae6-114">recurrenceSettings</span></span> | <span data-ttu-id="80ae6-115">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="80ae6-115">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="80ae6-116">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="80ae6-116">autoReviewEnabled</span></span> | <span data-ttu-id="80ae6-117">boolean</span><span class="sxs-lookup"><span data-stu-id="80ae6-117">boolean</span></span> |  |
| <span data-ttu-id="80ae6-118">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="80ae6-118">activityDurationInDays</span></span> | <span data-ttu-id="80ae6-119">Int32</span><span class="sxs-lookup"><span data-stu-id="80ae6-119">Int32</span></span> |  |
| <span data-ttu-id="80ae6-120">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="80ae6-120">autoReviewSettings</span></span> | <span data-ttu-id="80ae6-121">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="80ae6-121">autoReviewSettings</span></span> |  |
| <span data-ttu-id="80ae6-122">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="80ae6-122">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="80ae6-123">boolean</span><span class="sxs-lookup"><span data-stu-id="80ae6-123">boolean</span></span> |  |
| <span data-ttu-id="80ae6-124">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="80ae6-124">accessRecommendationsEnabled</span></span> | <span data-ttu-id="80ae6-125">boolean</span><span class="sxs-lookup"><span data-stu-id="80ae6-125">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="80ae6-126">关系</span><span class="sxs-lookup"><span data-stu-id="80ae6-126">Relationships</span></span>
<span data-ttu-id="80ae6-127">无</span><span class="sxs-lookup"><span data-stu-id="80ae6-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80ae6-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80ae6-128">JSON Representation</span></span>
<span data-ttu-id="80ae6-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80ae6-129">Here is a JSON representation of the resource.</span></span>
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



