---
title: addIn 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 46daa8c4f1218b3de485643a47f7acbe881c661c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974524"
---
# <a name="addin-resource-type"></a><span data-ttu-id="e597d-103">addIn 资源类型</span><span class="sxs-lookup"><span data-stu-id="e597d-103">addIn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="e597d-104">属性</span><span class="sxs-lookup"><span data-stu-id="e597d-104">Properties</span></span>
| <span data-ttu-id="e597d-105">属性</span><span class="sxs-lookup"><span data-stu-id="e597d-105">Property</span></span>     | <span data-ttu-id="e597d-106">类型</span><span class="sxs-lookup"><span data-stu-id="e597d-106">Type</span></span>   |<span data-ttu-id="e597d-107">说明</span><span class="sxs-lookup"><span data-stu-id="e597d-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e597d-108">id</span><span class="sxs-lookup"><span data-stu-id="e597d-108">id</span></span>|<span data-ttu-id="e597d-109">containerparentjob</span><span class="sxs-lookup"><span data-stu-id="e597d-109">guid</span></span>||
|<span data-ttu-id="e597d-110">properties</span><span class="sxs-lookup"><span data-stu-id="e597d-110">properties</span></span>|<span data-ttu-id="e597d-111">[keyValue](keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e597d-111">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="e597d-112">类型</span><span class="sxs-lookup"><span data-stu-id="e597d-112">type</span></span>|<span data-ttu-id="e597d-113">string</span><span class="sxs-lookup"><span data-stu-id="e597d-113">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="e597d-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e597d-114">JSON representation</span></span>

<span data-ttu-id="e597d-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e597d-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyValue"}],
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
