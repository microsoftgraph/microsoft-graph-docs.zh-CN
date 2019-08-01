---
title: patternedRecurrence 资源类型
description: 定期模式和区域。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a5ad30474b23c6ef96bbc1a66142098e7f696138
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035565"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="d107f-103">patternedRecurrence 资源类型</span><span class="sxs-lookup"><span data-stu-id="d107f-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="d107f-104">定期模式和区域。</span><span class="sxs-lookup"><span data-stu-id="d107f-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="d107f-105">属性</span><span class="sxs-lookup"><span data-stu-id="d107f-105">Properties</span></span>
| <span data-ttu-id="d107f-106">属性</span><span class="sxs-lookup"><span data-stu-id="d107f-106">Property</span></span>     | <span data-ttu-id="d107f-107">类型</span><span class="sxs-lookup"><span data-stu-id="d107f-107">Type</span></span>   |<span data-ttu-id="d107f-108">说明</span><span class="sxs-lookup"><span data-stu-id="d107f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d107f-109">模式</span><span class="sxs-lookup"><span data-stu-id="d107f-109">pattern</span></span>|[<span data-ttu-id="d107f-110">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="d107f-110">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="d107f-111">事件发生的频率。</span><span class="sxs-lookup"><span data-stu-id="d107f-111">The frequency of an event.</span></span>|
|<span data-ttu-id="d107f-112">区域</span><span class="sxs-lookup"><span data-stu-id="d107f-112">range</span></span>|[<span data-ttu-id="d107f-113">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="d107f-113">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="d107f-114">事件的持续时间。</span><span class="sxs-lookup"><span data-stu-id="d107f-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d107f-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d107f-115">JSON representation</span></span>

<span data-ttu-id="d107f-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d107f-116">Here is a JSON representation of the resource</span></span>

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
