---
title: metadataEntry 资源类型
description: 给定对象的元数据。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 9d10c6fd30d161e886ea782ca3564f550352a5f6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131864"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="f214a-103">metadataEntry 资源类型</span><span class="sxs-lookup"><span data-stu-id="f214a-103">metadataEntry resource type</span></span>

<span data-ttu-id="f214a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f214a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f214a-105">给定对象的元数据。</span><span class="sxs-lookup"><span data-stu-id="f214a-105">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="f214a-106">属性</span><span class="sxs-lookup"><span data-stu-id="f214a-106">Properties</span></span>
| <span data-ttu-id="f214a-107">属性</span><span class="sxs-lookup"><span data-stu-id="f214a-107">Property</span></span>     | <span data-ttu-id="f214a-108">类型</span><span class="sxs-lookup"><span data-stu-id="f214a-108">Type</span></span>   |<span data-ttu-id="f214a-109">说明</span><span class="sxs-lookup"><span data-stu-id="f214a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f214a-110">Key</span><span class="sxs-lookup"><span data-stu-id="f214a-110">key</span></span>|<span data-ttu-id="f214a-111">字符串</span><span class="sxs-lookup"><span data-stu-id="f214a-111">String</span></span>|<span data-ttu-id="f214a-112">元数据属性的名称。</span><span class="sxs-lookup"><span data-stu-id="f214a-112">Name of the metadata property.</span></span>|
|<span data-ttu-id="f214a-113">value</span><span class="sxs-lookup"><span data-stu-id="f214a-113">value</span></span>|<span data-ttu-id="f214a-114">String</span><span class="sxs-lookup"><span data-stu-id="f214a-114">String</span></span>|<span data-ttu-id="f214a-115">元数据属性的值。</span><span class="sxs-lookup"><span data-stu-id="f214a-115">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f214a-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f214a-116">JSON representation</span></span>

<span data-ttu-id="f214a-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f214a-117">The following is a JSON representation of the resource.</span></span>

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


