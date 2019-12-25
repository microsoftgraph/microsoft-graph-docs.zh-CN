---
title: invitationParticipantInfo 资源类型
description: 表示受邀加入组呼叫的实体。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bddce0358bfa0ec46d8231958817002cb4ca8c20
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870220"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="93717-103">invitationParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="93717-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93717-104">表示受邀加入组呼叫的实体。</span><span class="sxs-lookup"><span data-stu-id="93717-104">Represents an entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="93717-105">属性</span><span class="sxs-lookup"><span data-stu-id="93717-105">Properties</span></span>

| <span data-ttu-id="93717-106">属性</span><span class="sxs-lookup"><span data-stu-id="93717-106">Property</span></span>                           | <span data-ttu-id="93717-107">类型</span><span class="sxs-lookup"><span data-stu-id="93717-107">Type</span></span>                          | <span data-ttu-id="93717-108">说明</span><span class="sxs-lookup"><span data-stu-id="93717-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="93717-109">endpointType</span><span class="sxs-lookup"><span data-stu-id="93717-109">endpointType</span></span>                       | <span data-ttu-id="93717-110">String</span><span class="sxs-lookup"><span data-stu-id="93717-110">String</span></span>                        | <span data-ttu-id="93717-111">终结点的类型。</span><span class="sxs-lookup"><span data-stu-id="93717-111">The type of endpoint.</span></span> <span data-ttu-id="93717-112">可取值为：`default`、`voicemail`。</span><span class="sxs-lookup"><span data-stu-id="93717-112">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="93717-113">窃取</span><span class="sxs-lookup"><span data-stu-id="93717-113">identity</span></span>                           | [<span data-ttu-id="93717-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="93717-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="93717-115">与此邀请关联的[了解 identityset](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="93717-115">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="93717-116">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="93717-116">replacesCallId</span></span>                     | <span data-ttu-id="93717-117">String</span><span class="sxs-lookup"><span data-stu-id="93717-117">String</span></span>                        | <span data-ttu-id="93717-118">可选。</span><span class="sxs-lookup"><span data-stu-id="93717-118">Optional.</span></span> <span data-ttu-id="93717-119">目标 idenity 当前是其一部分的调用。</span><span class="sxs-lookup"><span data-stu-id="93717-119">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="93717-120">添加参与者后，将删除此呼叫。</span><span class="sxs-lookup"><span data-stu-id="93717-120">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="93717-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93717-121">JSON representation</span></span>

<span data-ttu-id="93717-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93717-122">The following is a JSON representation of the resource.</span></span>

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
