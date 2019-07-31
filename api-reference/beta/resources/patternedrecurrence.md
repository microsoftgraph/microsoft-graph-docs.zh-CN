---
title: patternedRecurrence 资源类型
description: 定期模式和区域。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 463e3324d3a32d0679584a3aa2dddbe6613d2925
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966193"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="59b1e-103">patternedRecurrence 资源类型</span><span class="sxs-lookup"><span data-stu-id="59b1e-103">patternedRecurrence resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59b1e-104">定期模式和区域。</span><span class="sxs-lookup"><span data-stu-id="59b1e-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="59b1e-105">属性</span><span class="sxs-lookup"><span data-stu-id="59b1e-105">Properties</span></span>
| <span data-ttu-id="59b1e-106">属性</span><span class="sxs-lookup"><span data-stu-id="59b1e-106">Property</span></span>     | <span data-ttu-id="59b1e-107">类型</span><span class="sxs-lookup"><span data-stu-id="59b1e-107">Type</span></span>   |<span data-ttu-id="59b1e-108">说明</span><span class="sxs-lookup"><span data-stu-id="59b1e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59b1e-109">模式</span><span class="sxs-lookup"><span data-stu-id="59b1e-109">pattern</span></span>|[<span data-ttu-id="59b1e-110">recurrencePattern</span><span class="sxs-lookup"><span data-stu-id="59b1e-110">recurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="59b1e-111">事件发生的频率。</span><span class="sxs-lookup"><span data-stu-id="59b1e-111">The frequency of an event.</span></span>|
|<span data-ttu-id="59b1e-112">区域</span><span class="sxs-lookup"><span data-stu-id="59b1e-112">range</span></span>|[<span data-ttu-id="59b1e-113">recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="59b1e-113">recurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="59b1e-114">事件的持续时间。</span><span class="sxs-lookup"><span data-stu-id="59b1e-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59b1e-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59b1e-115">JSON representation</span></span>

<span data-ttu-id="59b1e-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59b1e-116">Here is a JSON representation of the resource</span></span>

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
