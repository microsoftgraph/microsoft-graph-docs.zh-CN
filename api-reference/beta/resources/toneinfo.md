---
title: toneInfo 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: b4ed9667c2e2156f52703c6fa15f4937ead5cef4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048771"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="43560-103">toneInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="43560-103">toneInfo resource type</span></span>

> <span data-ttu-id="43560-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="43560-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43560-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="43560-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="43560-106">属性</span><span class="sxs-lookup"><span data-stu-id="43560-106">Properties</span></span>

| <span data-ttu-id="43560-107">属性</span><span class="sxs-lookup"><span data-stu-id="43560-107">Property</span></span>       | <span data-ttu-id="43560-108">类型</span><span class="sxs-lookup"><span data-stu-id="43560-108">Type</span></span>    | <span data-ttu-id="43560-109">说明</span><span class="sxs-lookup"><span data-stu-id="43560-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="43560-110">sequenceId</span><span class="sxs-lookup"><span data-stu-id="43560-110">sequenceId</span></span> | <span data-ttu-id="43560-111">Int64</span><span class="sxs-lookup"><span data-stu-id="43560-111">Int64</span></span> | <span data-ttu-id="43560-112">用于排序 DTMF 事件增量标识符。</span><span class="sxs-lookup"><span data-stu-id="43560-112">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="43560-113">音</span><span class="sxs-lookup"><span data-stu-id="43560-113">tone</span></span> | <span data-ttu-id="43560-114">字符串</span><span class="sxs-lookup"><span data-stu-id="43560-114">String</span></span> | <span data-ttu-id="43560-115">可能的值为： `tone0`， `tone1`， `tone2`， `tone3`， `tone4`， `tone5`， `tone6`， `tone7`， `tone8`， `tone9`， `star`， `pound`， `a`， `b`， `c`， `d`， `flash`。</span><span class="sxs-lookup"><span data-stu-id="43560-115">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="43560-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43560-116">JSON representation</span></span>

<span data-ttu-id="43560-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43560-117">The following is a JSON representation of the resource.</span></span>

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