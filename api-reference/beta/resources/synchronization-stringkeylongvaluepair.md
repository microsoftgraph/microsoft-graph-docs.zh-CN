---
title: stringKeyLongValuePair 资源类型
description: 表示键值对，其中键是字符串，值为 Int64。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7a726b1aa3aa122422cd43003366996c479461e0
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217568"
---
# <a name="stringkeylongvaluepair-resource-type"></a><span data-ttu-id="196a6-103">stringKeyLongValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="196a6-103">stringKeyLongValuePair resource type</span></span>

<span data-ttu-id="196a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="196a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="196a6-105">表示键值对，其中键是字符串，值为 Int64。</span><span class="sxs-lookup"><span data-stu-id="196a6-105">Represents a key-value pair where the key is a string and the value is an Int64.</span></span>

## <a name="properties"></a><span data-ttu-id="196a6-106">属性</span><span class="sxs-lookup"><span data-stu-id="196a6-106">Properties</span></span>
| <span data-ttu-id="196a6-107">属性</span><span class="sxs-lookup"><span data-stu-id="196a6-107">Property</span></span>     | <span data-ttu-id="196a6-108">类型</span><span class="sxs-lookup"><span data-stu-id="196a6-108">Type</span></span>   |<span data-ttu-id="196a6-109">说明</span><span class="sxs-lookup"><span data-stu-id="196a6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="196a6-110">Key</span><span class="sxs-lookup"><span data-stu-id="196a6-110">key</span></span>|<span data-ttu-id="196a6-111">String</span><span class="sxs-lookup"><span data-stu-id="196a6-111">String</span></span>|<span data-ttu-id="196a6-112">键。</span><span class="sxs-lookup"><span data-stu-id="196a6-112">Key.</span></span>|
|<span data-ttu-id="196a6-113">值</span><span class="sxs-lookup"><span data-stu-id="196a6-113">value</span></span>|<span data-ttu-id="196a6-114">Int64</span><span class="sxs-lookup"><span data-stu-id="196a6-114">Int64</span></span>|<span data-ttu-id="196a6-115">值。</span><span class="sxs-lookup"><span data-stu-id="196a6-115">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="196a6-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="196a6-116">JSON representation</span></span>

<span data-ttu-id="196a6-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="196a6-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyLongValuePair"
}-->

```json
{
  "key": "String",
  "value": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyLongValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
