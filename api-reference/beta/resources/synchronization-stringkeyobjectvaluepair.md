---
title: stringKeyObjectValuePair 资源类型
description: 表示键值对, 其中键是字符串, 值是任意的 JSON 对象。 这是一种 OData 开放类型, 它应具有一个名`value`为的属性, 它是一个有效的 JSON 对象。
localization_priority: Normal
ms.openlocfilehash: 8f939c177f2130813c6080d46ad78664f6118857
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523208"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="0e7e8-104">stringKeyObjectValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e7e8-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e7e8-105">表示键值对, 其中键是字符串, 值是任意的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0e7e8-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="0e7e8-106">这是一种 OData 开放类型, 它应具有一个名`value`为的属性, 它是一个有效的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0e7e8-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="0e7e8-107">属性</span><span class="sxs-lookup"><span data-stu-id="0e7e8-107">Properties</span></span>
| <span data-ttu-id="0e7e8-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e7e8-108">Property</span></span>     | <span data-ttu-id="0e7e8-109">类型</span><span class="sxs-lookup"><span data-stu-id="0e7e8-109">Type</span></span>   |<span data-ttu-id="0e7e8-110">说明</span><span class="sxs-lookup"><span data-stu-id="0e7e8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e7e8-111">Key</span><span class="sxs-lookup"><span data-stu-id="0e7e8-111">key</span></span>|<span data-ttu-id="0e7e8-112">String</span><span class="sxs-lookup"><span data-stu-id="0e7e8-112">String</span></span>|<span data-ttu-id="0e7e8-113">键。</span><span class="sxs-lookup"><span data-stu-id="0e7e8-113">Key.</span></span>|
|<span data-ttu-id="0e7e8-114">值</span><span class="sxs-lookup"><span data-stu-id="0e7e8-114">value</span></span>|<span data-ttu-id="0e7e8-115">任意</span><span class="sxs-lookup"><span data-stu-id="0e7e8-115">Any</span></span>|<span data-ttu-id="0e7e8-116">任意 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0e7e8-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e7e8-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e7e8-117">JSON representation</span></span>

<span data-ttu-id="0e7e8-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e7e8-118">The following is a JSON representation of the resource.</span></span>

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
