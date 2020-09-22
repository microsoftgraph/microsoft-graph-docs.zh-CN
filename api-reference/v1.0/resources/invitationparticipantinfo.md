---
title: invitationParticipantInfo 资源类型
description: '**InvitationParticipant**用于表示与对话邀请关联的一组标识，并提供其他邀请参数。'
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2425f7ebd6ac516a9100605c9ebfe47f1b87a114
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984248"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="ef33a-103">invitationParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="ef33a-103">invitationParticipantInfo resource type</span></span>

<span data-ttu-id="ef33a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef33a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ef33a-105">此资源用于表示受邀加入组呼叫的实体。</span><span class="sxs-lookup"><span data-stu-id="ef33a-105">This resource is used to represent the entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="ef33a-106">属性</span><span class="sxs-lookup"><span data-stu-id="ef33a-106">Properties</span></span>

| <span data-ttu-id="ef33a-107">属性</span><span class="sxs-lookup"><span data-stu-id="ef33a-107">Property</span></span>                           | <span data-ttu-id="ef33a-108">类型</span><span class="sxs-lookup"><span data-stu-id="ef33a-108">Type</span></span>                          | <span data-ttu-id="ef33a-109">说明</span><span class="sxs-lookup"><span data-stu-id="ef33a-109">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="ef33a-110">窃取</span><span class="sxs-lookup"><span data-stu-id="ef33a-110">identity</span></span>                           | [<span data-ttu-id="ef33a-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="ef33a-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="ef33a-112">与此邀请关联的 [了解 identityset](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="ef33a-112">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="ef33a-113">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="ef33a-113">replacesCallId</span></span>                     | <span data-ttu-id="ef33a-114">String</span><span class="sxs-lookup"><span data-stu-id="ef33a-114">String</span></span>                        | <span data-ttu-id="ef33a-115">可选。</span><span class="sxs-lookup"><span data-stu-id="ef33a-115">Optional.</span></span> <span data-ttu-id="ef33a-116">目标标识当前是其一部分的调用。</span><span class="sxs-lookup"><span data-stu-id="ef33a-116">The call which the target identity is currently a part of.</span></span> <span data-ttu-id="ef33a-117">添加参与者后，将删除此呼叫。</span><span class="sxs-lookup"><span data-stu-id="ef33a-117">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ef33a-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ef33a-118">JSON representation</span></span>

<span data-ttu-id="ef33a-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef33a-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "replacesCallId"
  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
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

