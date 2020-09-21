---
title: patternedRecurrence 资源类型
description: 定期模式和区域。
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: edf6013b4c0293eb79b2b21aafc5a6ce944b0fa2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002973"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="53b92-103">patternedRecurrence 资源类型</span><span class="sxs-lookup"><span data-stu-id="53b92-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="53b92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53b92-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53b92-105">定期模式和区域。</span><span class="sxs-lookup"><span data-stu-id="53b92-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="53b92-106">属性</span><span class="sxs-lookup"><span data-stu-id="53b92-106">Properties</span></span>
| <span data-ttu-id="53b92-107">属性</span><span class="sxs-lookup"><span data-stu-id="53b92-107">Property</span></span>     | <span data-ttu-id="53b92-108">类型</span><span class="sxs-lookup"><span data-stu-id="53b92-108">Type</span></span>   |<span data-ttu-id="53b92-109">说明</span><span class="sxs-lookup"><span data-stu-id="53b92-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53b92-110">模式</span><span class="sxs-lookup"><span data-stu-id="53b92-110">pattern</span></span>|[<span data-ttu-id="53b92-111">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="53b92-111">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="53b92-112">事件发生的频率。</span><span class="sxs-lookup"><span data-stu-id="53b92-112">The frequency of an event.</span></span>|
|<span data-ttu-id="53b92-113">区域</span><span class="sxs-lookup"><span data-stu-id="53b92-113">range</span></span>|[<span data-ttu-id="53b92-114">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="53b92-114">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="53b92-115">事件的持续时间。</span><span class="sxs-lookup"><span data-stu-id="53b92-115">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53b92-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53b92-116">JSON representation</span></span>

<span data-ttu-id="53b92-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53b92-117">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

