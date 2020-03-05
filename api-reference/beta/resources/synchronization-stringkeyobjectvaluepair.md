---
title: stringKeyObjectValuePair 资源类型
description: 表示键值对，其中键是字符串，值是任意的 JSON 对象。 这是一种 OData 开放类型，它应具有一个名`value`为的属性，它是一个有效的 JSON 对象。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c3a86cd4963f8d17fbe9f4c5371e98070f8f8f4e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520091"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="a4927-104">stringKeyObjectValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4927-104">stringKeyObjectValuePair resource type</span></span>

<span data-ttu-id="a4927-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a4927-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4927-106">表示键值对，其中键是字符串，值是任意的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a4927-106">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="a4927-107">这是一种 OData 开放类型，它应具有一个名`value`为的属性，它是一个有效的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a4927-107">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="a4927-108">属性</span><span class="sxs-lookup"><span data-stu-id="a4927-108">Properties</span></span>
| <span data-ttu-id="a4927-109">属性</span><span class="sxs-lookup"><span data-stu-id="a4927-109">Property</span></span>     | <span data-ttu-id="a4927-110">类型</span><span class="sxs-lookup"><span data-stu-id="a4927-110">Type</span></span>   |<span data-ttu-id="a4927-111">说明</span><span class="sxs-lookup"><span data-stu-id="a4927-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4927-112">Key</span><span class="sxs-lookup"><span data-stu-id="a4927-112">key</span></span>|<span data-ttu-id="a4927-113">String</span><span class="sxs-lookup"><span data-stu-id="a4927-113">String</span></span>|<span data-ttu-id="a4927-114">键。</span><span class="sxs-lookup"><span data-stu-id="a4927-114">Key.</span></span>|
|<span data-ttu-id="a4927-115">值</span><span class="sxs-lookup"><span data-stu-id="a4927-115">value</span></span>|<span data-ttu-id="a4927-116">Json</span><span class="sxs-lookup"><span data-stu-id="a4927-116">Json</span></span>|<span data-ttu-id="a4927-117">任意 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a4927-117">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4927-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4927-118">JSON representation</span></span>

<span data-ttu-id="a4927-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4927-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
