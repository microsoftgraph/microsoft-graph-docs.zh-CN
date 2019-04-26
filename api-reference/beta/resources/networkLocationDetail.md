---
title: networkLocationDetail 资源类型
description: 指示与网络位置相关联的详细信息。 .
localization_priority: Normal
ms.openlocfilehash: c4a5323099258d9670b970b1bb85bd0d01f3cf8d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342175"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="d788f-104">networkLocationDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="d788f-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="d788f-105">指示与网络位置相关联的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d788f-105">Indicates details associated with the network location.</span></span>



## <a name="properties"></a><span data-ttu-id="d788f-106">属性</span><span class="sxs-lookup"><span data-stu-id="d788f-106">Properties</span></span>
| <span data-ttu-id="d788f-107">属性</span><span class="sxs-lookup"><span data-stu-id="d788f-107">Property</span></span>     | <span data-ttu-id="d788f-108">类型</span><span class="sxs-lookup"><span data-stu-id="d788f-108">Type</span></span>   |<span data-ttu-id="d788f-109">说明</span><span class="sxs-lookup"><span data-stu-id="d788f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d788f-110">网络</span><span class="sxs-lookup"><span data-stu-id="d788f-110">networkType</span></span>|<span data-ttu-id="d788f-111">网络</span><span class="sxs-lookup"><span data-stu-id="d788f-111">networkType</span></span>|<span data-ttu-id="d788f-112">提供网络的类型。</span><span class="sxs-lookup"><span data-stu-id="d788f-112">Provides the type of the network.</span></span> <span data-ttu-id="d788f-113">可能的值为`intranet`、 `extranet` `namedNetwork`、和`trusted`。</span><span class="sxs-lookup"><span data-stu-id="d788f-113">The possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="d788f-114">networkNames</span><span class="sxs-lookup"><span data-stu-id="d788f-114">networkNames</span></span>|<span data-ttu-id="d788f-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="d788f-115">String collection</span></span>|<span data-ttu-id="d788f-116">网络的名称。</span><span class="sxs-lookup"><span data-stu-id="d788f-116">Names of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d788f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d788f-117">JSON representation</span></span>

<span data-ttu-id="d788f-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d788f-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkLocationDetail"
}-->

```json
{
  "networkType": "string",
  "networkNames": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkLocationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
