---
title: toneInfo 资源类型
description: 单个 DTMF 事件。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9cf89df775bb663fbfb4c844b98c6cb35d085aa4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345489"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="81a34-103">toneInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="81a34-103">toneInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81a34-104">单个 DTMF 事件。</span><span class="sxs-lookup"><span data-stu-id="81a34-104">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="81a34-105">属性</span><span class="sxs-lookup"><span data-stu-id="81a34-105">Properties</span></span>

| <span data-ttu-id="81a34-106">属性</span><span class="sxs-lookup"><span data-stu-id="81a34-106">Property</span></span>       | <span data-ttu-id="81a34-107">类型</span><span class="sxs-lookup"><span data-stu-id="81a34-107">Type</span></span>    | <span data-ttu-id="81a34-108">说明</span><span class="sxs-lookup"><span data-stu-id="81a34-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="81a34-109">sequenceId</span><span class="sxs-lookup"><span data-stu-id="81a34-109">sequenceId</span></span> | <span data-ttu-id="81a34-110">Int64</span><span class="sxs-lookup"><span data-stu-id="81a34-110">Int64</span></span> | <span data-ttu-id="81a34-111">用于对 DTMF 事件进行排序的增量标识符。</span><span class="sxs-lookup"><span data-stu-id="81a34-111">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="81a34-112">按键</span><span class="sxs-lookup"><span data-stu-id="81a34-112">tone</span></span> | <span data-ttu-id="81a34-113">String</span><span class="sxs-lookup"><span data-stu-id="81a34-113">String</span></span> | <span data-ttu-id="81a34-114">可能的值是`tone0`: `tone1`、 `tone2`、 `tone3` `tone4` `tone5` `tone6` `tone7` `tone8` `tone9` `flash`、、 `star`、、、、、、、、、、、、。 `pound` `a` `b` `c` `d`</span><span class="sxs-lookup"><span data-stu-id="81a34-114">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="81a34-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81a34-115">JSON representation</span></span>

<span data-ttu-id="81a34-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81a34-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "toneInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
