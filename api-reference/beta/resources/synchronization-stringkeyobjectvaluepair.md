---
title: stringKeyObjectValuePair 资源类型
description: 表示键值对，其中键是字符串，值是任意 JSON 对象。 这是一种 OData 打开类型，预期具有一个名为有效 `value` JSON 对象的属性。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 535e9f104f42771e6f6c182769f0a5e1f68169b6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137065"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="7a65d-104">stringKeyObjectValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a65d-104">stringKeyObjectValuePair resource type</span></span>

<span data-ttu-id="7a65d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a65d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a65d-106">表示键值对，其中键是字符串，值是任意 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7a65d-106">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="7a65d-107">这是一种 OData 打开类型，预期具有一个名为有效 `value` JSON 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7a65d-107">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="7a65d-108">属性</span><span class="sxs-lookup"><span data-stu-id="7a65d-108">Properties</span></span>
| <span data-ttu-id="7a65d-109">属性</span><span class="sxs-lookup"><span data-stu-id="7a65d-109">Property</span></span>     | <span data-ttu-id="7a65d-110">类型</span><span class="sxs-lookup"><span data-stu-id="7a65d-110">Type</span></span>   |<span data-ttu-id="7a65d-111">说明</span><span class="sxs-lookup"><span data-stu-id="7a65d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a65d-112">Key</span><span class="sxs-lookup"><span data-stu-id="7a65d-112">key</span></span>|<span data-ttu-id="7a65d-113">String</span><span class="sxs-lookup"><span data-stu-id="7a65d-113">String</span></span>|<span data-ttu-id="7a65d-114">键。</span><span class="sxs-lookup"><span data-stu-id="7a65d-114">Key.</span></span>|
|<span data-ttu-id="7a65d-115">值</span><span class="sxs-lookup"><span data-stu-id="7a65d-115">value</span></span>|<span data-ttu-id="7a65d-116">Json</span><span class="sxs-lookup"><span data-stu-id="7a65d-116">Json</span></span>|<span data-ttu-id="7a65d-117">任意 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7a65d-117">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a65d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a65d-118">JSON representation</span></span>

<span data-ttu-id="7a65d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a65d-119">The following is a JSON representation of the resource.</span></span>

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


