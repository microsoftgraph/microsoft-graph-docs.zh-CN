---
title: accessReviewRecurrenceSettings 资源类型
description: 指定定期重复访问评审。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cb2a05589bfa92331a213a489bfb2a5129850065
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755656"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="7dbed-103">accessReviewRecurrenceSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="7dbed-103">accessReviewRecurrenceSettings resource type</span></span>

<span data-ttu-id="7dbed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dbed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

<span data-ttu-id="7dbed-105">**accessReviewRecurrenceSettings** 资源类型在 [accessReviewSettings](accessreviewsettings.md)资源中使用，并指定定期重复访问评审。</span><span class="sxs-lookup"><span data-stu-id="7dbed-105">The **accessReviewRecurrenceSettings** resource type is used in the [accessReviewSettings](accessreviewsettings.md) resource and specifies that the access review recurs at regular intervals.</span></span>

## <a name="properties"></a><span data-ttu-id="7dbed-106">属性</span><span class="sxs-lookup"><span data-stu-id="7dbed-106">Properties</span></span>

| <span data-ttu-id="7dbed-107">属性</span><span class="sxs-lookup"><span data-stu-id="7dbed-107">Property</span></span> | <span data-ttu-id="7dbed-108">类型</span><span class="sxs-lookup"><span data-stu-id="7dbed-108">Type</span></span> | <span data-ttu-id="7dbed-109">说明</span><span class="sxs-lookup"><span data-stu-id="7dbed-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="7dbed-110">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="7dbed-110">recurrenceType</span></span> | <span data-ttu-id="7dbed-111">String</span><span class="sxs-lookup"><span data-stu-id="7dbed-111">String</span></span> | <span data-ttu-id="7dbed-112">定期间隔。</span><span class="sxs-lookup"><span data-stu-id="7dbed-112">The recurrence interval.</span></span> <span data-ttu-id="7dbed-113">可能的模块 `onetime` `weekly` `monthly` ：、、、或 `quarterly` `halfyearly` `annual` 。</span><span class="sxs-lookup"><span data-stu-id="7dbed-113">Possible vaules: `onetime`, `weekly`, `monthly`, `quarterly`, `halfyearly` or `annual`.</span></span>                                                                   |
| <span data-ttu-id="7dbed-114">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="7dbed-114">recurrenceEndType</span></span> | <span data-ttu-id="7dbed-115">String</span><span class="sxs-lookup"><span data-stu-id="7dbed-115">String</span></span> | <span data-ttu-id="7dbed-116">定期的结束时间。</span><span class="sxs-lookup"><span data-stu-id="7dbed-116">How the recurrence ends.</span></span> <span data-ttu-id="7dbed-117">可能的值 `never` `endBy` ：、、 `occurrences` 或 `recurrenceCount` 。</span><span class="sxs-lookup"><span data-stu-id="7dbed-117">Possible values: `never`, `endBy`, `occurrences`, or `recurrenceCount`.</span></span> <span data-ttu-id="7dbed-118">如果是 ， `never` 则定期系列没有显式结束。</span><span class="sxs-lookup"><span data-stu-id="7dbed-118">If it is `never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="7dbed-119">如果是 ， `endBy` 则重复周期在特定日期结束。</span><span class="sxs-lookup"><span data-stu-id="7dbed-119">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="7dbed-120">如果是 ， `occurrences` 则系列将在审阅 `recurrenceCount` 实例完成后结束。</span><span class="sxs-lookup"><span data-stu-id="7dbed-120">If it is `occurrences`, then the series ends after `recurrenceCount` instances of the review have completed.</span></span> |
| <span data-ttu-id="7dbed-121">durationInDays</span><span class="sxs-lookup"><span data-stu-id="7dbed-121">durationInDays</span></span> | <span data-ttu-id="7dbed-122">Int32</span><span class="sxs-lookup"><span data-stu-id="7dbed-122">Int32</span></span> | <span data-ttu-id="7dbed-123">重复周期的持续时间（以天表示）。</span><span class="sxs-lookup"><span data-stu-id="7dbed-123">The duration in days for recurrence.</span></span> |
| <span data-ttu-id="7dbed-124">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="7dbed-124">recurrenceCount</span></span> | <span data-ttu-id="7dbed-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7dbed-125">Int32</span></span> | <span data-ttu-id="7dbed-126">定期计数（如果 **recurrenceEndType** 的值为 `occurrences` ，否则为 `0` ）。</span><span class="sxs-lookup"><span data-stu-id="7dbed-126">The count of recurrences, if the value of **recurrenceEndType** is `occurrences`, or `0` otherwise.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7dbed-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7dbed-127">JSON representation</span></span>

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
