---
title: stringKeyStringValuePair 资源类型
description: 表示键值对，其中键是字符串，值是字符串。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 03bcea7786b5790ad9936d7068d5b89ef3214088
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217554"
---
# <a name="stringkeystringvaluepair-resource-type"></a><span data-ttu-id="aad11-103">stringKeyStringValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="aad11-103">stringKeyStringValuePair resource type</span></span>

<span data-ttu-id="aad11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aad11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aad11-105">表示键值对，其中键是字符串，值是字符串。</span><span class="sxs-lookup"><span data-stu-id="aad11-105">Represents a key-value pair where the key is a string and the value is a string.</span></span>

## <a name="properties"></a><span data-ttu-id="aad11-106">属性</span><span class="sxs-lookup"><span data-stu-id="aad11-106">Properties</span></span>
| <span data-ttu-id="aad11-107">属性</span><span class="sxs-lookup"><span data-stu-id="aad11-107">Property</span></span>     | <span data-ttu-id="aad11-108">类型</span><span class="sxs-lookup"><span data-stu-id="aad11-108">Type</span></span>   |<span data-ttu-id="aad11-109">说明</span><span class="sxs-lookup"><span data-stu-id="aad11-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aad11-110">Key</span><span class="sxs-lookup"><span data-stu-id="aad11-110">key</span></span>|<span data-ttu-id="aad11-111">字符串</span><span class="sxs-lookup"><span data-stu-id="aad11-111">String</span></span>|<span data-ttu-id="aad11-112">键。</span><span class="sxs-lookup"><span data-stu-id="aad11-112">Key.</span></span>|
|<span data-ttu-id="aad11-113">value</span><span class="sxs-lookup"><span data-stu-id="aad11-113">value</span></span>|<span data-ttu-id="aad11-114">String</span><span class="sxs-lookup"><span data-stu-id="aad11-114">String</span></span>|<span data-ttu-id="aad11-115">值。</span><span class="sxs-lookup"><span data-stu-id="aad11-115">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aad11-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aad11-116">JSON representation</span></span>

<span data-ttu-id="aad11-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aad11-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
