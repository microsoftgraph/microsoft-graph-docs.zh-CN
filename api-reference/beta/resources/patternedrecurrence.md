---
title: patternedRecurrence 资源类型
description: 定期模式和区域。
localization_priority: Normal
ms.openlocfilehash: 2c2d68046c69ed702738318121a0289eb6a347a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825242"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="a6b4f-103">patternedRecurrence 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6b4f-103">patternedRecurrence resource type</span></span>

> <span data-ttu-id="a6b4f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a6b4f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6b4f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a6b4f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6b4f-106">定期模式和区域。</span><span class="sxs-lookup"><span data-stu-id="a6b4f-106">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="a6b4f-107">属性</span><span class="sxs-lookup"><span data-stu-id="a6b4f-107">Properties</span></span>
| <span data-ttu-id="a6b4f-108">属性</span><span class="sxs-lookup"><span data-stu-id="a6b4f-108">Property</span></span>     | <span data-ttu-id="a6b4f-109">类型</span><span class="sxs-lookup"><span data-stu-id="a6b4f-109">Type</span></span>   |<span data-ttu-id="a6b4f-110">说明</span><span class="sxs-lookup"><span data-stu-id="a6b4f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6b4f-111">模式</span><span class="sxs-lookup"><span data-stu-id="a6b4f-111">pattern</span></span>|[<span data-ttu-id="a6b4f-112">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="a6b4f-112">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="a6b4f-113">事件发生的频率。</span><span class="sxs-lookup"><span data-stu-id="a6b4f-113">The frequency of an event.</span></span>|
|<span data-ttu-id="a6b4f-114">区域</span><span class="sxs-lookup"><span data-stu-id="a6b4f-114">range</span></span>|[<span data-ttu-id="a6b4f-115">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="a6b4f-115">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="a6b4f-116">事件的持续时间。</span><span class="sxs-lookup"><span data-stu-id="a6b4f-116">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6b4f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6b4f-117">JSON representation</span></span>

<span data-ttu-id="a6b4f-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6b4f-118">Here is a JSON representation of the resource</span></span>

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
