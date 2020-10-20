---
title: serviceEndpoint 资源类型
description: ServiceEndpoint 类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b650b2f105a9feb2d33327a0ceef9add18716d00
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601564"
---
# <a name="serviceendpoint-resource-type"></a><span data-ttu-id="33239-103">serviceEndpoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="33239-103">serviceEndpoint resource type</span></span>

<span data-ttu-id="33239-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="33239-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="33239-105">表示呼叫中的服务终结点。</span><span class="sxs-lookup"><span data-stu-id="33239-105">Represents a service endpoint in a call.</span></span> <span data-ttu-id="33239-106">终结点表示呼叫媒体服务器或其他服务实体。</span><span class="sxs-lookup"><span data-stu-id="33239-106">The endpoint represents a calling media server or other service entity.</span></span> <span data-ttu-id="33239-107">从 [终结点](callrecords-endpoint.md) 类型继承。</span><span class="sxs-lookup"><span data-stu-id="33239-107">Inherits from [endpoint](callrecords-endpoint.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="33239-108">属性</span><span class="sxs-lookup"><span data-stu-id="33239-108">Properties</span></span>

| <span data-ttu-id="33239-109">属性</span><span class="sxs-lookup"><span data-stu-id="33239-109">Property</span></span>     | <span data-ttu-id="33239-110">类型</span><span class="sxs-lookup"><span data-stu-id="33239-110">Type</span></span>        | <span data-ttu-id="33239-111">说明</span><span class="sxs-lookup"><span data-stu-id="33239-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="33239-112">userAgent</span><span class="sxs-lookup"><span data-stu-id="33239-112">userAgent</span></span>|[<span data-ttu-id="33239-113">callRecords。 userAgent</span><span class="sxs-lookup"><span data-stu-id="33239-113">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="33239-114">此终结点报告的用户代理。</span><span class="sxs-lookup"><span data-stu-id="33239-114">User-agent reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33239-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33239-115">JSON representation</span></span>

<span data-ttu-id="33239-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33239-116">The following is a JSON representation of the resource.</span></span>

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
