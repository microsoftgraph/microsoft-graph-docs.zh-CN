---
title: stringKeyLongValuePair 资源类型
description: 表示键值对, 其中键是字符串, 值为 Int64。
localization_priority: Normal
ms.openlocfilehash: 97ca9f4f7b4079311a1ce6996fde0472c527e7f9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524538"
---
# <a name="stringkeylongvaluepair-resource-type"></a><span data-ttu-id="763d8-103">stringKeyLongValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="763d8-103">stringKeyLongValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="763d8-104">表示键值对, 其中键是字符串, 值为 Int64。</span><span class="sxs-lookup"><span data-stu-id="763d8-104">Represents a key-value pair where the key is a string and the value is an Int64.</span></span>

## <a name="properties"></a><span data-ttu-id="763d8-105">属性</span><span class="sxs-lookup"><span data-stu-id="763d8-105">Properties</span></span>
| <span data-ttu-id="763d8-106">属性</span><span class="sxs-lookup"><span data-stu-id="763d8-106">Property</span></span>     | <span data-ttu-id="763d8-107">类型</span><span class="sxs-lookup"><span data-stu-id="763d8-107">Type</span></span>   |<span data-ttu-id="763d8-108">说明</span><span class="sxs-lookup"><span data-stu-id="763d8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="763d8-109">Key</span><span class="sxs-lookup"><span data-stu-id="763d8-109">key</span></span>|<span data-ttu-id="763d8-110">String</span><span class="sxs-lookup"><span data-stu-id="763d8-110">String</span></span>|<span data-ttu-id="763d8-111">键。</span><span class="sxs-lookup"><span data-stu-id="763d8-111">Key.</span></span>|
|<span data-ttu-id="763d8-112">值</span><span class="sxs-lookup"><span data-stu-id="763d8-112">value</span></span>|<span data-ttu-id="763d8-113">Int64</span><span class="sxs-lookup"><span data-stu-id="763d8-113">Int64</span></span>|<span data-ttu-id="763d8-114">值。</span><span class="sxs-lookup"><span data-stu-id="763d8-114">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="763d8-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="763d8-115">JSON representation</span></span>

<span data-ttu-id="763d8-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="763d8-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyLongValuePair"
}-->

```json
{
  "key": "String",
  "value": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyLongValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeylongvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
