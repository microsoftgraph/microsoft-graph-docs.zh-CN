---
title: stringKeyObjectValuePair 资源类型
description: 表示其中的密钥是一个字符串，值是一个任意 JSON 对象的键 / 值对。 这是认为应该有一个名为属性 OData 打开类型`value`，它是一个有效的 JSON 对象。
localization_priority: Normal
ms.openlocfilehash: 8545a4ef5a4931d3b886c95b4f39218bc418f53d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831449"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="4a565-104">stringKeyObjectValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a565-104">stringKeyObjectValuePair resource type</span></span>

> <span data-ttu-id="4a565-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4a565-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a565-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4a565-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a565-107">表示其中的密钥是一个字符串，值是一个任意 JSON 对象的键 / 值对。</span><span class="sxs-lookup"><span data-stu-id="4a565-107">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="4a565-108">这是认为应该有一个名为属性 OData 打开类型`value`，它是一个有效的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4a565-108">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="4a565-109">属性</span><span class="sxs-lookup"><span data-stu-id="4a565-109">Properties</span></span>
| <span data-ttu-id="4a565-110">属性</span><span class="sxs-lookup"><span data-stu-id="4a565-110">Property</span></span>     | <span data-ttu-id="4a565-111">类型</span><span class="sxs-lookup"><span data-stu-id="4a565-111">Type</span></span>   |<span data-ttu-id="4a565-112">说明</span><span class="sxs-lookup"><span data-stu-id="4a565-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a565-113">Key</span><span class="sxs-lookup"><span data-stu-id="4a565-113">key</span></span>|<span data-ttu-id="4a565-114">字符串</span><span class="sxs-lookup"><span data-stu-id="4a565-114">String</span></span>|<span data-ttu-id="4a565-115">键。</span><span class="sxs-lookup"><span data-stu-id="4a565-115">Key.</span></span>|
|<span data-ttu-id="4a565-116">值</span><span class="sxs-lookup"><span data-stu-id="4a565-116">value</span></span>|<span data-ttu-id="4a565-117">任意</span><span class="sxs-lookup"><span data-stu-id="4a565-117">Any</span></span>|<span data-ttu-id="4a565-118">任意的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4a565-118">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a565-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a565-119">JSON representation</span></span>

<span data-ttu-id="4a565-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a565-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
