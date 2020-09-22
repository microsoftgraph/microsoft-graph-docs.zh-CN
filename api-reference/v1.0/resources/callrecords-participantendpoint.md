---
title: participantEndpoint 资源类型
description: ParticipantEndpoint 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b425deeea49780ee752e8ace04078f3d1d6160a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069342"
---
# <a name="participantendpoint-resource-type"></a><span data-ttu-id="4ae48-103">participantEndpoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ae48-103">participantEndpoint resource type</span></span>

<span data-ttu-id="4ae48-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="4ae48-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="4ae48-105">表示呼叫中的参与者终结点。</span><span class="sxs-lookup"><span data-stu-id="4ae48-105">Represents an participant endpoint in a call.</span></span> <span data-ttu-id="4ae48-106">终结点表示用户或用户-like 实体。</span><span class="sxs-lookup"><span data-stu-id="4ae48-106">The endpoint represents a user or user-like entity.</span></span> <span data-ttu-id="4ae48-107">从 [终结点](callrecords-endpoint.md) 类型继承。</span><span class="sxs-lookup"><span data-stu-id="4ae48-107">Inherits from [endpoint](callrecords-endpoint.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="4ae48-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ae48-108">Properties</span></span>

| <span data-ttu-id="4ae48-109">属性</span><span class="sxs-lookup"><span data-stu-id="4ae48-109">Property</span></span>     | <span data-ttu-id="4ae48-110">类型</span><span class="sxs-lookup"><span data-stu-id="4ae48-110">Type</span></span>        | <span data-ttu-id="4ae48-111">说明</span><span class="sxs-lookup"><span data-stu-id="4ae48-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4ae48-112">userAgent</span><span class="sxs-lookup"><span data-stu-id="4ae48-112">userAgent</span></span>|[<span data-ttu-id="4ae48-113">callRecords。 userAgent</span><span class="sxs-lookup"><span data-stu-id="4ae48-113">microsoft.graph.callRecords.userAgent</span></span>](callrecords-useragent.md)|<span data-ttu-id="4ae48-114">此终结点报告的用户代理。</span><span class="sxs-lookup"><span data-stu-id="4ae48-114">User-agent reported by this endpoint.</span></span>|
|<span data-ttu-id="4ae48-115">反馈</span><span class="sxs-lookup"><span data-stu-id="4ae48-115">feedback</span></span>|[<span data-ttu-id="4ae48-116">callRecords。 userFeedback</span><span class="sxs-lookup"><span data-stu-id="4ae48-116">microsoft.graph.callRecords.userFeedback</span></span>](callrecords-userfeedback.md)|<span data-ttu-id="4ae48-117">此终结点的用户提供的有关会话质量的反馈。</span><span class="sxs-lookup"><span data-stu-id="4ae48-117">The feedback provided by the user of this endpoint about the quality of the session.</span></span>|
|<span data-ttu-id="4ae48-118">窃取</span><span class="sxs-lookup"><span data-stu-id="4ae48-118">identity</span></span>|[<span data-ttu-id="4ae48-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="4ae48-119">identitySet</span></span>](identityset.md)|<span data-ttu-id="4ae48-120">与终结点关联的标识。</span><span class="sxs-lookup"><span data-stu-id="4ae48-120">Identity associated with the endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ae48-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ae48-121">JSON representation</span></span>

<span data-ttu-id="4ae48-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ae48-122">The following is a JSON representation of the resource.</span></span>

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
