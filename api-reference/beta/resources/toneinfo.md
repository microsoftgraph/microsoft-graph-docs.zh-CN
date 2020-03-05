---
title: toneInfo 资源类型
description: 单个 DTMF 事件。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 99889abd2d3d9272f4f0ecb9b4d1b5321029beea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519657"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="f0ee7-103">toneInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0ee7-103">toneInfo resource type</span></span>

<span data-ttu-id="f0ee7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f0ee7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0ee7-105">单个 DTMF 事件。</span><span class="sxs-lookup"><span data-stu-id="f0ee7-105">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="f0ee7-106">属性</span><span class="sxs-lookup"><span data-stu-id="f0ee7-106">Properties</span></span>

| <span data-ttu-id="f0ee7-107">属性</span><span class="sxs-lookup"><span data-stu-id="f0ee7-107">Property</span></span>       | <span data-ttu-id="f0ee7-108">类型</span><span class="sxs-lookup"><span data-stu-id="f0ee7-108">Type</span></span>    | <span data-ttu-id="f0ee7-109">说明</span><span class="sxs-lookup"><span data-stu-id="f0ee7-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f0ee7-110">sequenceId</span><span class="sxs-lookup"><span data-stu-id="f0ee7-110">sequenceId</span></span> | <span data-ttu-id="f0ee7-111">Int64</span><span class="sxs-lookup"><span data-stu-id="f0ee7-111">Int64</span></span> | <span data-ttu-id="f0ee7-112">用于对 DTMF 事件进行排序的增量标识符。</span><span class="sxs-lookup"><span data-stu-id="f0ee7-112">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="f0ee7-113">按键</span><span class="sxs-lookup"><span data-stu-id="f0ee7-113">tone</span></span> | <span data-ttu-id="f0ee7-114">String</span><span class="sxs-lookup"><span data-stu-id="f0ee7-114">String</span></span> | <span data-ttu-id="f0ee7-115">可能的值是`tone0`： `tone1`、 `tone2`、 `tone3` `tone4` `tone5` `tone6` `tone7` `tone8` `tone9` `flash`、、 `star`、、、、、、、、、、、、。 `pound` `a` `b` `c` `d`</span><span class="sxs-lookup"><span data-stu-id="f0ee7-115">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f0ee7-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0ee7-116">JSON representation</span></span>

<span data-ttu-id="f0ee7-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0ee7-117">The following is a JSON representation of the resource.</span></span>

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
