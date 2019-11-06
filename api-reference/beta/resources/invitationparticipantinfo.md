---
title: invitationParticipantInfo 资源类型
description: '**InvitationParticipant**用于表示与对话邀请关联的一组标识，并提供其他邀请参数。'
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7e25e65fb87f664788b0649f188def29b62c13d2
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006689"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="88a4e-103">invitationParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="88a4e-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88a4e-104">此资源用于表示与对话邀请关联的一组标识，并提供其他邀请参数。</span><span class="sxs-lookup"><span data-stu-id="88a4e-104">This resource is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="88a4e-105">属性</span><span class="sxs-lookup"><span data-stu-id="88a4e-105">Properties</span></span>

| <span data-ttu-id="88a4e-106">属性</span><span class="sxs-lookup"><span data-stu-id="88a4e-106">Property</span></span>                           | <span data-ttu-id="88a4e-107">类型</span><span class="sxs-lookup"><span data-stu-id="88a4e-107">Type</span></span>                          | <span data-ttu-id="88a4e-108">说明</span><span class="sxs-lookup"><span data-stu-id="88a4e-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="88a4e-109">endpointType</span><span class="sxs-lookup"><span data-stu-id="88a4e-109">endpointType</span></span>                       | <span data-ttu-id="88a4e-110">String</span><span class="sxs-lookup"><span data-stu-id="88a4e-110">String</span></span>                        | <span data-ttu-id="88a4e-111">终结点的类型。</span><span class="sxs-lookup"><span data-stu-id="88a4e-111">The type of endpoint.</span></span> <span data-ttu-id="88a4e-112">可取值为：`default`、`voicemail`。</span><span class="sxs-lookup"><span data-stu-id="88a4e-112">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="88a4e-113">窃取</span><span class="sxs-lookup"><span data-stu-id="88a4e-113">identity</span></span>                           | [<span data-ttu-id="88a4e-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="88a4e-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="88a4e-115">与此邀请关联的[了解 identityset](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="88a4e-115">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="88a4e-116">languageId</span><span class="sxs-lookup"><span data-stu-id="88a4e-116">languageId</span></span>                         | <span data-ttu-id="88a4e-117">String</span><span class="sxs-lookup"><span data-stu-id="88a4e-117">String</span></span>                        | <span data-ttu-id="88a4e-118">语言区域性字符串。</span><span class="sxs-lookup"><span data-stu-id="88a4e-118">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="88a4e-119">范围</span><span class="sxs-lookup"><span data-stu-id="88a4e-119">region</span></span>                             | <span data-ttu-id="88a4e-120">String</span><span class="sxs-lookup"><span data-stu-id="88a4e-120">String</span></span>                        | <span data-ttu-id="88a4e-121">参与者的地区。</span><span class="sxs-lookup"><span data-stu-id="88a4e-121">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="88a4e-122">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="88a4e-122">replacesCallId</span></span>                     | <span data-ttu-id="88a4e-123">String</span><span class="sxs-lookup"><span data-stu-id="88a4e-123">String</span></span>                        | <span data-ttu-id="88a4e-124">可选。</span><span class="sxs-lookup"><span data-stu-id="88a4e-124">Optional.</span></span> <span data-ttu-id="88a4e-125">目标 idenity 当前是其一部分的调用。</span><span class="sxs-lookup"><span data-stu-id="88a4e-125">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="88a4e-126">添加参与者后，将删除此呼叫。</span><span class="sxs-lookup"><span data-stu-id="88a4e-126">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="88a4e-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88a4e-127">JSON representation</span></span>

<span data-ttu-id="88a4e-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88a4e-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "languageId": "String",
  "region": "String",
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
