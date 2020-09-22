---
title: invitationParticipantInfo 资源类型
description: 表示受邀加入组呼叫的实体。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9193ec70a3884ba9bf25e4f1c8c33eb7c77d838f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989036"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="c0c1d-103">invitationParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="c0c1d-103">invitationParticipantInfo resource type</span></span>

<span data-ttu-id="c0c1d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0c1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0c1d-105">表示受邀加入组呼叫的实体。</span><span class="sxs-lookup"><span data-stu-id="c0c1d-105">Represents an entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="c0c1d-106">属性</span><span class="sxs-lookup"><span data-stu-id="c0c1d-106">Properties</span></span>

| <span data-ttu-id="c0c1d-107">属性</span><span class="sxs-lookup"><span data-stu-id="c0c1d-107">Property</span></span>                           | <span data-ttu-id="c0c1d-108">类型</span><span class="sxs-lookup"><span data-stu-id="c0c1d-108">Type</span></span>                          | <span data-ttu-id="c0c1d-109">说明</span><span class="sxs-lookup"><span data-stu-id="c0c1d-109">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="c0c1d-110">endpointType</span><span class="sxs-lookup"><span data-stu-id="c0c1d-110">endpointType</span></span>                       | <span data-ttu-id="c0c1d-111">String</span><span class="sxs-lookup"><span data-stu-id="c0c1d-111">String</span></span>                        | <span data-ttu-id="c0c1d-112">终结点的类型。</span><span class="sxs-lookup"><span data-stu-id="c0c1d-112">The type of endpoint.</span></span> <span data-ttu-id="c0c1d-113">可取值为：`default`、`voicemail`。</span><span class="sxs-lookup"><span data-stu-id="c0c1d-113">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="c0c1d-114">窃取</span><span class="sxs-lookup"><span data-stu-id="c0c1d-114">identity</span></span>                           | [<span data-ttu-id="c0c1d-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="c0c1d-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="c0c1d-116">与此邀请关联的 [了解 identityset](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="c0c1d-116">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="c0c1d-117">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="c0c1d-117">replacesCallId</span></span>                     | <span data-ttu-id="c0c1d-118">String</span><span class="sxs-lookup"><span data-stu-id="c0c1d-118">String</span></span>                        | <span data-ttu-id="c0c1d-119">可选。</span><span class="sxs-lookup"><span data-stu-id="c0c1d-119">Optional.</span></span> <span data-ttu-id="c0c1d-120">目标 idenity 当前是其一部分的调用。</span><span class="sxs-lookup"><span data-stu-id="c0c1d-120">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="c0c1d-121">添加参与者后，将删除此呼叫。</span><span class="sxs-lookup"><span data-stu-id="c0c1d-121">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c0c1d-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0c1d-122">JSON representation</span></span>

<span data-ttu-id="c0c1d-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0c1d-123">The following is a JSON representation of the resource.</span></span>

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


