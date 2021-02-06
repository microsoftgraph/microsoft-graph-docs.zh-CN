---
title: stringKeyAttributeMappingSourceValuePair 资源类型
description: 表示键值对，其中键是字符串，值为 attributeMappingSource。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d0bd761b64c41c930bda84b820d98501870e0c26
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135092"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="4d777-103">stringKeyAttributeMappingSourceValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d777-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

<span data-ttu-id="4d777-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d777-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d777-105">表示键值对，其中键是字符串，值为 [attributeMappingSource](synchronization-attributemappingsource.md)。</span><span class="sxs-lookup"><span data-stu-id="4d777-105">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4d777-106">属性</span><span class="sxs-lookup"><span data-stu-id="4d777-106">Properties</span></span>
| <span data-ttu-id="4d777-107">属性</span><span class="sxs-lookup"><span data-stu-id="4d777-107">Property</span></span>     | <span data-ttu-id="4d777-108">类型</span><span class="sxs-lookup"><span data-stu-id="4d777-108">Type</span></span>   |<span data-ttu-id="4d777-109">说明</span><span class="sxs-lookup"><span data-stu-id="4d777-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d777-110">Key</span><span class="sxs-lookup"><span data-stu-id="4d777-110">key</span></span>|<span data-ttu-id="4d777-111">字符串</span><span class="sxs-lookup"><span data-stu-id="4d777-111">String</span></span>|<span data-ttu-id="4d777-112">参数的名称。</span><span class="sxs-lookup"><span data-stu-id="4d777-112">The name of the parameter.</span></span>|
|<span data-ttu-id="4d777-113">值</span><span class="sxs-lookup"><span data-stu-id="4d777-113">value</span></span>|[<span data-ttu-id="4d777-114">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="4d777-114">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="4d777-115">参数的值。</span><span class="sxs-lookup"><span data-stu-id="4d777-115">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d777-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d777-116">JSON representation</span></span>

<span data-ttu-id="4d777-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d777-117">The following is a JSON representation of the resource.</span></span>

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


