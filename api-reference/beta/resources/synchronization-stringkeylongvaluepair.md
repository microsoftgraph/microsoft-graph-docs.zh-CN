---
title: stringKeyLongValuePair 资源类型
description: 表示键值对, 其中键是字符串, 值为 Int64。
localization_priority: Normal
ms.openlocfilehash: 48ca44c70e02be153aaeb5ee1171cd8c60e0fa2d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342748"
---
# <a name="stringkeylongvaluepair-resource-type"></a><span data-ttu-id="0307b-103">stringKeyLongValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="0307b-103">stringKeyLongValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0307b-104">表示键值对, 其中键是字符串, 值为 Int64。</span><span class="sxs-lookup"><span data-stu-id="0307b-104">Represents a key-value pair where the key is a string and the value is an Int64.</span></span>

## <a name="properties"></a><span data-ttu-id="0307b-105">属性</span><span class="sxs-lookup"><span data-stu-id="0307b-105">Properties</span></span>
| <span data-ttu-id="0307b-106">属性</span><span class="sxs-lookup"><span data-stu-id="0307b-106">Property</span></span>     | <span data-ttu-id="0307b-107">类型</span><span class="sxs-lookup"><span data-stu-id="0307b-107">Type</span></span>   |<span data-ttu-id="0307b-108">说明</span><span class="sxs-lookup"><span data-stu-id="0307b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0307b-109">Key</span><span class="sxs-lookup"><span data-stu-id="0307b-109">key</span></span>|<span data-ttu-id="0307b-110">String</span><span class="sxs-lookup"><span data-stu-id="0307b-110">String</span></span>|<span data-ttu-id="0307b-111">键。</span><span class="sxs-lookup"><span data-stu-id="0307b-111">Key.</span></span>|
|<span data-ttu-id="0307b-112">值</span><span class="sxs-lookup"><span data-stu-id="0307b-112">value</span></span>|<span data-ttu-id="0307b-113">Int64</span><span class="sxs-lookup"><span data-stu-id="0307b-113">Int64</span></span>|<span data-ttu-id="0307b-114">值。</span><span class="sxs-lookup"><span data-stu-id="0307b-114">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0307b-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0307b-115">JSON representation</span></span>

<span data-ttu-id="0307b-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0307b-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
