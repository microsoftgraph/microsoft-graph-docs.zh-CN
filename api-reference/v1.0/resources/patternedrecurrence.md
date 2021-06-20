---
title: patternedRecurrence 资源类型
description: 定期模式和区域。
localization_priority: Normal
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5bc4c78a4996c6690f40de863d20ba6f2d55949a
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030871"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="8cb8d-103">patternedRecurrence 资源类型</span><span class="sxs-lookup"><span data-stu-id="8cb8d-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="8cb8d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cb8d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8cb8d-105">定期模式和区域。</span><span class="sxs-lookup"><span data-stu-id="8cb8d-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="8cb8d-106">属性</span><span class="sxs-lookup"><span data-stu-id="8cb8d-106">Properties</span></span>
| <span data-ttu-id="8cb8d-107">属性</span><span class="sxs-lookup"><span data-stu-id="8cb8d-107">Property</span></span>     | <span data-ttu-id="8cb8d-108">类型</span><span class="sxs-lookup"><span data-stu-id="8cb8d-108">Type</span></span>   |<span data-ttu-id="8cb8d-109">说明</span><span class="sxs-lookup"><span data-stu-id="8cb8d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cb8d-110">模式</span><span class="sxs-lookup"><span data-stu-id="8cb8d-110">pattern</span></span>|[<span data-ttu-id="8cb8d-111">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="8cb8d-111">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="8cb8d-112">事件发生的频率。</span><span class="sxs-lookup"><span data-stu-id="8cb8d-112">The frequency of an event.</span></span> <span data-ttu-id="8cb8d-113">不要指定一次访问评审。</span><span class="sxs-lookup"><span data-stu-id="8cb8d-113">Do not specify for a one-time access review.</span></span>|
|<span data-ttu-id="8cb8d-114">区域</span><span class="sxs-lookup"><span data-stu-id="8cb8d-114">range</span></span>|[<span data-ttu-id="8cb8d-115">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="8cb8d-115">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="8cb8d-116">事件的持续时间。</span><span class="sxs-lookup"><span data-stu-id="8cb8d-116">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8cb8d-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8cb8d-117">JSON representation</span></span>

<span data-ttu-id="8cb8d-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cb8d-118">Here is a JSON representation of the resource</span></span>

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

