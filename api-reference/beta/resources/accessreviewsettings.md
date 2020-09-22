---
title: accessReviewSettings 资源类型
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 201f0c0ac11a0e26174661aa4d8a63baf23f7f3c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024561"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="99880-102">accessReviewSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="99880-102">accessReviewSettings resource type</span></span>

<span data-ttu-id="99880-103">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99880-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="99880-104">属性</span><span class="sxs-lookup"><span data-stu-id="99880-104">Properties</span></span>
|<span data-ttu-id="99880-105">属性</span><span class="sxs-lookup"><span data-stu-id="99880-105">Property</span></span>|<span data-ttu-id="99880-106">类型</span><span class="sxs-lookup"><span data-stu-id="99880-106">Type</span></span>|<span data-ttu-id="99880-107">说明</span><span class="sxs-lookup"><span data-stu-id="99880-107">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="99880-108">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="99880-108">mailNotificationsEnabled</span></span> | <span data-ttu-id="99880-109">boolean</span><span class="sxs-lookup"><span data-stu-id="99880-109">boolean</span></span> |  |
| <span data-ttu-id="99880-110">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="99880-110">remindersEnabled</span></span> | <span data-ttu-id="99880-111">boolean</span><span class="sxs-lookup"><span data-stu-id="99880-111">boolean</span></span> |  |
| <span data-ttu-id="99880-112">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="99880-112">justificationRequiredOnApproval</span></span> | <span data-ttu-id="99880-113">boolean</span><span class="sxs-lookup"><span data-stu-id="99880-113">boolean</span></span> |  |
| <span data-ttu-id="99880-114">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="99880-114">recurrenceSettings</span></span> | <span data-ttu-id="99880-115">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="99880-115">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="99880-116">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="99880-116">autoReviewEnabled</span></span> | <span data-ttu-id="99880-117">boolean</span><span class="sxs-lookup"><span data-stu-id="99880-117">boolean</span></span> |  |
| <span data-ttu-id="99880-118">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="99880-118">activityDurationInDays</span></span> | <span data-ttu-id="99880-119">Int32</span><span class="sxs-lookup"><span data-stu-id="99880-119">Int32</span></span> |  |
| <span data-ttu-id="99880-120">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="99880-120">autoReviewSettings</span></span> | <span data-ttu-id="99880-121">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="99880-121">autoReviewSettings</span></span> |  |
| <span data-ttu-id="99880-122">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="99880-122">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="99880-123">boolean</span><span class="sxs-lookup"><span data-stu-id="99880-123">boolean</span></span> |  |
| <span data-ttu-id="99880-124">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="99880-124">accessRecommendationsEnabled</span></span> | <span data-ttu-id="99880-125">boolean</span><span class="sxs-lookup"><span data-stu-id="99880-125">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="99880-126">关系</span><span class="sxs-lookup"><span data-stu-id="99880-126">Relationships</span></span>
<span data-ttu-id="99880-127">无</span><span class="sxs-lookup"><span data-stu-id="99880-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="99880-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99880-128">JSON Representation</span></span>
<span data-ttu-id="99880-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99880-129">Here is a JSON representation of the resource.</span></span>
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





