---
title: stringKeyAttributeMappingSourceValuePair 资源类型
description: 表示键值对，其中键是字符串，值为 attributeMappingSource。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d70337be1a3f28e9ba30734ccc919c5459dcbd0b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026192"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="e2d1f-103">stringKeyAttributeMappingSourceValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2d1f-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

<span data-ttu-id="e2d1f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2d1f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2d1f-105">表示键值对，其中键是字符串，值为 [attributeMappingSource](synchronization-attributemappingsource.md)。</span><span class="sxs-lookup"><span data-stu-id="e2d1f-105">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e2d1f-106">属性</span><span class="sxs-lookup"><span data-stu-id="e2d1f-106">Properties</span></span>
| <span data-ttu-id="e2d1f-107">属性</span><span class="sxs-lookup"><span data-stu-id="e2d1f-107">Property</span></span>     | <span data-ttu-id="e2d1f-108">类型</span><span class="sxs-lookup"><span data-stu-id="e2d1f-108">Type</span></span>   |<span data-ttu-id="e2d1f-109">说明</span><span class="sxs-lookup"><span data-stu-id="e2d1f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2d1f-110">Key</span><span class="sxs-lookup"><span data-stu-id="e2d1f-110">key</span></span>|<span data-ttu-id="e2d1f-111">String</span><span class="sxs-lookup"><span data-stu-id="e2d1f-111">String</span></span>|<span data-ttu-id="e2d1f-112">参数的名称。</span><span class="sxs-lookup"><span data-stu-id="e2d1f-112">The name of the parameter.</span></span>|
|<span data-ttu-id="e2d1f-113">值</span><span class="sxs-lookup"><span data-stu-id="e2d1f-113">value</span></span>|[<span data-ttu-id="e2d1f-114">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="e2d1f-114">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="e2d1f-115">参数的值。</span><span class="sxs-lookup"><span data-stu-id="e2d1f-115">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2d1f-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2d1f-116">JSON representation</span></span>

<span data-ttu-id="e2d1f-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2d1f-117">The following is a JSON representation of the resource.</span></span>

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


