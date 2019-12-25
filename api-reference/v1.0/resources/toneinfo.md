---
title: toneInfo 资源类型
description: 单个 DTMF 事件。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a370fe4b6375cecd563c797a21096d02d741e52e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865755"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="cc0e9-103">toneInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc0e9-103">toneInfo resource type</span></span>

<span data-ttu-id="cc0e9-104">单个 DTMF 事件。</span><span class="sxs-lookup"><span data-stu-id="cc0e9-104">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="cc0e9-105">属性</span><span class="sxs-lookup"><span data-stu-id="cc0e9-105">Properties</span></span>

| <span data-ttu-id="cc0e9-106">属性</span><span class="sxs-lookup"><span data-stu-id="cc0e9-106">Property</span></span>       | <span data-ttu-id="cc0e9-107">类型</span><span class="sxs-lookup"><span data-stu-id="cc0e9-107">Type</span></span>    | <span data-ttu-id="cc0e9-108">说明</span><span class="sxs-lookup"><span data-stu-id="cc0e9-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cc0e9-109">sequenceId</span><span class="sxs-lookup"><span data-stu-id="cc0e9-109">sequenceId</span></span> | <span data-ttu-id="cc0e9-110">Int64</span><span class="sxs-lookup"><span data-stu-id="cc0e9-110">Int64</span></span> | <span data-ttu-id="cc0e9-111">用于对 DTMF 事件进行排序的增量标识符。</span><span class="sxs-lookup"><span data-stu-id="cc0e9-111">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="cc0e9-112">按键</span><span class="sxs-lookup"><span data-stu-id="cc0e9-112">tone</span></span> | <span data-ttu-id="cc0e9-113">String</span><span class="sxs-lookup"><span data-stu-id="cc0e9-113">String</span></span> | <span data-ttu-id="cc0e9-114">可能的值为`tone0`： `tone1`、 `tone2`、 `tone3` `tone4` `tone5` `tone6` `tone7` `tone8`、 `tone9`、、、、、 `star`、、`pound`</span><span class="sxs-lookup"><span data-stu-id="cc0e9-114">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cc0e9-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc0e9-115">JSON representation</span></span>

<span data-ttu-id="cc0e9-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc0e9-116">The following is a JSON representation of the resource.</span></span>

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
