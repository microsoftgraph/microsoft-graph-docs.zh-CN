---
title: patternedRecurrence 资源类型
description: 定期模式和区域。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: 9fb6741ab3710ae71c27dfe32870b6f3e3411dd5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998108"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="660e7-103">patternedRecurrence 资源类型</span><span class="sxs-lookup"><span data-stu-id="660e7-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="660e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="660e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="660e7-105">定期模式和区域。</span><span class="sxs-lookup"><span data-stu-id="660e7-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="660e7-106">属性</span><span class="sxs-lookup"><span data-stu-id="660e7-106">Properties</span></span>
| <span data-ttu-id="660e7-107">属性</span><span class="sxs-lookup"><span data-stu-id="660e7-107">Property</span></span>     | <span data-ttu-id="660e7-108">类型</span><span class="sxs-lookup"><span data-stu-id="660e7-108">Type</span></span>   |<span data-ttu-id="660e7-109">说明</span><span class="sxs-lookup"><span data-stu-id="660e7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="660e7-110">模式</span><span class="sxs-lookup"><span data-stu-id="660e7-110">pattern</span></span>|[<span data-ttu-id="660e7-111">recurrencePattern</span><span class="sxs-lookup"><span data-stu-id="660e7-111">recurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="660e7-112">事件发生的频率。</span><span class="sxs-lookup"><span data-stu-id="660e7-112">The frequency of an event.</span></span>|
|<span data-ttu-id="660e7-113">区域</span><span class="sxs-lookup"><span data-stu-id="660e7-113">range</span></span>|[<span data-ttu-id="660e7-114">recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="660e7-114">recurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="660e7-115">事件的持续时间。</span><span class="sxs-lookup"><span data-stu-id="660e7-115">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="660e7-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="660e7-116">JSON representation</span></span>

<span data-ttu-id="660e7-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="660e7-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedRecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


