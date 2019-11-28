---
title: invitationParticipantInfo 资源类型
description: '**InvitationParticipant**用于表示与对话邀请关联的一组标识，并提供其他邀请参数。'
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 762e5dc75c03cda78581b90b54c3fea27a7f12f2
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636665"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="61f88-103">invitationParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="61f88-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61f88-104">此资源用于表示与对话邀请关联的一组标识，并提供其他邀请参数。</span><span class="sxs-lookup"><span data-stu-id="61f88-104">This resource is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="61f88-105">属性</span><span class="sxs-lookup"><span data-stu-id="61f88-105">Properties</span></span>

| <span data-ttu-id="61f88-106">属性</span><span class="sxs-lookup"><span data-stu-id="61f88-106">Property</span></span>                           | <span data-ttu-id="61f88-107">类型</span><span class="sxs-lookup"><span data-stu-id="61f88-107">Type</span></span>                          | <span data-ttu-id="61f88-108">说明</span><span class="sxs-lookup"><span data-stu-id="61f88-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="61f88-109">endpointType</span><span class="sxs-lookup"><span data-stu-id="61f88-109">endpointType</span></span>                       | <span data-ttu-id="61f88-110">String</span><span class="sxs-lookup"><span data-stu-id="61f88-110">String</span></span>                        | <span data-ttu-id="61f88-111">终结点的类型。</span><span class="sxs-lookup"><span data-stu-id="61f88-111">The type of endpoint.</span></span> <span data-ttu-id="61f88-112">可取值为：`default`、`voicemail`。</span><span class="sxs-lookup"><span data-stu-id="61f88-112">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="61f88-113">窃取</span><span class="sxs-lookup"><span data-stu-id="61f88-113">identity</span></span>                           | [<span data-ttu-id="61f88-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="61f88-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="61f88-115">与此邀请关联的[了解 identityset](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="61f88-115">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="61f88-116">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="61f88-116">replacesCallId</span></span>                     | <span data-ttu-id="61f88-117">String</span><span class="sxs-lookup"><span data-stu-id="61f88-117">String</span></span>                        | <span data-ttu-id="61f88-118">可选。</span><span class="sxs-lookup"><span data-stu-id="61f88-118">Optional.</span></span> <span data-ttu-id="61f88-119">目标 idenity 当前是其一部分的调用。</span><span class="sxs-lookup"><span data-stu-id="61f88-119">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="61f88-120">添加参与者后，将删除此呼叫。</span><span class="sxs-lookup"><span data-stu-id="61f88-120">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="61f88-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61f88-121">JSON representation</span></span>

<span data-ttu-id="61f88-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61f88-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "endpointType",
    "replacesCallId"
  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "replacesCallId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
