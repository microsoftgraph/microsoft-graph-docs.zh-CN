---
title: 键值资源类型
description: 标准键值对资源类型。
localization_priority: Normal
ms.openlocfilehash: aa026f36d69e894e056f21ba19865c730ec5b643
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629269"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="04e54-103">键值资源类型</span><span class="sxs-lookup"><span data-stu-id="04e54-103">keyValue resource type</span></span>

<span data-ttu-id="04e54-104">表示键/值对。</span><span class="sxs-lookup"><span data-stu-id="04e54-104">Represents a key-value pair.</span></span>

## <a name="properties"></a><span data-ttu-id="04e54-105">属性</span><span class="sxs-lookup"><span data-stu-id="04e54-105">Properties</span></span>

| <span data-ttu-id="04e54-106">属性</span><span class="sxs-lookup"><span data-stu-id="04e54-106">Property</span></span>     | <span data-ttu-id="04e54-107">类型</span><span class="sxs-lookup"><span data-stu-id="04e54-107">Type</span></span>   |<span data-ttu-id="04e54-108">说明</span><span class="sxs-lookup"><span data-stu-id="04e54-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04e54-109">Key</span><span class="sxs-lookup"><span data-stu-id="04e54-109">key</span></span>|<span data-ttu-id="04e54-110">string</span><span class="sxs-lookup"><span data-stu-id="04e54-110">string</span></span>| <span data-ttu-id="04e54-111">键/值对的键。</span><span class="sxs-lookup"><span data-stu-id="04e54-111">Key for the key-value pair.</span></span> |
|<span data-ttu-id="04e54-112">value</span><span class="sxs-lookup"><span data-stu-id="04e54-112">value</span></span>|<span data-ttu-id="04e54-113">字符串</span><span class="sxs-lookup"><span data-stu-id="04e54-113">string</span></span>| <span data-ttu-id="04e54-114">键/值对的值。</span><span class="sxs-lookup"><span data-stu-id="04e54-114">Value for the key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04e54-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04e54-115">JSON representation</span></span>

<span data-ttu-id="04e54-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04e54-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValue"
}-->

```json
{
  "key": "string",
  "value": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
