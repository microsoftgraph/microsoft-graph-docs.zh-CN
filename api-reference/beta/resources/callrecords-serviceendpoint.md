---
title: serviceEndpoint 资源类型
description: ServiceEndpoint 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9fe86f55615c4e7d58a219f15bd9e6792e5ae72b
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394689"
---
# <a name="serviceendpoint-resource-type"></a><span data-ttu-id="2d093-103">serviceEndpoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d093-103">serviceEndpoint resource type</span></span>

<span data-ttu-id="2d093-104">命名空间： callRecords</span><span class="sxs-lookup"><span data-stu-id="2d093-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d093-105">表示呼叫中的服务终结点。</span><span class="sxs-lookup"><span data-stu-id="2d093-105">Represents a service endpoint in a call.</span></span> <span data-ttu-id="2d093-106">终结点表示呼叫媒体服务器或其他服务实体。</span><span class="sxs-lookup"><span data-stu-id="2d093-106">The endpoint represents a calling media server or other service entity.</span></span> <span data-ttu-id="2d093-107">从[终结点](callrecords-endpoint.md)类型继承。</span><span class="sxs-lookup"><span data-stu-id="2d093-107">Inherits from [endpoint](callrecords-endpoint.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="2d093-108">属性</span><span class="sxs-lookup"><span data-stu-id="2d093-108">Properties</span></span>

| <span data-ttu-id="2d093-109">属性</span><span class="sxs-lookup"><span data-stu-id="2d093-109">Property</span></span>     | <span data-ttu-id="2d093-110">类型</span><span class="sxs-lookup"><span data-stu-id="2d093-110">Type</span></span>        | <span data-ttu-id="2d093-111">说明</span><span class="sxs-lookup"><span data-stu-id="2d093-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2d093-112">userAgent</span><span class="sxs-lookup"><span data-stu-id="2d093-112">userAgent</span></span>|[<span data-ttu-id="2d093-113">callRecords。 userAgent</span><span class="sxs-lookup"><span data-stu-id="2d093-113">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="2d093-114">此终结点报告的用户代理。</span><span class="sxs-lookup"><span data-stu-id="2d093-114">User-agent reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d093-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d093-115">JSON representation</span></span>

<span data-ttu-id="2d093-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d093-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.serviceEndpoint",
  "baseType": "microsoft.graph.callRecords.endpoint"
}-->

```json
{
  "userAgent": {"@odata.type": "microsoft.graph.callRecords.userAgent"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->