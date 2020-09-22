---
title: incomingContext 资源类型
description: 与来电相关的上下文。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fdbaaadc55877aee89f7ea984d60818cbbad0814
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016559"
---
# <a name="incomingcontext-resource-type"></a><span data-ttu-id="f37e9-103">incomingContext 资源类型</span><span class="sxs-lookup"><span data-stu-id="f37e9-103">incomingContext resource type</span></span>

<span data-ttu-id="f37e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f37e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f37e9-105">与来电相关的上下文。</span><span class="sxs-lookup"><span data-stu-id="f37e9-105">The context associated with an incoming call.</span></span>

## <a name="properties"></a><span data-ttu-id="f37e9-106">属性</span><span class="sxs-lookup"><span data-stu-id="f37e9-106">Properties</span></span>

| <span data-ttu-id="f37e9-107">属性</span><span class="sxs-lookup"><span data-stu-id="f37e9-107">Property</span></span>              | <span data-ttu-id="f37e9-108">类型</span><span class="sxs-lookup"><span data-stu-id="f37e9-108">Type</span></span>                          | <span data-ttu-id="f37e9-109">说明</span><span class="sxs-lookup"><span data-stu-id="f37e9-109">Description</span></span>                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| <span data-ttu-id="f37e9-110">observedParticipantId</span><span class="sxs-lookup"><span data-stu-id="f37e9-110">observedParticipantId</span></span> | <span data-ttu-id="f37e9-111">String</span><span class="sxs-lookup"><span data-stu-id="f37e9-111">String</span></span>                        | <span data-ttu-id="f37e9-112">正在观察的参与者的 id。</span><span class="sxs-lookup"><span data-stu-id="f37e9-112">The id of the participant that is under observation.</span></span> <span data-ttu-id="f37e9-113">只读。</span><span class="sxs-lookup"><span data-stu-id="f37e9-113">Read-only.</span></span>         |
| <span data-ttu-id="f37e9-114">onBehalfOf</span><span class="sxs-lookup"><span data-stu-id="f37e9-114">onBehalfOf</span></span>            | [<span data-ttu-id="f37e9-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="f37e9-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="f37e9-116">代表调用所发生的标识。</span><span class="sxs-lookup"><span data-stu-id="f37e9-116">The identity that the call is happening on behalf of.</span></span>                   |
| <span data-ttu-id="f37e9-117">sourceParticipantId</span><span class="sxs-lookup"><span data-stu-id="f37e9-117">sourceParticipantId</span></span>   | <span data-ttu-id="f37e9-118">String</span><span class="sxs-lookup"><span data-stu-id="f37e9-118">String</span></span>                        | <span data-ttu-id="f37e9-119">触发传入呼叫的参与者的 id。</span><span class="sxs-lookup"><span data-stu-id="f37e9-119">The id of the participant that triggered the incoming call.</span></span> <span data-ttu-id="f37e9-120">只读。</span><span class="sxs-lookup"><span data-stu-id="f37e9-120">Read-only.</span></span>  |
| <span data-ttu-id="f37e9-121">transferor</span><span class="sxs-lookup"><span data-stu-id="f37e9-121">transferor</span></span>            | [<span data-ttu-id="f37e9-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="f37e9-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="f37e9-123">转接呼叫的标识。</span><span class="sxs-lookup"><span data-stu-id="f37e9-123">The identity that transferred the call.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="f37e9-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f37e9-124">JSON representation</span></span>

<span data-ttu-id="f37e9-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f37e9-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "observedParticipantId",
    "onBehalfOf",
    "transferor"
  ],
  "@odata.type": "microsoft.graph.incomingContext"
}-->
```json
{
  "observedParticipantId": "String",
  "onBehalfOf": {"@odata.type": "#microsoft.graph.identitySet"},
  "sourceParticipantId": "String",
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


