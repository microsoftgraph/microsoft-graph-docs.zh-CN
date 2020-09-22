---
title: 终结点资源类型
description: 终结点类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ae7d976c9dbf94aadd11af1d48f8615f5fab14a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069442"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="e1db9-103">终结点资源类型</span><span class="sxs-lookup"><span data-stu-id="e1db9-103">endpoint resource type</span></span>

<span data-ttu-id="e1db9-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="e1db9-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="e1db9-105">表示调用中的终结点。</span><span class="sxs-lookup"><span data-stu-id="e1db9-105">Represents an endpoint in a call.</span></span> <span data-ttu-id="e1db9-106">终结点可以是用户的设备、会议、应用程序/机器人等。 [ParticipantEndpoint](callrecords-participantendpoint.md) 和 [serviceEndpoint](callrecords-serviceendpoint.md) 类型继承自此类型。</span><span class="sxs-lookup"><span data-stu-id="e1db9-106">The endpoint could be a user's device, a meeting, an application/bot, etc. The [participantEndpoint](callrecords-participantendpoint.md) and [serviceEndpoint](callrecords-serviceendpoint.md) types inherit from this type.</span></span>

## <a name="properties"></a><span data-ttu-id="e1db9-107">属性</span><span class="sxs-lookup"><span data-stu-id="e1db9-107">Properties</span></span>

| <span data-ttu-id="e1db9-108">属性</span><span class="sxs-lookup"><span data-stu-id="e1db9-108">Property</span></span>     | <span data-ttu-id="e1db9-109">类型</span><span class="sxs-lookup"><span data-stu-id="e1db9-109">Type</span></span>        | <span data-ttu-id="e1db9-110">说明</span><span class="sxs-lookup"><span data-stu-id="e1db9-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e1db9-111">userAgent</span><span class="sxs-lookup"><span data-stu-id="e1db9-111">userAgent</span></span>|[<span data-ttu-id="e1db9-112">callRecords。 userAgent</span><span class="sxs-lookup"><span data-stu-id="e1db9-112">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="e1db9-113">此终结点报告的用户代理。</span><span class="sxs-lookup"><span data-stu-id="e1db9-113">User-agent reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1db9-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1db9-114">JSON representation</span></span>

<span data-ttu-id="e1db9-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1db9-115">The following is a JSON representation of the resource.</span></span>

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
