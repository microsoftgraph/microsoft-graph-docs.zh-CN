---
title: incomingContext 资源类型
description: 与来电相关的上下文。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a7eba09d18b2b60c3a5ae45a8ad335d8971d2c77
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496374"
---
# <a name="incomingcontext-resource-type"></a><span data-ttu-id="2a838-103">incomingContext 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a838-103">incomingContext resource type</span></span>

<span data-ttu-id="2a838-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2a838-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a838-105">与来电相关的上下文。</span><span class="sxs-lookup"><span data-stu-id="2a838-105">The context associated with an incoming call.</span></span>

## <a name="properties"></a><span data-ttu-id="2a838-106">属性</span><span class="sxs-lookup"><span data-stu-id="2a838-106">Properties</span></span>

| <span data-ttu-id="2a838-107">属性</span><span class="sxs-lookup"><span data-stu-id="2a838-107">Property</span></span>              | <span data-ttu-id="2a838-108">类型</span><span class="sxs-lookup"><span data-stu-id="2a838-108">Type</span></span>                          | <span data-ttu-id="2a838-109">说明</span><span class="sxs-lookup"><span data-stu-id="2a838-109">Description</span></span>                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| <span data-ttu-id="2a838-110">observedParticipantId</span><span class="sxs-lookup"><span data-stu-id="2a838-110">observedParticipantId</span></span> | <span data-ttu-id="2a838-111">String</span><span class="sxs-lookup"><span data-stu-id="2a838-111">String</span></span>                        | <span data-ttu-id="2a838-112">正在观察的参与者的 id。</span><span class="sxs-lookup"><span data-stu-id="2a838-112">The id of the participant that is under observation.</span></span> <span data-ttu-id="2a838-113">只读。</span><span class="sxs-lookup"><span data-stu-id="2a838-113">Read-only.</span></span>         |
| <span data-ttu-id="2a838-114">onBehalfOf</span><span class="sxs-lookup"><span data-stu-id="2a838-114">onBehalfOf</span></span>            | [<span data-ttu-id="2a838-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="2a838-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="2a838-116">代表调用所发生的标识。</span><span class="sxs-lookup"><span data-stu-id="2a838-116">The identity that the call is happening on behalf of.</span></span>                   |
| <span data-ttu-id="2a838-117">sourceParticipantId</span><span class="sxs-lookup"><span data-stu-id="2a838-117">sourceParticipantId</span></span>   | <span data-ttu-id="2a838-118">String</span><span class="sxs-lookup"><span data-stu-id="2a838-118">String</span></span>                        | <span data-ttu-id="2a838-119">触发传入呼叫的参与者的 id。</span><span class="sxs-lookup"><span data-stu-id="2a838-119">The id of the participant that triggered the incoming call.</span></span> <span data-ttu-id="2a838-120">只读。</span><span class="sxs-lookup"><span data-stu-id="2a838-120">Read-only.</span></span>  |
| <span data-ttu-id="2a838-121">transferor</span><span class="sxs-lookup"><span data-stu-id="2a838-121">transferor</span></span>            | [<span data-ttu-id="2a838-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="2a838-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="2a838-123">转接呼叫的标识。</span><span class="sxs-lookup"><span data-stu-id="2a838-123">The identity that transferred the call.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="2a838-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a838-124">JSON representation</span></span>

<span data-ttu-id="2a838-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a838-125">The following is a JSON representation of the resource.</span></span>

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
