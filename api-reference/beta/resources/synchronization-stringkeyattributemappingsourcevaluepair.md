---
title: stringKeyAttributeMappingSourceValuePair 资源类型
description: 表示键值对, 其中键是字符串, 值为 attributeMappingSource。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dab0376441904f7ec935aa87da3b825d2a0e197d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007877"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="e07b3-103">stringKeyAttributeMappingSourceValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="e07b3-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e07b3-104">表示键值对, 其中键是字符串, 值为[attributeMappingSource](synchronization-attributemappingsource.md)。</span><span class="sxs-lookup"><span data-stu-id="e07b3-104">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e07b3-105">属性</span><span class="sxs-lookup"><span data-stu-id="e07b3-105">Properties</span></span>
| <span data-ttu-id="e07b3-106">属性</span><span class="sxs-lookup"><span data-stu-id="e07b3-106">Property</span></span>     | <span data-ttu-id="e07b3-107">类型</span><span class="sxs-lookup"><span data-stu-id="e07b3-107">Type</span></span>   |<span data-ttu-id="e07b3-108">说明</span><span class="sxs-lookup"><span data-stu-id="e07b3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e07b3-109">Key</span><span class="sxs-lookup"><span data-stu-id="e07b3-109">key</span></span>|<span data-ttu-id="e07b3-110">String</span><span class="sxs-lookup"><span data-stu-id="e07b3-110">String</span></span>|<span data-ttu-id="e07b3-111">参数的名称。</span><span class="sxs-lookup"><span data-stu-id="e07b3-111">The name of the parameter.</span></span>|
|<span data-ttu-id="e07b3-112">值</span><span class="sxs-lookup"><span data-stu-id="e07b3-112">value</span></span>|[<span data-ttu-id="e07b3-113">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="e07b3-113">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="e07b3-114">参数的值。</span><span class="sxs-lookup"><span data-stu-id="e07b3-114">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e07b3-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e07b3-115">JSON representation</span></span>

<span data-ttu-id="e07b3-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e07b3-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
