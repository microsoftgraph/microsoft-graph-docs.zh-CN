---
title: incomingContext 资源类型
description: 与传入呼叫相关联的上下文。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0afe972be631a2048b2a1970b1fda41e8cb72920
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636895"
---
# <a name="incomingcontext-resource-type"></a><span data-ttu-id="ac4bc-103">incomingContext 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac4bc-103">incomingContext resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac4bc-104">与传入呼叫相关联的上下文。</span><span class="sxs-lookup"><span data-stu-id="ac4bc-104">The context associated with an incoming call.</span></span>

## <a name="properties"></a><span data-ttu-id="ac4bc-105">属性</span><span class="sxs-lookup"><span data-stu-id="ac4bc-105">Properties</span></span>

| <span data-ttu-id="ac4bc-106">属性</span><span class="sxs-lookup"><span data-stu-id="ac4bc-106">Property</span></span>              | <span data-ttu-id="ac4bc-107">类型</span><span class="sxs-lookup"><span data-stu-id="ac4bc-107">Type</span></span>                          | <span data-ttu-id="ac4bc-108">说明</span><span class="sxs-lookup"><span data-stu-id="ac4bc-108">Description</span></span>                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| <span data-ttu-id="ac4bc-109">observedParticipantId</span><span class="sxs-lookup"><span data-stu-id="ac4bc-109">observedParticipantId</span></span> | <span data-ttu-id="ac4bc-110">String</span><span class="sxs-lookup"><span data-stu-id="ac4bc-110">String</span></span>                        | <span data-ttu-id="ac4bc-111">正在观察的参与者的 id。</span><span class="sxs-lookup"><span data-stu-id="ac4bc-111">The id of the participant that is under observation.</span></span> <span data-ttu-id="ac4bc-112">只读。</span><span class="sxs-lookup"><span data-stu-id="ac4bc-112">Read-only.</span></span>         |
| <span data-ttu-id="ac4bc-113">onBehalfOf</span><span class="sxs-lookup"><span data-stu-id="ac4bc-113">onBehalfOf</span></span>            | [<span data-ttu-id="ac4bc-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="ac4bc-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="ac4bc-115">代表调用所发生的标识。</span><span class="sxs-lookup"><span data-stu-id="ac4bc-115">The identity that the call is happening on behalf of.</span></span>                   |
| <span data-ttu-id="ac4bc-116">sourceParticipantId</span><span class="sxs-lookup"><span data-stu-id="ac4bc-116">sourceParticipantId</span></span>   | <span data-ttu-id="ac4bc-117">String</span><span class="sxs-lookup"><span data-stu-id="ac4bc-117">String</span></span>                        | <span data-ttu-id="ac4bc-118">触发传入呼叫的参与者的 id。</span><span class="sxs-lookup"><span data-stu-id="ac4bc-118">The id of the participant that triggered the incoming call.</span></span> <span data-ttu-id="ac4bc-119">只读。</span><span class="sxs-lookup"><span data-stu-id="ac4bc-119">Read-only.</span></span>  |
| <span data-ttu-id="ac4bc-120">transferor</span><span class="sxs-lookup"><span data-stu-id="ac4bc-120">transferor</span></span>            | [<span data-ttu-id="ac4bc-121">identitySet</span><span class="sxs-lookup"><span data-stu-id="ac4bc-121">identitySet</span></span>](identityset.md) | <span data-ttu-id="ac4bc-122">转接呼叫的标识。</span><span class="sxs-lookup"><span data-stu-id="ac4bc-122">The identity that transferred the call.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="ac4bc-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac4bc-123">JSON representation</span></span>

<span data-ttu-id="ac4bc-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac4bc-124">The following is a JSON representation of the resource.</span></span>

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
