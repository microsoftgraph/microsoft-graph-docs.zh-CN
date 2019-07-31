---
title: metadataEntry 资源类型
description: 给定对象的元数据。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 55b686bc04ccf869ddf9d6dc6029c6206f7b2274
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964826"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="2f553-103">metadataEntry 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f553-103">metadataEntry resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f553-104">给定对象的元数据。</span><span class="sxs-lookup"><span data-stu-id="2f553-104">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="2f553-105">属性</span><span class="sxs-lookup"><span data-stu-id="2f553-105">Properties</span></span>
| <span data-ttu-id="2f553-106">属性</span><span class="sxs-lookup"><span data-stu-id="2f553-106">Property</span></span>     | <span data-ttu-id="2f553-107">类型</span><span class="sxs-lookup"><span data-stu-id="2f553-107">Type</span></span>   |<span data-ttu-id="2f553-108">说明</span><span class="sxs-lookup"><span data-stu-id="2f553-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f553-109">Key</span><span class="sxs-lookup"><span data-stu-id="2f553-109">key</span></span>|<span data-ttu-id="2f553-110">String</span><span class="sxs-lookup"><span data-stu-id="2f553-110">String</span></span>|<span data-ttu-id="2f553-111">元数据属性的名称。</span><span class="sxs-lookup"><span data-stu-id="2f553-111">Name of the metadata property.</span></span>|
|<span data-ttu-id="2f553-112">value</span><span class="sxs-lookup"><span data-stu-id="2f553-112">value</span></span>|<span data-ttu-id="2f553-113">String</span><span class="sxs-lookup"><span data-stu-id="2f553-113">String</span></span>|<span data-ttu-id="2f553-114">元数据属性的值。</span><span class="sxs-lookup"><span data-stu-id="2f553-114">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f553-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f553-115">JSON representation</span></span>

<span data-ttu-id="2f553-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f553-116">The following is a JSON representation of the resource.</span></span>

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
