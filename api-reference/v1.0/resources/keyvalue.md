---
title: keyValue 资源类型
description: 标准键值对资源类型。
localization_priority: Normal
author: dougeby
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3ae252d03884b6d43b2ca12a4d59d2f5477dab5b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134713"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="1c780-103">keyValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c780-103">keyValue resource type</span></span>

<span data-ttu-id="1c780-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c780-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c780-105">表示键值对。</span><span class="sxs-lookup"><span data-stu-id="1c780-105">Represents a key-value pair.</span></span>

## <a name="properties"></a><span data-ttu-id="1c780-106">属性</span><span class="sxs-lookup"><span data-stu-id="1c780-106">Properties</span></span>

| <span data-ttu-id="1c780-107">属性</span><span class="sxs-lookup"><span data-stu-id="1c780-107">Property</span></span>     | <span data-ttu-id="1c780-108">类型</span><span class="sxs-lookup"><span data-stu-id="1c780-108">Type</span></span>   |<span data-ttu-id="1c780-109">说明</span><span class="sxs-lookup"><span data-stu-id="1c780-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c780-110">Key</span><span class="sxs-lookup"><span data-stu-id="1c780-110">key</span></span>|<span data-ttu-id="1c780-111">string</span><span class="sxs-lookup"><span data-stu-id="1c780-111">string</span></span>| <span data-ttu-id="1c780-112">键值对的键。</span><span class="sxs-lookup"><span data-stu-id="1c780-112">Key for the key-value pair.</span></span> |
|<span data-ttu-id="1c780-113">value</span><span class="sxs-lookup"><span data-stu-id="1c780-113">value</span></span>|<span data-ttu-id="1c780-114">string</span><span class="sxs-lookup"><span data-stu-id="1c780-114">string</span></span>| <span data-ttu-id="1c780-115">键值对的值。</span><span class="sxs-lookup"><span data-stu-id="1c780-115">Value for the key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c780-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c780-116">JSON representation</span></span>

<span data-ttu-id="1c780-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c780-117">Here is a JSON representation of the resource.</span></span>

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

