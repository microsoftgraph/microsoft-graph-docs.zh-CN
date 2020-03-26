---
title: incomingContext 资源类型
description: 代表与传入呼叫相关联的上下文。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6acd1928b223789df7580a5f74eefc723570ca93
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962540"
---
# <a name="incomingcontext-resource-type"></a><span data-ttu-id="b981f-103">incomingContext 资源类型</span><span class="sxs-lookup"><span data-stu-id="b981f-103">incomingContext resource type</span></span>

<span data-ttu-id="b981f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b981f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b981f-105">代表与传入呼叫相关联的上下文。</span><span class="sxs-lookup"><span data-stu-id="b981f-105">Represents the context associated with an incoming call.</span></span>

## <a name="properties"></a><span data-ttu-id="b981f-106">属性</span><span class="sxs-lookup"><span data-stu-id="b981f-106">Properties</span></span>

| <span data-ttu-id="b981f-107">属性</span><span class="sxs-lookup"><span data-stu-id="b981f-107">Property</span></span>              | <span data-ttu-id="b981f-108">类型</span><span class="sxs-lookup"><span data-stu-id="b981f-108">Type</span></span>                          | <span data-ttu-id="b981f-109">说明</span><span class="sxs-lookup"><span data-stu-id="b981f-109">Description</span></span>                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| <span data-ttu-id="b981f-110">sourceParticipantId</span><span class="sxs-lookup"><span data-stu-id="b981f-110">sourceParticipantId</span></span>   | <span data-ttu-id="b981f-111">String</span><span class="sxs-lookup"><span data-stu-id="b981f-111">String</span></span>                        | <span data-ttu-id="b981f-112">触发传入呼叫的参与者的 ID。</span><span class="sxs-lookup"><span data-stu-id="b981f-112">The ID of the participant that triggered the incoming call.</span></span> <span data-ttu-id="b981f-113">只读。</span><span class="sxs-lookup"><span data-stu-id="b981f-113">Read-only.</span></span>  |
| <span data-ttu-id="b981f-114">observedParticipantId</span><span class="sxs-lookup"><span data-stu-id="b981f-114">observedParticipantId</span></span> | <span data-ttu-id="b981f-115">String</span><span class="sxs-lookup"><span data-stu-id="b981f-115">String</span></span>                        | <span data-ttu-id="b981f-116">正在观察的参与者的 ID。</span><span class="sxs-lookup"><span data-stu-id="b981f-116">The ID of the participant that is under observation.</span></span> <span data-ttu-id="b981f-117">只读。</span><span class="sxs-lookup"><span data-stu-id="b981f-117">Read-only.</span></span>         |
| <span data-ttu-id="b981f-118">onBehalfOf</span><span class="sxs-lookup"><span data-stu-id="b981f-118">onBehalfOf</span></span>            | [<span data-ttu-id="b981f-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="b981f-119">identitySet</span></span>](identityset.md) | <span data-ttu-id="b981f-120">代表调用所发生的标识。</span><span class="sxs-lookup"><span data-stu-id="b981f-120">The identity that the call is happening on behalf of.</span></span>                   |
| <span data-ttu-id="b981f-121">transferor</span><span class="sxs-lookup"><span data-stu-id="b981f-121">transferor</span></span>            | [<span data-ttu-id="b981f-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="b981f-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="b981f-123">转接呼叫的标识。</span><span class="sxs-lookup"><span data-stu-id="b981f-123">The identity that transferred the call.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="b981f-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b981f-124">JSON representation</span></span>

<span data-ttu-id="b981f-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b981f-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "sourceParticipantId",
    "observedParticipantId",
    "onBehalfOf",
    "transferor"
  ],
  "@odata.type": "microsoft.graph.incomingContext"
}-->
```json
{
  "sourceParticipantId": "String",
  "observedParticipantId": "String",
  "onBehalfOf": {"@odata.type": "#microsoft.graph.identitySet"},
  "transferor": {"@odata.type": "#microsoft.graph.identitySet"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "incomingContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
