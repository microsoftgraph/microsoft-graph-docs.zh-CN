---
title: 键值资源类型
description: 标准键值对资源类型。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: adac348de690b3796399a4276ede4280f35713b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447603"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="a1833-103">键值资源类型</span><span class="sxs-lookup"><span data-stu-id="a1833-103">keyValue resource type</span></span>

<span data-ttu-id="a1833-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a1833-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1833-105">表示键/值对。</span><span class="sxs-lookup"><span data-stu-id="a1833-105">Represents a key-value pair.</span></span>

## <a name="properties"></a><span data-ttu-id="a1833-106">属性</span><span class="sxs-lookup"><span data-stu-id="a1833-106">Properties</span></span>

| <span data-ttu-id="a1833-107">属性</span><span class="sxs-lookup"><span data-stu-id="a1833-107">Property</span></span>     | <span data-ttu-id="a1833-108">类型</span><span class="sxs-lookup"><span data-stu-id="a1833-108">Type</span></span>   |<span data-ttu-id="a1833-109">说明</span><span class="sxs-lookup"><span data-stu-id="a1833-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1833-110">Key</span><span class="sxs-lookup"><span data-stu-id="a1833-110">key</span></span>|<span data-ttu-id="a1833-111">string</span><span class="sxs-lookup"><span data-stu-id="a1833-111">string</span></span>| <span data-ttu-id="a1833-112">键/值对的键。</span><span class="sxs-lookup"><span data-stu-id="a1833-112">Key for the key-value pair.</span></span> |
|<span data-ttu-id="a1833-113">value</span><span class="sxs-lookup"><span data-stu-id="a1833-113">value</span></span>|<span data-ttu-id="a1833-114">字符串</span><span class="sxs-lookup"><span data-stu-id="a1833-114">string</span></span>| <span data-ttu-id="a1833-115">键/值对的值。</span><span class="sxs-lookup"><span data-stu-id="a1833-115">Value for the key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1833-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1833-116">JSON representation</span></span>

<span data-ttu-id="a1833-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1833-117">Here is a JSON representation of the resource.</span></span>

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
