---
title: invitationParticipantInfo 资源类型
description: '**InvitationParticipant**用于表示一组标识相关联的对话邀请，并提供其他邀请参数。'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 666de597d40570a567ea88a375ab15d1e5f09038
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573597"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="3f636-103">invitationParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f636-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f636-104">**InvitationParticipant**用于表示一组标识相关联的对话邀请，并提供其他邀请参数。</span><span class="sxs-lookup"><span data-stu-id="3f636-104">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="3f636-105">属性</span><span class="sxs-lookup"><span data-stu-id="3f636-105">Properties</span></span>

| <span data-ttu-id="3f636-106">属性</span><span class="sxs-lookup"><span data-stu-id="3f636-106">Property</span></span>                           | <span data-ttu-id="3f636-107">类型</span><span class="sxs-lookup"><span data-stu-id="3f636-107">Type</span></span>                          | <span data-ttu-id="3f636-108">说明</span><span class="sxs-lookup"><span data-stu-id="3f636-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="3f636-109">endpointType</span><span class="sxs-lookup"><span data-stu-id="3f636-109">endpointType</span></span>                       | <span data-ttu-id="3f636-110">operationStatus</span><span class="sxs-lookup"><span data-stu-id="3f636-110">operationStatus</span></span>               | <span data-ttu-id="3f636-111">可取值为：`default`、`voicemail`。</span><span class="sxs-lookup"><span data-stu-id="3f636-111">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="3f636-112">identity</span><span class="sxs-lookup"><span data-stu-id="3f636-112">identity</span></span>                           | [<span data-ttu-id="3f636-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="3f636-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="3f636-114">与此邀请关联[identitySet](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="3f636-114">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="3f636-115">languageId</span><span class="sxs-lookup"><span data-stu-id="3f636-115">languageId</span></span>                         | <span data-ttu-id="3f636-116">String</span><span class="sxs-lookup"><span data-stu-id="3f636-116">String</span></span>                        | <span data-ttu-id="3f636-117">语言区域性字符串。</span><span class="sxs-lookup"><span data-stu-id="3f636-117">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="3f636-118">区域</span><span class="sxs-lookup"><span data-stu-id="3f636-118">region</span></span>                             | <span data-ttu-id="3f636-119">String</span><span class="sxs-lookup"><span data-stu-id="3f636-119">String</span></span>                        | <span data-ttu-id="3f636-120">参与者的区域。</span><span class="sxs-lookup"><span data-stu-id="3f636-120">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="3f636-121">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="3f636-121">replacesCallId</span></span>                     | <span data-ttu-id="3f636-122">String</span><span class="sxs-lookup"><span data-stu-id="3f636-122">String</span></span>                        | <span data-ttu-id="3f636-123">可选。</span><span class="sxs-lookup"><span data-stu-id="3f636-123">Optional.</span></span> <span data-ttu-id="3f636-124">呼叫的目标 idenity 目前的一部分。</span><span class="sxs-lookup"><span data-stu-id="3f636-124">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="3f636-125">一旦添加参与者，此呼叫将被丢弃。</span><span class="sxs-lookup"><span data-stu-id="3f636-125">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3f636-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f636-126">JSON representation</span></span>

<span data-ttu-id="3f636-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f636-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "operationStatus",
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
