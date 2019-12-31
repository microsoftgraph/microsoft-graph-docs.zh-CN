---
title: invitationParticipantInfo 资源类型
description: '**InvitationParticipant**用于表示与对话邀请关联的一组标识，并提供其他邀请参数。'
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8b42e89f89332e58fa2f7edcf39c774446c6b9d9
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913399"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="5d17c-103">invitationParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="5d17c-103">invitationParticipantInfo resource type</span></span>

<span data-ttu-id="5d17c-104">此资源用于表示受邀加入组呼叫的实体。</span><span class="sxs-lookup"><span data-stu-id="5d17c-104">This resource is used to represent the entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="5d17c-105">属性</span><span class="sxs-lookup"><span data-stu-id="5d17c-105">Properties</span></span>

| <span data-ttu-id="5d17c-106">属性</span><span class="sxs-lookup"><span data-stu-id="5d17c-106">Property</span></span>                           | <span data-ttu-id="5d17c-107">类型</span><span class="sxs-lookup"><span data-stu-id="5d17c-107">Type</span></span>                          | <span data-ttu-id="5d17c-108">说明</span><span class="sxs-lookup"><span data-stu-id="5d17c-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="5d17c-109">窃取</span><span class="sxs-lookup"><span data-stu-id="5d17c-109">identity</span></span>                           | [<span data-ttu-id="5d17c-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="5d17c-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="5d17c-111">与此邀请关联的[了解 identityset](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="5d17c-111">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="5d17c-112">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="5d17c-112">replacesCallId</span></span>                     | <span data-ttu-id="5d17c-113">String</span><span class="sxs-lookup"><span data-stu-id="5d17c-113">String</span></span>                        | <span data-ttu-id="5d17c-114">可选。</span><span class="sxs-lookup"><span data-stu-id="5d17c-114">Optional.</span></span> <span data-ttu-id="5d17c-115">目标标识当前是其一部分的调用。</span><span class="sxs-lookup"><span data-stu-id="5d17c-115">The call which the target identity is currently a part of.</span></span> <span data-ttu-id="5d17c-116">添加参与者后，将删除此呼叫。</span><span class="sxs-lookup"><span data-stu-id="5d17c-116">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5d17c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5d17c-117">JSON representation</span></span>

<span data-ttu-id="5d17c-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d17c-118">The following is a JSON representation of the resource.</span></span>

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
