---
title: toneInfo 资源类型
description: 单个 DTMF 事件。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 479697ea847f3a943e1d9bb7de19c422d15b47c6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916969"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="2cc70-103">toneInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="2cc70-103">toneInfo resource type</span></span>

> <span data-ttu-id="2cc70-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2cc70-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2cc70-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2cc70-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2cc70-106">单个 DTMF 事件。</span><span class="sxs-lookup"><span data-stu-id="2cc70-106">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="2cc70-107">属性</span><span class="sxs-lookup"><span data-stu-id="2cc70-107">Properties</span></span>

| <span data-ttu-id="2cc70-108">属性</span><span class="sxs-lookup"><span data-stu-id="2cc70-108">Property</span></span>       | <span data-ttu-id="2cc70-109">类型</span><span class="sxs-lookup"><span data-stu-id="2cc70-109">Type</span></span>    | <span data-ttu-id="2cc70-110">说明</span><span class="sxs-lookup"><span data-stu-id="2cc70-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2cc70-111">sequenceId</span><span class="sxs-lookup"><span data-stu-id="2cc70-111">sequenceId</span></span> | <span data-ttu-id="2cc70-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2cc70-112">Int64</span></span> | <span data-ttu-id="2cc70-113">用于排序 DTMF 事件增量标识符。</span><span class="sxs-lookup"><span data-stu-id="2cc70-113">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="2cc70-114">音</span><span class="sxs-lookup"><span data-stu-id="2cc70-114">tone</span></span> | <span data-ttu-id="2cc70-115">字符串</span><span class="sxs-lookup"><span data-stu-id="2cc70-115">String</span></span> | <span data-ttu-id="2cc70-116">可能的值为： `tone0`， `tone1`， `tone2`， `tone3`， `tone4`， `tone5`， `tone6`， `tone7`， `tone8`， `tone9`， `star`， `pound`， `a`， `b`， `c`， `d`， `flash`。</span><span class="sxs-lookup"><span data-stu-id="2cc70-116">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2cc70-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2cc70-117">JSON representation</span></span>

<span data-ttu-id="2cc70-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2cc70-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.toneInfo"
}-->
```json
{
  "sequenceId": 1024,
  "tone": "tone0 | tone1 | tone2 | tone3 | tone4 | tone5 | tone6 | tone7 | tone8 | tone9 | star | pound | a | b | c | d | flash"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "toneInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
