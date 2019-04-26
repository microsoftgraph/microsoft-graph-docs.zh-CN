---
title: invitationParticipantInfo 资源类型
description: '**InvitationParticipant**用于表示与对话邀请关联的一组标识, 并提供其他邀请参数。'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb20dde1a74472695755e65dc404a6709f79c8b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569961"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="c346b-103">invitationParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="c346b-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c346b-104">**InvitationParticipant**用于表示与对话邀请关联的一组标识, 并提供其他邀请参数。</span><span class="sxs-lookup"><span data-stu-id="c346b-104">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="c346b-105">属性</span><span class="sxs-lookup"><span data-stu-id="c346b-105">Properties</span></span>

| <span data-ttu-id="c346b-106">属性</span><span class="sxs-lookup"><span data-stu-id="c346b-106">Property</span></span>                           | <span data-ttu-id="c346b-107">类型</span><span class="sxs-lookup"><span data-stu-id="c346b-107">Type</span></span>                          | <span data-ttu-id="c346b-108">说明</span><span class="sxs-lookup"><span data-stu-id="c346b-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="c346b-109">endpointType</span><span class="sxs-lookup"><span data-stu-id="c346b-109">endpointType</span></span>                       | <span data-ttu-id="c346b-110">String</span><span class="sxs-lookup"><span data-stu-id="c346b-110">String</span></span>                        | <span data-ttu-id="c346b-111">可取值为：`default`、`voicemail`。</span><span class="sxs-lookup"><span data-stu-id="c346b-111">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="c346b-112">窃取</span><span class="sxs-lookup"><span data-stu-id="c346b-112">identity</span></span>                           | [<span data-ttu-id="c346b-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="c346b-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="c346b-114">与此邀请关联的[了解 identityset](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="c346b-114">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="c346b-115">languageId</span><span class="sxs-lookup"><span data-stu-id="c346b-115">languageId</span></span>                         | <span data-ttu-id="c346b-116">String</span><span class="sxs-lookup"><span data-stu-id="c346b-116">String</span></span>                        | <span data-ttu-id="c346b-117">语言区域性字符串。</span><span class="sxs-lookup"><span data-stu-id="c346b-117">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="c346b-118">范围</span><span class="sxs-lookup"><span data-stu-id="c346b-118">region</span></span>                             | <span data-ttu-id="c346b-119">String</span><span class="sxs-lookup"><span data-stu-id="c346b-119">String</span></span>                        | <span data-ttu-id="c346b-120">参与者的地区。</span><span class="sxs-lookup"><span data-stu-id="c346b-120">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="c346b-121">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="c346b-121">replacesCallId</span></span>                     | <span data-ttu-id="c346b-122">字符串</span><span class="sxs-lookup"><span data-stu-id="c346b-122">String</span></span>                        | <span data-ttu-id="c346b-123">可选。</span><span class="sxs-lookup"><span data-stu-id="c346b-123">Optional.</span></span> <span data-ttu-id="c346b-124">目标 idenity 当前是其一部分的调用。</span><span class="sxs-lookup"><span data-stu-id="c346b-124">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="c346b-125">添加参与者后, 将删除此呼叫。</span><span class="sxs-lookup"><span data-stu-id="c346b-125">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c346b-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c346b-126">JSON representation</span></span>

<span data-ttu-id="c346b-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c346b-127">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/invitationparticipantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
