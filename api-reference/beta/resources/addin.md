---
title: addIn 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 777b9e2eac1ec4052fae30b13d09aaf91a808375
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339121"
---
# <a name="addin-resource-type"></a><span data-ttu-id="0c4ba-103">addIn 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c4ba-103">addIn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="0c4ba-104">属性</span><span class="sxs-lookup"><span data-stu-id="0c4ba-104">Properties</span></span>
| <span data-ttu-id="0c4ba-105">属性</span><span class="sxs-lookup"><span data-stu-id="0c4ba-105">Property</span></span>     | <span data-ttu-id="0c4ba-106">类型</span><span class="sxs-lookup"><span data-stu-id="0c4ba-106">Type</span></span>   |<span data-ttu-id="0c4ba-107">说明</span><span class="sxs-lookup"><span data-stu-id="0c4ba-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c4ba-108">id</span><span class="sxs-lookup"><span data-stu-id="0c4ba-108">id</span></span>|<span data-ttu-id="0c4ba-109">containerparentjob</span><span class="sxs-lookup"><span data-stu-id="0c4ba-109">guid</span></span>||
|<span data-ttu-id="0c4ba-110">properties</span><span class="sxs-lookup"><span data-stu-id="0c4ba-110">properties</span></span>|<span data-ttu-id="0c4ba-111">[keyValue](keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0c4ba-111">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="0c4ba-112">类型</span><span class="sxs-lookup"><span data-stu-id="0c4ba-112">type</span></span>|<span data-ttu-id="0c4ba-113">string</span><span class="sxs-lookup"><span data-stu-id="0c4ba-113">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="0c4ba-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c4ba-114">JSON representation</span></span>

<span data-ttu-id="0c4ba-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c4ba-115">Here is a JSON representation of the resource.</span></span>

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
