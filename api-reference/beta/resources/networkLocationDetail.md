---
title: networkLocationDetail 资源类型
description: 指示与网络位置相关联的详细信息。 .
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3b7e12a87889909737cac9a52fadf64231f7f2a5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009606"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="f3eab-104">networkLocationDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3eab-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="f3eab-105">指示与网络位置相关联的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f3eab-105">Indicates details associated with the network location.</span></span>



## <a name="properties"></a><span data-ttu-id="f3eab-106">属性</span><span class="sxs-lookup"><span data-stu-id="f3eab-106">Properties</span></span>
| <span data-ttu-id="f3eab-107">属性</span><span class="sxs-lookup"><span data-stu-id="f3eab-107">Property</span></span>     | <span data-ttu-id="f3eab-108">类型</span><span class="sxs-lookup"><span data-stu-id="f3eab-108">Type</span></span>   |<span data-ttu-id="f3eab-109">说明</span><span class="sxs-lookup"><span data-stu-id="f3eab-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3eab-110">网络</span><span class="sxs-lookup"><span data-stu-id="f3eab-110">networkType</span></span>|<span data-ttu-id="f3eab-111">网络</span><span class="sxs-lookup"><span data-stu-id="f3eab-111">networkType</span></span>|<span data-ttu-id="f3eab-112">提供网络的类型。</span><span class="sxs-lookup"><span data-stu-id="f3eab-112">Provides the type of the network.</span></span> <span data-ttu-id="f3eab-113">可能的值为`intranet`、 `extranet` `namedNetwork`、和`trusted`。</span><span class="sxs-lookup"><span data-stu-id="f3eab-113">The possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="f3eab-114">networkNames</span><span class="sxs-lookup"><span data-stu-id="f3eab-114">networkNames</span></span>|<span data-ttu-id="f3eab-115">String collection</span><span class="sxs-lookup"><span data-stu-id="f3eab-115">String collection</span></span>|<span data-ttu-id="f3eab-116">网络的名称。</span><span class="sxs-lookup"><span data-stu-id="f3eab-116">Names of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f3eab-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3eab-117">JSON representation</span></span>

<span data-ttu-id="f3eab-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3eab-118">Here is a JSON representation of the resource.</span></span>

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
