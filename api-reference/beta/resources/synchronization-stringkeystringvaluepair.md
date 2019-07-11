---
title: stringKeyStringValuePair 资源类型
description: 表示键值对, 其中键是字符串, 值是字符串。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 01e9dde3631858858e90164b37a5d68a97949454
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620813"
---
# <a name="stringkeystringvaluepair-resource-type"></a><span data-ttu-id="218c9-103">stringKeyStringValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="218c9-103">stringKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="218c9-104">表示键值对, 其中键是字符串, 值是字符串。</span><span class="sxs-lookup"><span data-stu-id="218c9-104">Represents a key-value pair where the key is a string and the value is a string.</span></span>

## <a name="properties"></a><span data-ttu-id="218c9-105">属性</span><span class="sxs-lookup"><span data-stu-id="218c9-105">Properties</span></span>
| <span data-ttu-id="218c9-106">属性</span><span class="sxs-lookup"><span data-stu-id="218c9-106">Property</span></span>     | <span data-ttu-id="218c9-107">类型</span><span class="sxs-lookup"><span data-stu-id="218c9-107">Type</span></span>   |<span data-ttu-id="218c9-108">说明</span><span class="sxs-lookup"><span data-stu-id="218c9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="218c9-109">Key</span><span class="sxs-lookup"><span data-stu-id="218c9-109">key</span></span>|<span data-ttu-id="218c9-110">String</span><span class="sxs-lookup"><span data-stu-id="218c9-110">String</span></span>|<span data-ttu-id="218c9-111">键。</span><span class="sxs-lookup"><span data-stu-id="218c9-111">Key.</span></span>|
|<span data-ttu-id="218c9-112">value</span><span class="sxs-lookup"><span data-stu-id="218c9-112">value</span></span>|<span data-ttu-id="218c9-113">String</span><span class="sxs-lookup"><span data-stu-id="218c9-113">String</span></span>|<span data-ttu-id="218c9-114">值。</span><span class="sxs-lookup"><span data-stu-id="218c9-114">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="218c9-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="218c9-115">JSON representation</span></span>

<span data-ttu-id="218c9-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="218c9-116">The following is a JSON representation of the resource.</span></span>

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
