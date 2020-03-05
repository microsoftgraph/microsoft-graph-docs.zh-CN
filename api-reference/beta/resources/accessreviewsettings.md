---
title: accessReviewSettings 资源类型
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: ''
ms.openlocfilehash: 21915811da771bd0eebdb5fb2c16df5cfbdea096
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508455"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="07ee4-102">accessReviewSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="07ee4-102">accessReviewSettings resource type</span></span>

<span data-ttu-id="07ee4-103">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="07ee4-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="07ee4-104">属性</span><span class="sxs-lookup"><span data-stu-id="07ee4-104">Properties</span></span>
|<span data-ttu-id="07ee4-105">属性</span><span class="sxs-lookup"><span data-stu-id="07ee4-105">Property</span></span>|<span data-ttu-id="07ee4-106">类型</span><span class="sxs-lookup"><span data-stu-id="07ee4-106">Type</span></span>|<span data-ttu-id="07ee4-107">说明</span><span class="sxs-lookup"><span data-stu-id="07ee4-107">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="07ee4-108">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="07ee4-108">mailNotificationsEnabled</span></span> | <span data-ttu-id="07ee4-109">boolean</span><span class="sxs-lookup"><span data-stu-id="07ee4-109">boolean</span></span> |  |
| <span data-ttu-id="07ee4-110">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="07ee4-110">remindersEnabled</span></span> | <span data-ttu-id="07ee4-111">boolean</span><span class="sxs-lookup"><span data-stu-id="07ee4-111">boolean</span></span> |  |
| <span data-ttu-id="07ee4-112">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="07ee4-112">justificationRequiredOnApproval</span></span> | <span data-ttu-id="07ee4-113">boolean</span><span class="sxs-lookup"><span data-stu-id="07ee4-113">boolean</span></span> |  |
| <span data-ttu-id="07ee4-114">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="07ee4-114">recurrenceSettings</span></span> | <span data-ttu-id="07ee4-115">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="07ee4-115">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="07ee4-116">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="07ee4-116">autoReviewEnabled</span></span> | <span data-ttu-id="07ee4-117">boolean</span><span class="sxs-lookup"><span data-stu-id="07ee4-117">boolean</span></span> |  |
| <span data-ttu-id="07ee4-118">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="07ee4-118">activityDurationInDays</span></span> | <span data-ttu-id="07ee4-119">Int32</span><span class="sxs-lookup"><span data-stu-id="07ee4-119">Int32</span></span> |  |
| <span data-ttu-id="07ee4-120">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="07ee4-120">autoReviewSettings</span></span> | <span data-ttu-id="07ee4-121">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="07ee4-121">autoReviewSettings</span></span> |  |
| <span data-ttu-id="07ee4-122">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="07ee4-122">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="07ee4-123">boolean</span><span class="sxs-lookup"><span data-stu-id="07ee4-123">boolean</span></span> |  |
| <span data-ttu-id="07ee4-124">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="07ee4-124">accessRecommendationsEnabled</span></span> | <span data-ttu-id="07ee4-125">boolean</span><span class="sxs-lookup"><span data-stu-id="07ee4-125">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="07ee4-126">关系</span><span class="sxs-lookup"><span data-stu-id="07ee4-126">Relationships</span></span>
<span data-ttu-id="07ee4-127">无</span><span class="sxs-lookup"><span data-stu-id="07ee4-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="07ee4-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07ee4-128">JSON Representation</span></span>
<span data-ttu-id="07ee4-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07ee4-129">Here is a JSON representation of the resource.</span></span>
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



