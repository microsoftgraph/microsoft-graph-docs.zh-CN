---
title: accessReviewRecurrenceSettings 资源类型
description: 指定定期重复访问评审。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9a39881a7675598d12de79f2738a1e14d1c759b3
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292920"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="ac6eb-103">accessReviewRecurrenceSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac6eb-103">accessReviewRecurrenceSettings resource type</span></span>

<span data-ttu-id="ac6eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac6eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

<span data-ttu-id="ac6eb-105">**accessReviewRecurrenceSettings** 资源类型用于 [accessReviewSettings](accessreviewsettings.md)资源，并指定访问评审定期定期发生。</span><span class="sxs-lookup"><span data-stu-id="ac6eb-105">The **accessReviewRecurrenceSettings** resource type is used in the [accessReviewSettings](accessreviewsettings.md) resource and specifies that the access review recurs at regular intervals.</span></span>

## <a name="properties"></a><span data-ttu-id="ac6eb-106">属性</span><span class="sxs-lookup"><span data-stu-id="ac6eb-106">Properties</span></span>

| <span data-ttu-id="ac6eb-107">属性</span><span class="sxs-lookup"><span data-stu-id="ac6eb-107">Property</span></span> | <span data-ttu-id="ac6eb-108">类型</span><span class="sxs-lookup"><span data-stu-id="ac6eb-108">Type</span></span> | <span data-ttu-id="ac6eb-109">说明</span><span class="sxs-lookup"><span data-stu-id="ac6eb-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="ac6eb-110">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="ac6eb-110">recurrenceType</span></span> | <span data-ttu-id="ac6eb-111">String</span><span class="sxs-lookup"><span data-stu-id="ac6eb-111">String</span></span> | <span data-ttu-id="ac6eb-112">定期间隔。</span><span class="sxs-lookup"><span data-stu-id="ac6eb-112">The recurrence interval.</span></span> <span data-ttu-id="ac6eb-113">可能的 vaules： `onetime` ， ， ， 或 `weekly` `monthly` `quarterly` `halfyearly` `annual` 。</span><span class="sxs-lookup"><span data-stu-id="ac6eb-113">Possible vaules: `onetime`, `weekly`, `monthly`, `quarterly`, `halfyearly` or `annual`.</span></span>                                                                   |
| <span data-ttu-id="ac6eb-114">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="ac6eb-114">recurrenceEndType</span></span> | <span data-ttu-id="ac6eb-115">String</span><span class="sxs-lookup"><span data-stu-id="ac6eb-115">String</span></span> | <span data-ttu-id="ac6eb-116">重复周期结束时间。</span><span class="sxs-lookup"><span data-stu-id="ac6eb-116">How the recurrence ends.</span></span> <span data-ttu-id="ac6eb-117">可能的值 `never` `endBy` `occurrences` ：、、或 `recurrenceCount` 。</span><span class="sxs-lookup"><span data-stu-id="ac6eb-117">Possible values: `never`, `endBy`, `occurrences`, or `recurrenceCount`.</span></span> <span data-ttu-id="ac6eb-118">如果是， `never` 则定期系列没有显式结束。</span><span class="sxs-lookup"><span data-stu-id="ac6eb-118">If it is `never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="ac6eb-119">如果是， `endBy` 重复周期将在特定日期结束。</span><span class="sxs-lookup"><span data-stu-id="ac6eb-119">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="ac6eb-120">如果是，则系列将在审阅实例完成后 `occurrences` `recurrenceCount` 结束。</span><span class="sxs-lookup"><span data-stu-id="ac6eb-120">If it is `occurrences`, then the series ends after `recurrenceCount` instances of the review have completed.</span></span> |
| <span data-ttu-id="ac6eb-121">durationInDays</span><span class="sxs-lookup"><span data-stu-id="ac6eb-121">durationInDays</span></span> | <span data-ttu-id="ac6eb-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ac6eb-122">Int32</span></span> | <span data-ttu-id="ac6eb-123">重复周期的持续时间（以天表示）。</span><span class="sxs-lookup"><span data-stu-id="ac6eb-123">The duration in days for recurrence.</span></span> |
| <span data-ttu-id="ac6eb-124">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="ac6eb-124">recurrenceCount</span></span> | <span data-ttu-id="ac6eb-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ac6eb-125">Int32</span></span> | <span data-ttu-id="ac6eb-126">定期计数（如果 **recurrenceEndType** 的值为 ，否则为 `occurrences` 0）。</span><span class="sxs-lookup"><span data-stu-id="ac6eb-126">The count of recurrences, if the value of **recurrenceEndType** is `occurrences`, or 0 otherwise.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ac6eb-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac6eb-127">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"
}-->
```json
{
  "recurrenceType": "string",
  "recurrenceEndType": "string",
  "durationInDays": 1024,
  "recurrenceCount": 1024
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewRecurrenceSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
