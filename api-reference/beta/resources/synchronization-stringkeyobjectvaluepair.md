---
title: stringKeyObjectValuePair 资源类型
description: 表示键值对，其中键是字符串，值是任意的 JSON 对象。 这是一种 OData 开放类型，它应具有一个名`value`为的属性，它是一个有效的 JSON 对象。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9a04df77ee010368b73abfe5a2d8d78cfe99b0b4
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217561"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="10e6e-104">stringKeyObjectValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="10e6e-104">stringKeyObjectValuePair resource type</span></span>

<span data-ttu-id="10e6e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10e6e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10e6e-106">表示键值对，其中键是字符串，值是任意的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="10e6e-106">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="10e6e-107">这是一种 OData 开放类型，它应具有一个名`value`为的属性，它是一个有效的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="10e6e-107">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="10e6e-108">属性</span><span class="sxs-lookup"><span data-stu-id="10e6e-108">Properties</span></span>
| <span data-ttu-id="10e6e-109">属性</span><span class="sxs-lookup"><span data-stu-id="10e6e-109">Property</span></span>     | <span data-ttu-id="10e6e-110">类型</span><span class="sxs-lookup"><span data-stu-id="10e6e-110">Type</span></span>   |<span data-ttu-id="10e6e-111">说明</span><span class="sxs-lookup"><span data-stu-id="10e6e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10e6e-112">Key</span><span class="sxs-lookup"><span data-stu-id="10e6e-112">key</span></span>|<span data-ttu-id="10e6e-113">String</span><span class="sxs-lookup"><span data-stu-id="10e6e-113">String</span></span>|<span data-ttu-id="10e6e-114">键。</span><span class="sxs-lookup"><span data-stu-id="10e6e-114">Key.</span></span>|
|<span data-ttu-id="10e6e-115">值</span><span class="sxs-lookup"><span data-stu-id="10e6e-115">value</span></span>|<span data-ttu-id="10e6e-116">Json</span><span class="sxs-lookup"><span data-stu-id="10e6e-116">Json</span></span>|<span data-ttu-id="10e6e-117">任意 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="10e6e-117">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10e6e-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10e6e-118">JSON representation</span></span>

<span data-ttu-id="10e6e-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10e6e-119">The following is a JSON representation of the resource.</span></span>

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
