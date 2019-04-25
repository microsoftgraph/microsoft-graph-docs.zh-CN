---
title: keyValuePair 资源类型
description: action 参数的项值对。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 86a5415c20721f717947238838341345ec9a4250
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522683"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="57c9b-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="57c9b-103">keyValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57c9b-104">action 参数的项值对。</span><span class="sxs-lookup"><span data-stu-id="57c9b-104">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="57c9b-105">属性</span><span class="sxs-lookup"><span data-stu-id="57c9b-105">Properties</span></span>

| <span data-ttu-id="57c9b-106">属性</span><span class="sxs-lookup"><span data-stu-id="57c9b-106">Property</span></span>     | <span data-ttu-id="57c9b-107">类型</span><span class="sxs-lookup"><span data-stu-id="57c9b-107">Type</span></span>        | <span data-ttu-id="57c9b-108">说明</span><span class="sxs-lookup"><span data-stu-id="57c9b-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="57c9b-109">name</span><span class="sxs-lookup"><span data-stu-id="57c9b-109">name</span></span>|<span data-ttu-id="57c9b-110">String</span><span class="sxs-lookup"><span data-stu-id="57c9b-110">String</span></span>|<span data-ttu-id="57c9b-111">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="57c9b-111">Name for this key-value pair</span></span>|
|<span data-ttu-id="57c9b-112">value</span><span class="sxs-lookup"><span data-stu-id="57c9b-112">value</span></span>|<span data-ttu-id="57c9b-113">String</span><span class="sxs-lookup"><span data-stu-id="57c9b-113">String</span></span>|<span data-ttu-id="57c9b-114">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="57c9b-114">Value for this key-value pair</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57c9b-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57c9b-115">JSON representation</span></span>

<span data-ttu-id="57c9b-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57c9b-116">The following is a JSON representation of the resource.</span></span>

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