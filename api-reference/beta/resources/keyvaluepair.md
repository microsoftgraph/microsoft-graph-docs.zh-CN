---
title: keyValuePair 资源类型
description: Action 参数的项值对。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2417ada5a3fa3937d6560f62a47c99f6b47d44e0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523014"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="224c2-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="224c2-103">keyValuePair resource type</span></span>

<span data-ttu-id="224c2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="224c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="224c2-105">Action 参数的项值对。</span><span class="sxs-lookup"><span data-stu-id="224c2-105">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="224c2-106">属性</span><span class="sxs-lookup"><span data-stu-id="224c2-106">Properties</span></span>

| <span data-ttu-id="224c2-107">属性</span><span class="sxs-lookup"><span data-stu-id="224c2-107">Property</span></span>     | <span data-ttu-id="224c2-108">类型</span><span class="sxs-lookup"><span data-stu-id="224c2-108">Type</span></span>        | <span data-ttu-id="224c2-109">说明</span><span class="sxs-lookup"><span data-stu-id="224c2-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="224c2-110">name</span><span class="sxs-lookup"><span data-stu-id="224c2-110">name</span></span>|<span data-ttu-id="224c2-111">String</span><span class="sxs-lookup"><span data-stu-id="224c2-111">String</span></span>|<span data-ttu-id="224c2-112">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="224c2-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="224c2-113">value</span><span class="sxs-lookup"><span data-stu-id="224c2-113">value</span></span>|<span data-ttu-id="224c2-114">String</span><span class="sxs-lookup"><span data-stu-id="224c2-114">String</span></span>|<span data-ttu-id="224c2-115">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="224c2-115">Value for this key-value pair</span></span>|

## <a name="json-representation"></a><span data-ttu-id="224c2-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="224c2-116">JSON representation</span></span>

<span data-ttu-id="224c2-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="224c2-117">The following is a JSON representation of the resource.</span></span>

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