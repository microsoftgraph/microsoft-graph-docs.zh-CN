---
title: participantEndpoint 资源类型
description: ParticipantEndpoint 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ff590acb76d50da9d0772bdaece805a1db0cd26a
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492021"
---
# <a name="participantendpoint-resource-type"></a><span data-ttu-id="10f68-103">participantEndpoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="10f68-103">participantEndpoint resource type</span></span>

<span data-ttu-id="10f68-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="10f68-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="10f68-105">表示呼叫中的参与者终结点。</span><span class="sxs-lookup"><span data-stu-id="10f68-105">Represents an participant endpoint in a call.</span></span> <span data-ttu-id="10f68-106">终结点表示用户或用户-like 实体。</span><span class="sxs-lookup"><span data-stu-id="10f68-106">The endpoint represents a user or user-like entity.</span></span> <span data-ttu-id="10f68-107">从[终结点](callrecords-endpoint.md)类型继承。</span><span class="sxs-lookup"><span data-stu-id="10f68-107">Inherits from [endpoint](callrecords-endpoint.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="10f68-108">属性</span><span class="sxs-lookup"><span data-stu-id="10f68-108">Properties</span></span>

| <span data-ttu-id="10f68-109">属性</span><span class="sxs-lookup"><span data-stu-id="10f68-109">Property</span></span>     | <span data-ttu-id="10f68-110">类型</span><span class="sxs-lookup"><span data-stu-id="10f68-110">Type</span></span>        | <span data-ttu-id="10f68-111">Description</span><span class="sxs-lookup"><span data-stu-id="10f68-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="10f68-112">userAgent</span><span class="sxs-lookup"><span data-stu-id="10f68-112">userAgent</span></span>|[<span data-ttu-id="10f68-113">callRecords。 userAgent</span><span class="sxs-lookup"><span data-stu-id="10f68-113">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="10f68-114">此终结点报告的用户代理。</span><span class="sxs-lookup"><span data-stu-id="10f68-114">User-agent reported by this endpoint.</span></span>|
|<span data-ttu-id="10f68-115">反馈</span><span class="sxs-lookup"><span data-stu-id="10f68-115">feedback</span></span>|[<span data-ttu-id="10f68-116">callRecords。 userFeedback</span><span class="sxs-lookup"><span data-stu-id="10f68-116">microsoft.graph.callRecords.userFeedback</span></span>](callrecords-userfeedback.md)|<span data-ttu-id="10f68-117">此终结点的用户提供的有关会话质量的反馈。</span><span class="sxs-lookup"><span data-stu-id="10f68-117">The feedback provided by the user of this endpoint about the quality of the session.</span></span>|
|<span data-ttu-id="10f68-118">窃取</span><span class="sxs-lookup"><span data-stu-id="10f68-118">identity</span></span>|[<span data-ttu-id="10f68-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="10f68-119">identitySet</span></span>](identityset.md)|<span data-ttu-id="10f68-120">与终结点关联的标识。</span><span class="sxs-lookup"><span data-stu-id="10f68-120">Identity associated with the endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10f68-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10f68-121">JSON representation</span></span>

<span data-ttu-id="10f68-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10f68-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.participantEndpoint",
  "baseType": "microsoft.graph.callRecords.endpoint"
}-->

```json
{
  "userAgent": {"@odata.type": "microsoft.graph.callRecords.userAgent"},
  "feedback": {"@odata.type": "microsoft.graph.callRecords.userFeedback"},
  "identity": {"@odata.type": "microsoft.graph.identitySet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->