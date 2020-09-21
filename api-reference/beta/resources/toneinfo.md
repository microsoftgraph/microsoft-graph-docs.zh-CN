---
title: toneInfo 资源类型
description: 单个 DTMF 事件。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5555ae61920751d63a70fdb86199ffa572dcb9be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083945"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="6bffd-103">toneInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="6bffd-103">toneInfo resource type</span></span>

<span data-ttu-id="6bffd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bffd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bffd-105">单个 DTMF 事件。</span><span class="sxs-lookup"><span data-stu-id="6bffd-105">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="6bffd-106">属性</span><span class="sxs-lookup"><span data-stu-id="6bffd-106">Properties</span></span>

| <span data-ttu-id="6bffd-107">属性</span><span class="sxs-lookup"><span data-stu-id="6bffd-107">Property</span></span>       | <span data-ttu-id="6bffd-108">类型</span><span class="sxs-lookup"><span data-stu-id="6bffd-108">Type</span></span>    | <span data-ttu-id="6bffd-109">说明</span><span class="sxs-lookup"><span data-stu-id="6bffd-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6bffd-110">sequenceId</span><span class="sxs-lookup"><span data-stu-id="6bffd-110">sequenceId</span></span> | <span data-ttu-id="6bffd-111">Int64</span><span class="sxs-lookup"><span data-stu-id="6bffd-111">Int64</span></span> | <span data-ttu-id="6bffd-112">用于对 DTMF 事件进行排序的增量标识符。</span><span class="sxs-lookup"><span data-stu-id="6bffd-112">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="6bffd-113">按键</span><span class="sxs-lookup"><span data-stu-id="6bffd-113">tone</span></span> | <span data-ttu-id="6bffd-114">字符串</span><span class="sxs-lookup"><span data-stu-id="6bffd-114">String</span></span> | <span data-ttu-id="6bffd-115">可能的值是：、、、、、、、、、、、、、、、、 `tone0` `tone1` `tone2` `tone3` `tone4` `tone5` `tone6` `tone7` `tone8` `tone9` `star` `pound` `a` `b` `c` `d` `flash` 。</span><span class="sxs-lookup"><span data-stu-id="6bffd-115">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6bffd-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6bffd-116">JSON representation</span></span>

<span data-ttu-id="6bffd-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6bffd-117">The following is a JSON representation of the resource.</span></span>

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


