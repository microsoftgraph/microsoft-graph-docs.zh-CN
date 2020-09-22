---
title: serviceEndpoint 资源类型
description: ServiceEndpoint 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e51d8998ffe332426c617e1b17abd6a6362da77e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069321"
---
# <a name="serviceendpoint-resource-type"></a><span data-ttu-id="668bc-103">serviceEndpoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="668bc-103">serviceEndpoint resource type</span></span>

<span data-ttu-id="668bc-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="668bc-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="668bc-105">表示呼叫中的服务终结点。</span><span class="sxs-lookup"><span data-stu-id="668bc-105">Represents a service endpoint in a call.</span></span> <span data-ttu-id="668bc-106">终结点表示呼叫媒体服务器或其他服务实体。</span><span class="sxs-lookup"><span data-stu-id="668bc-106">The endpoint represents a calling media server or other service entity.</span></span> <span data-ttu-id="668bc-107">从 [终结点](callrecords-endpoint.md) 类型继承。</span><span class="sxs-lookup"><span data-stu-id="668bc-107">Inherits from [endpoint](callrecords-endpoint.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="668bc-108">属性</span><span class="sxs-lookup"><span data-stu-id="668bc-108">Properties</span></span>

| <span data-ttu-id="668bc-109">属性</span><span class="sxs-lookup"><span data-stu-id="668bc-109">Property</span></span>     | <span data-ttu-id="668bc-110">类型</span><span class="sxs-lookup"><span data-stu-id="668bc-110">Type</span></span>        | <span data-ttu-id="668bc-111">说明</span><span class="sxs-lookup"><span data-stu-id="668bc-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="668bc-112">userAgent</span><span class="sxs-lookup"><span data-stu-id="668bc-112">userAgent</span></span>|[<span data-ttu-id="668bc-113">callRecords。 userAgent</span><span class="sxs-lookup"><span data-stu-id="668bc-113">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="668bc-114">此终结点报告的用户代理。</span><span class="sxs-lookup"><span data-stu-id="668bc-114">User-agent reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="668bc-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="668bc-115">JSON representation</span></span>

<span data-ttu-id="668bc-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="668bc-116">The following is a JSON representation of the resource.</span></span>

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
