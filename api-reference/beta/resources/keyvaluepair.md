---
title: keyValuePair 资源类型
description: Action 参数的项值对。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: db8d3b14ceaa0ff05181894af803b8b6feea77c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967033"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="a91e1-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="a91e1-103">keyValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a91e1-104">Action 参数的项值对。</span><span class="sxs-lookup"><span data-stu-id="a91e1-104">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="a91e1-105">属性</span><span class="sxs-lookup"><span data-stu-id="a91e1-105">Properties</span></span>

| <span data-ttu-id="a91e1-106">属性</span><span class="sxs-lookup"><span data-stu-id="a91e1-106">Property</span></span>     | <span data-ttu-id="a91e1-107">类型</span><span class="sxs-lookup"><span data-stu-id="a91e1-107">Type</span></span>        | <span data-ttu-id="a91e1-108">说明</span><span class="sxs-lookup"><span data-stu-id="a91e1-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a91e1-109">name</span><span class="sxs-lookup"><span data-stu-id="a91e1-109">name</span></span>|<span data-ttu-id="a91e1-110">String</span><span class="sxs-lookup"><span data-stu-id="a91e1-110">String</span></span>|<span data-ttu-id="a91e1-111">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="a91e1-111">Name for this key-value pair</span></span>|
|<span data-ttu-id="a91e1-112">value</span><span class="sxs-lookup"><span data-stu-id="a91e1-112">value</span></span>|<span data-ttu-id="a91e1-113">String</span><span class="sxs-lookup"><span data-stu-id="a91e1-113">String</span></span>|<span data-ttu-id="a91e1-114">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="a91e1-114">Value for this key-value pair</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a91e1-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a91e1-115">JSON representation</span></span>

<span data-ttu-id="a91e1-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a91e1-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValuePair",
  "baseType": null
}-->

```json
{
  "name": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->