---
title: networkLocationDetail 资源类型
description: 指示与网络位置相关联的详细信息。 .
localization_priority: Normal
ms.openlocfilehash: bfa84591f543253ed794016bbc2d25d325cd0bcc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581441"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="810ca-104">networkLocationDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="810ca-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="810ca-105">指示与网络位置相关联的详细信息。</span><span class="sxs-lookup"><span data-stu-id="810ca-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="810ca-106">.</span><span class="sxs-lookup"><span data-stu-id="810ca-106"></span></span>



## <a name="properties"></a><span data-ttu-id="810ca-107">属性</span><span class="sxs-lookup"><span data-stu-id="810ca-107">Properties</span></span>
| <span data-ttu-id="810ca-108">属性</span><span class="sxs-lookup"><span data-stu-id="810ca-108">Property</span></span>     | <span data-ttu-id="810ca-109">类型</span><span class="sxs-lookup"><span data-stu-id="810ca-109">Type</span></span>   |<span data-ttu-id="810ca-110">说明</span><span class="sxs-lookup"><span data-stu-id="810ca-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="810ca-111">网络</span><span class="sxs-lookup"><span data-stu-id="810ca-111">networkType</span></span>|<span data-ttu-id="810ca-112">String</span><span class="sxs-lookup"><span data-stu-id="810ca-112">String</span></span>|<span data-ttu-id="810ca-113">提供网络的类型。</span><span class="sxs-lookup"><span data-stu-id="810ca-113">Provides the type of the network.</span></span> <span data-ttu-id="810ca-114">可能的值`intranet`为`extranet`、 `namedNetwork`、和`trusted`。</span><span class="sxs-lookup"><span data-stu-id="810ca-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="810ca-115">networkName</span><span class="sxs-lookup"><span data-stu-id="810ca-115">networkName</span></span>|<span data-ttu-id="810ca-116">String</span><span class="sxs-lookup"><span data-stu-id="810ca-116">String</span></span>|<span data-ttu-id="810ca-117">网络的名称。</span><span class="sxs-lookup"><span data-stu-id="810ca-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="810ca-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="810ca-118">JSON representation</span></span>

<span data-ttu-id="810ca-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="810ca-119">Here is a JSON representation of the resource.</span></span>

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
