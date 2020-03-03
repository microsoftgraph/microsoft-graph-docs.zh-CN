---
title: 终结点资源类型
description: 终结点类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f17aa21de65fef33b0c7e4a94151eab4f49583ac
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394748"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="30039-103">终结点资源类型</span><span class="sxs-lookup"><span data-stu-id="30039-103">endpoint resource type</span></span>

<span data-ttu-id="30039-104">命名空间： callRecords</span><span class="sxs-lookup"><span data-stu-id="30039-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30039-105">表示调用中的终结点。</span><span class="sxs-lookup"><span data-stu-id="30039-105">Represents an endpoint in a call.</span></span> <span data-ttu-id="30039-106">终结点可以是用户的设备、会议、应用程序/机器人等。[ParticipantEndpoint](callrecords-participantendpoint.md)和[serviceEndpoint](callrecords-serviceendpoint.md)类型继承自此类型。</span><span class="sxs-lookup"><span data-stu-id="30039-106">The endpoint could be a user's device, a meeting, an application/bot, etc. The [participantEndpoint](callrecords-participantendpoint.md) and [serviceEndpoint](callrecords-serviceendpoint.md) types inherit from this type.</span></span>

## <a name="properties"></a><span data-ttu-id="30039-107">属性</span><span class="sxs-lookup"><span data-stu-id="30039-107">Properties</span></span>

| <span data-ttu-id="30039-108">属性</span><span class="sxs-lookup"><span data-stu-id="30039-108">Property</span></span>     | <span data-ttu-id="30039-109">类型</span><span class="sxs-lookup"><span data-stu-id="30039-109">Type</span></span>        | <span data-ttu-id="30039-110">说明</span><span class="sxs-lookup"><span data-stu-id="30039-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="30039-111">userAgent</span><span class="sxs-lookup"><span data-stu-id="30039-111">userAgent</span></span>|[<span data-ttu-id="30039-112">callRecords。 userAgent</span><span class="sxs-lookup"><span data-stu-id="30039-112">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="30039-113">此终结点报告的用户代理。</span><span class="sxs-lookup"><span data-stu-id="30039-113">User-agent reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30039-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30039-114">JSON representation</span></span>

<span data-ttu-id="30039-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30039-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.endpoint",
  "baseType": null
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
  "description": "endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->