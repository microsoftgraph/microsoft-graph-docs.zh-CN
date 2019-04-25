---
title: toneInfo 资源类型
description: 单个 DTMF 事件。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f58548f8f075494c6601db2962d88fb6cabb59ce
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522648"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="4ecb1-103">toneInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ecb1-103">toneInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ecb1-104">单个 DTMF 事件。</span><span class="sxs-lookup"><span data-stu-id="4ecb1-104">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="4ecb1-105">属性</span><span class="sxs-lookup"><span data-stu-id="4ecb1-105">Properties</span></span>

| <span data-ttu-id="4ecb1-106">属性</span><span class="sxs-lookup"><span data-stu-id="4ecb1-106">Property</span></span>       | <span data-ttu-id="4ecb1-107">类型</span><span class="sxs-lookup"><span data-stu-id="4ecb1-107">Type</span></span>    | <span data-ttu-id="4ecb1-108">说明</span><span class="sxs-lookup"><span data-stu-id="4ecb1-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4ecb1-109">sequenceId</span><span class="sxs-lookup"><span data-stu-id="4ecb1-109">sequenceId</span></span> | <span data-ttu-id="4ecb1-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4ecb1-110">Int64</span></span> | <span data-ttu-id="4ecb1-111">用于对 DTMF 事件进行排序的增量标识符。</span><span class="sxs-lookup"><span data-stu-id="4ecb1-111">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="4ecb1-112">按键</span><span class="sxs-lookup"><span data-stu-id="4ecb1-112">tone</span></span> | <span data-ttu-id="4ecb1-113">String</span><span class="sxs-lookup"><span data-stu-id="4ecb1-113">String</span></span> | <span data-ttu-id="4ecb1-114">可能的值是`tone0`: `tone1`、 `tone2`、 `tone3` `tone4` `tone5` `tone6` `tone7` `tone8` `tone9` `flash`、、 `star`、、、、、、、、、、、、。 `pound` `a` `b` `c` `d`</span><span class="sxs-lookup"><span data-stu-id="4ecb1-114">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4ecb1-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ecb1-115">JSON representation</span></span>

<span data-ttu-id="4ecb1-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ecb1-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/toneinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
