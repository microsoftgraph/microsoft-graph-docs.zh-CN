---
title: stringKeyObjectValuePair 资源类型
description: 表示其中的密钥是一个字符串，值是一个任意 JSON 对象的键 / 值对。 这是认为应该有一个名为属性 OData 打开类型`value`，它是一个有效的 JSON 对象。
localization_priority: Normal
ms.openlocfilehash: 8f939c177f2130813c6080d46ad78664f6118857
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516964"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="19e75-104">stringKeyObjectValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="19e75-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19e75-105">表示其中的密钥是一个字符串，值是一个任意 JSON 对象的键 / 值对。</span><span class="sxs-lookup"><span data-stu-id="19e75-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="19e75-106">这是认为应该有一个名为属性 OData 打开类型`value`，它是一个有效的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="19e75-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="19e75-107">属性</span><span class="sxs-lookup"><span data-stu-id="19e75-107">Properties</span></span>
| <span data-ttu-id="19e75-108">属性</span><span class="sxs-lookup"><span data-stu-id="19e75-108">Property</span></span>     | <span data-ttu-id="19e75-109">类型</span><span class="sxs-lookup"><span data-stu-id="19e75-109">Type</span></span>   |<span data-ttu-id="19e75-110">说明</span><span class="sxs-lookup"><span data-stu-id="19e75-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19e75-111">Key</span><span class="sxs-lookup"><span data-stu-id="19e75-111">key</span></span>|<span data-ttu-id="19e75-112">String</span><span class="sxs-lookup"><span data-stu-id="19e75-112">String</span></span>|<span data-ttu-id="19e75-113">键。</span><span class="sxs-lookup"><span data-stu-id="19e75-113">Key.</span></span>|
|<span data-ttu-id="19e75-114">值</span><span class="sxs-lookup"><span data-stu-id="19e75-114">value</span></span>|<span data-ttu-id="19e75-115">任意</span><span class="sxs-lookup"><span data-stu-id="19e75-115">Any</span></span>|<span data-ttu-id="19e75-116">任意的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="19e75-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19e75-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19e75-117">JSON representation</span></span>

<span data-ttu-id="19e75-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19e75-118">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeyobjectvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
