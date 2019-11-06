---
title: toneInfo 资源类型
description: 单个 DTMF 事件。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: aa0ef52126895e61300c1e2f7a258926e209866c
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006520"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="64ec5-103">toneInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="64ec5-103">toneInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64ec5-104">单个 DTMF 事件。</span><span class="sxs-lookup"><span data-stu-id="64ec5-104">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="64ec5-105">属性</span><span class="sxs-lookup"><span data-stu-id="64ec5-105">Properties</span></span>

| <span data-ttu-id="64ec5-106">属性</span><span class="sxs-lookup"><span data-stu-id="64ec5-106">Property</span></span>       | <span data-ttu-id="64ec5-107">类型</span><span class="sxs-lookup"><span data-stu-id="64ec5-107">Type</span></span>    | <span data-ttu-id="64ec5-108">说明</span><span class="sxs-lookup"><span data-stu-id="64ec5-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="64ec5-109">sequenceId</span><span class="sxs-lookup"><span data-stu-id="64ec5-109">sequenceId</span></span> | <span data-ttu-id="64ec5-110">Int64</span><span class="sxs-lookup"><span data-stu-id="64ec5-110">Int64</span></span> | <span data-ttu-id="64ec5-111">用于对 DTMF 事件进行排序的增量标识符。</span><span class="sxs-lookup"><span data-stu-id="64ec5-111">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="64ec5-112">按键</span><span class="sxs-lookup"><span data-stu-id="64ec5-112">tone</span></span> | <span data-ttu-id="64ec5-113">String</span><span class="sxs-lookup"><span data-stu-id="64ec5-113">String</span></span> | <span data-ttu-id="64ec5-114">可能的值是`tone0`： `tone1`、 `tone2`、 `tone3` `tone4` `tone5` `tone6` `tone7` `tone8` `tone9` `flash`、、 `star`、、、、、、、、、、、、。 `pound` `a` `b` `c` `d`</span><span class="sxs-lookup"><span data-stu-id="64ec5-114">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="64ec5-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64ec5-115">JSON representation</span></span>

<span data-ttu-id="64ec5-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64ec5-116">The following is a JSON representation of the resource.</span></span>

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
