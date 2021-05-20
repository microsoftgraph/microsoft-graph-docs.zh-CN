---
title: patternedRecurrence 资源类型
description: 定期模式和区域。
localization_priority: Normal
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 57e42faaaa30be31c45be7bfec6ad9ee17ffc869
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546201"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="099a7-103">patternedRecurrence 资源类型</span><span class="sxs-lookup"><span data-stu-id="099a7-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="099a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="099a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="099a7-105">定期模式和区域。</span><span class="sxs-lookup"><span data-stu-id="099a7-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="099a7-106">属性</span><span class="sxs-lookup"><span data-stu-id="099a7-106">Properties</span></span>
| <span data-ttu-id="099a7-107">属性</span><span class="sxs-lookup"><span data-stu-id="099a7-107">Property</span></span>     | <span data-ttu-id="099a7-108">类型</span><span class="sxs-lookup"><span data-stu-id="099a7-108">Type</span></span>   |<span data-ttu-id="099a7-109">说明</span><span class="sxs-lookup"><span data-stu-id="099a7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="099a7-110">模式</span><span class="sxs-lookup"><span data-stu-id="099a7-110">pattern</span></span>|[<span data-ttu-id="099a7-111">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="099a7-111">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="099a7-112">事件发生的频率。</span><span class="sxs-lookup"><span data-stu-id="099a7-112">The frequency of an event.</span></span>|
|<span data-ttu-id="099a7-113">区域</span><span class="sxs-lookup"><span data-stu-id="099a7-113">range</span></span>|[<span data-ttu-id="099a7-114">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="099a7-114">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="099a7-115">事件的持续时间。</span><span class="sxs-lookup"><span data-stu-id="099a7-115">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="099a7-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="099a7-116">JSON representation</span></span>

<span data-ttu-id="099a7-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="099a7-117">Here is a JSON representation of the resource</span></span>

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

