---
title: networkLocationDetail 资源类型
description: 指示与的网络位置关联的详细信息。 .
localization_priority: Normal
ms.openlocfilehash: bfa84591f543253ed794016bbc2d25d325cd0bcc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834319"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="73ed4-104">networkLocationDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="73ed4-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="73ed4-105">指示与的网络位置关联的详细信息。</span><span class="sxs-lookup"><span data-stu-id="73ed4-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="73ed4-106">.</span><span class="sxs-lookup"><span data-stu-id="73ed4-106"></span></span>



## <a name="properties"></a><span data-ttu-id="73ed4-107">属性</span><span class="sxs-lookup"><span data-stu-id="73ed4-107">Properties</span></span>
| <span data-ttu-id="73ed4-108">属性</span><span class="sxs-lookup"><span data-stu-id="73ed4-108">Property</span></span>     | <span data-ttu-id="73ed4-109">类型</span><span class="sxs-lookup"><span data-stu-id="73ed4-109">Type</span></span>   |<span data-ttu-id="73ed4-110">Description</span><span class="sxs-lookup"><span data-stu-id="73ed4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73ed4-111">networkType</span><span class="sxs-lookup"><span data-stu-id="73ed4-111">networkType</span></span>|<span data-ttu-id="73ed4-112">字符串</span><span class="sxs-lookup"><span data-stu-id="73ed4-112">String</span></span>|<span data-ttu-id="73ed4-113">提供了网络的类型。</span><span class="sxs-lookup"><span data-stu-id="73ed4-113">Provides the type of the network.</span></span> <span data-ttu-id="73ed4-114">可能的值为`intranet`， `extranet`， `namedNetwork`，和`trusted`。</span><span class="sxs-lookup"><span data-stu-id="73ed4-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="73ed4-115">networkName</span><span class="sxs-lookup"><span data-stu-id="73ed4-115">networkName</span></span>|<span data-ttu-id="73ed4-116">字符串</span><span class="sxs-lookup"><span data-stu-id="73ed4-116">String</span></span>|<span data-ttu-id="73ed4-117">网络的名称。</span><span class="sxs-lookup"><span data-stu-id="73ed4-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="73ed4-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73ed4-118">JSON representation</span></span>

<span data-ttu-id="73ed4-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73ed4-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "networkTypes": "namedNetork",
  "networkName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
