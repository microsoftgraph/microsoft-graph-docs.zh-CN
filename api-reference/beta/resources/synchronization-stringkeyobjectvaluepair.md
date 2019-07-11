---
title: stringKeyObjectValuePair 资源类型
description: 表示键值对, 其中键是字符串, 值是任意的 JSON 对象。 这是一种 OData 开放类型, 它应具有一个名`value`为的属性, 它是一个有效的 JSON 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b97f1f8bf10005a9e7829ee9280ebf936405b346
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620626"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="d4229-104">stringKeyObjectValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4229-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4229-105">表示键值对, 其中键是字符串, 值是任意的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d4229-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="d4229-106">这是一种 OData 开放类型, 它应具有一个名`value`为的属性, 它是一个有效的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d4229-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="d4229-107">属性</span><span class="sxs-lookup"><span data-stu-id="d4229-107">Properties</span></span>
| <span data-ttu-id="d4229-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4229-108">Property</span></span>     | <span data-ttu-id="d4229-109">类型</span><span class="sxs-lookup"><span data-stu-id="d4229-109">Type</span></span>   |<span data-ttu-id="d4229-110">说明</span><span class="sxs-lookup"><span data-stu-id="d4229-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4229-111">Key</span><span class="sxs-lookup"><span data-stu-id="d4229-111">key</span></span>|<span data-ttu-id="d4229-112">String</span><span class="sxs-lookup"><span data-stu-id="d4229-112">String</span></span>|<span data-ttu-id="d4229-113">键。</span><span class="sxs-lookup"><span data-stu-id="d4229-113">Key.</span></span>|
|<span data-ttu-id="d4229-114">值</span><span class="sxs-lookup"><span data-stu-id="d4229-114">value</span></span>|<span data-ttu-id="d4229-115">Json</span><span class="sxs-lookup"><span data-stu-id="d4229-115">Json</span></span>|<span data-ttu-id="d4229-116">任意 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d4229-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4229-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4229-117">JSON representation</span></span>

<span data-ttu-id="d4229-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4229-118">The following is a JSON representation of the resource.</span></span>

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
