---
title: metadataEntry 资源类型
description: 给定对象的元数据。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b9dc39021e297882bf92b9a314f342297d86d9ed
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218413"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="344f7-103">metadataEntry 资源类型</span><span class="sxs-lookup"><span data-stu-id="344f7-103">metadataEntry resource type</span></span>

<span data-ttu-id="344f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="344f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="344f7-105">给定对象的元数据。</span><span class="sxs-lookup"><span data-stu-id="344f7-105">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="344f7-106">属性</span><span class="sxs-lookup"><span data-stu-id="344f7-106">Properties</span></span>
| <span data-ttu-id="344f7-107">属性</span><span class="sxs-lookup"><span data-stu-id="344f7-107">Property</span></span>     | <span data-ttu-id="344f7-108">类型</span><span class="sxs-lookup"><span data-stu-id="344f7-108">Type</span></span>   |<span data-ttu-id="344f7-109">说明</span><span class="sxs-lookup"><span data-stu-id="344f7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="344f7-110">Key</span><span class="sxs-lookup"><span data-stu-id="344f7-110">key</span></span>|<span data-ttu-id="344f7-111">字符串</span><span class="sxs-lookup"><span data-stu-id="344f7-111">String</span></span>|<span data-ttu-id="344f7-112">元数据属性的名称。</span><span class="sxs-lookup"><span data-stu-id="344f7-112">Name of the metadata property.</span></span>|
|<span data-ttu-id="344f7-113">value</span><span class="sxs-lookup"><span data-stu-id="344f7-113">value</span></span>|<span data-ttu-id="344f7-114">String</span><span class="sxs-lookup"><span data-stu-id="344f7-114">String</span></span>|<span data-ttu-id="344f7-115">元数据属性的值。</span><span class="sxs-lookup"><span data-stu-id="344f7-115">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="344f7-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="344f7-116">JSON representation</span></span>

<span data-ttu-id="344f7-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="344f7-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataEntry"
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "metadataEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
