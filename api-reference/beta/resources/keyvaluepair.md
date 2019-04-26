---
title: keyValuePair 资源类型
description: action 参数的项值对。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 86a5415c20721f717947238838341345ec9a4250
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345319"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="dc98f-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc98f-103">keyValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc98f-104">action 参数的项值对。</span><span class="sxs-lookup"><span data-stu-id="dc98f-104">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="dc98f-105">属性</span><span class="sxs-lookup"><span data-stu-id="dc98f-105">Properties</span></span>

| <span data-ttu-id="dc98f-106">属性</span><span class="sxs-lookup"><span data-stu-id="dc98f-106">Property</span></span>     | <span data-ttu-id="dc98f-107">类型</span><span class="sxs-lookup"><span data-stu-id="dc98f-107">Type</span></span>        | <span data-ttu-id="dc98f-108">说明</span><span class="sxs-lookup"><span data-stu-id="dc98f-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dc98f-109">name</span><span class="sxs-lookup"><span data-stu-id="dc98f-109">name</span></span>|<span data-ttu-id="dc98f-110">String</span><span class="sxs-lookup"><span data-stu-id="dc98f-110">String</span></span>|<span data-ttu-id="dc98f-111">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="dc98f-111">Name for this key-value pair</span></span>|
|<span data-ttu-id="dc98f-112">value</span><span class="sxs-lookup"><span data-stu-id="dc98f-112">value</span></span>|<span data-ttu-id="dc98f-113">String</span><span class="sxs-lookup"><span data-stu-id="dc98f-113">String</span></span>|<span data-ttu-id="dc98f-114">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="dc98f-114">Value for this key-value pair</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc98f-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc98f-115">JSON representation</span></span>

<span data-ttu-id="dc98f-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc98f-116">The following is a JSON representation of the resource.</span></span>

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