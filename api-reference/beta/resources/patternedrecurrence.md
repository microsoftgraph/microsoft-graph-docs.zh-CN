---
title: patternedRecurrence 资源类型
description: 定期模式和区域。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: harini84
ms.openlocfilehash: baff2147ee0a9e03e4e55a143341171707dee2d7
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579301"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="d8662-103">patternedRecurrence 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8662-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="d8662-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8662-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8662-105">定期模式和区域。</span><span class="sxs-lookup"><span data-stu-id="d8662-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="d8662-106">属性</span><span class="sxs-lookup"><span data-stu-id="d8662-106">Properties</span></span>
| <span data-ttu-id="d8662-107">属性</span><span class="sxs-lookup"><span data-stu-id="d8662-107">Property</span></span>     | <span data-ttu-id="d8662-108">类型</span><span class="sxs-lookup"><span data-stu-id="d8662-108">Type</span></span>   |<span data-ttu-id="d8662-109">说明</span><span class="sxs-lookup"><span data-stu-id="d8662-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8662-110">模式</span><span class="sxs-lookup"><span data-stu-id="d8662-110">pattern</span></span>|[<span data-ttu-id="d8662-111">recurrencePattern</span><span class="sxs-lookup"><span data-stu-id="d8662-111">recurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="d8662-112">事件发生的频率。</span><span class="sxs-lookup"><span data-stu-id="d8662-112">The frequency of an event.</span></span> <span data-ttu-id="d8662-113">不要指定一次访问评审。</span><span class="sxs-lookup"><span data-stu-id="d8662-113">Do not specify for a one-time access review.</span></span>|
|<span data-ttu-id="d8662-114">range</span><span class="sxs-lookup"><span data-stu-id="d8662-114">range</span></span>|[<span data-ttu-id="d8662-115">recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="d8662-115">recurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="d8662-116">事件的持续时间。</span><span class="sxs-lookup"><span data-stu-id="d8662-116">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8662-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8662-117">JSON representation</span></span>

<span data-ttu-id="d8662-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8662-118">Here is a JSON representation of the resource</span></span>

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


