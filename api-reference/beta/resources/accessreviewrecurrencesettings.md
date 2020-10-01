---
title: accessReviewRecurrenceSettings 资源类型
description: 指定以固定间隔重复进行访问评审。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3ca66a818059efac84903f763e6be3c8a3b5c05a
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330165"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="41297-103">accessReviewRecurrenceSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="41297-103">accessReviewRecurrenceSettings resource type</span></span>

<span data-ttu-id="41297-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41297-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41297-105">**AccessReviewRecurrenceSettings**资源类型在[accessReviewSettings](accessreviewsettings.md)资源中使用，并指定以固定间隔重复进行访问评审。</span><span class="sxs-lookup"><span data-stu-id="41297-105">The **accessReviewRecurrenceSettings** resource type is used in the [accessReviewSettings](accessreviewsettings.md) resource and specifies that the access review recurs at regular intervals.</span></span>

## <a name="properties"></a><span data-ttu-id="41297-106">属性</span><span class="sxs-lookup"><span data-stu-id="41297-106">Properties</span></span>

| <span data-ttu-id="41297-107">属性</span><span class="sxs-lookup"><span data-stu-id="41297-107">Property</span></span> | <span data-ttu-id="41297-108">类型</span><span class="sxs-lookup"><span data-stu-id="41297-108">Type</span></span> | <span data-ttu-id="41297-109">说明</span><span class="sxs-lookup"><span data-stu-id="41297-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="41297-110">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="41297-110">recurrenceType</span></span> | <span data-ttu-id="41297-111">字符串</span><span class="sxs-lookup"><span data-stu-id="41297-111">String</span></span> | <span data-ttu-id="41297-112">定期间隔。</span><span class="sxs-lookup"><span data-stu-id="41297-112">The recurrence interval.</span></span> <span data-ttu-id="41297-113">可能的 vaules： `onetime` 、 `weekly` 、、 `monthly` `quarterly` `halfyearly` 或 `annual` 。</span><span class="sxs-lookup"><span data-stu-id="41297-113">Possible vaules: `onetime`, `weekly`, `monthly`, `quarterly`, `halfyearly` or `annual`.</span></span>                                                                   |
| <span data-ttu-id="41297-114">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="41297-114">recurrenceEndType</span></span> | <span data-ttu-id="41297-115">字符串</span><span class="sxs-lookup"><span data-stu-id="41297-115">String</span></span> | <span data-ttu-id="41297-116">重复周期的结束方式。</span><span class="sxs-lookup"><span data-stu-id="41297-116">How the recurrence ends.</span></span> <span data-ttu-id="41297-117">可能的值： `never` 、、 `endBy` `occurrences` 或 `recurrenceCount` 。</span><span class="sxs-lookup"><span data-stu-id="41297-117">Possible values: `never`, `endBy`, `occurrences`, or `recurrenceCount`.</span></span> <span data-ttu-id="41297-118">如果是，则不 `never` 会出现定期系列的显式结束。</span><span class="sxs-lookup"><span data-stu-id="41297-118">If it is `never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="41297-119">如果是 `endBy` ，则重复周期将在特定日期结束。</span><span class="sxs-lookup"><span data-stu-id="41297-119">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="41297-120">如果是 `occurrences` ，则在审阅的实例完成后，该系列将结束 `recurrenceCount` 。</span><span class="sxs-lookup"><span data-stu-id="41297-120">If it is `occurrences`, then the series ends after `recurrenceCount` instances of the review have completed.</span></span> |
| <span data-ttu-id="41297-121">durationInDays</span><span class="sxs-lookup"><span data-stu-id="41297-121">durationInDays</span></span> | <span data-ttu-id="41297-122">Int32</span><span class="sxs-lookup"><span data-stu-id="41297-122">Int32</span></span> | <span data-ttu-id="41297-123">定期的持续时间（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="41297-123">The duration in days for recurrence.</span></span> |
| <span data-ttu-id="41297-124">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="41297-124">recurrenceCount</span></span> | <span data-ttu-id="41297-125">Int32</span><span class="sxs-lookup"><span data-stu-id="41297-125">Int32</span></span> | <span data-ttu-id="41297-126">如果 **recurrenceEndType** 的值为，则为定期计数 `occurrences` ，否则为0。</span><span class="sxs-lookup"><span data-stu-id="41297-126">The count of recurrences, if the value of **recurrenceEndType** is `occurrences`, or 0 otherwise.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="41297-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41297-127">JSON representation</span></span>

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