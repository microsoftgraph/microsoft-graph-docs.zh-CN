---
title: inviteParticipantsOperation 资源类型
description: 表示长时间运行的参与者邀请操作的状态，通过调用参与者-邀请 API 触发。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5802f5a8a63c971007cb6cda11f16823e6140298
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006681"
---
# <a name="inviteparticipantsoperation-resource-type"></a><span data-ttu-id="c55c5-103">inviteParticipantsOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="c55c5-103">inviteParticipantsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c55c5-104">表示长时间运行的参与者邀请操作的状态，通过调用参与者-邀请 API 触发。</span><span class="sxs-lookup"><span data-stu-id="c55c5-104">Represents the status of a long-running participant invitation operation, triggered by a call to the participant-invite API.</span></span>

## <a name="properties"></a><span data-ttu-id="c55c5-105">属性</span><span class="sxs-lookup"><span data-stu-id="c55c5-105">Properties</span></span>

| <span data-ttu-id="c55c5-106">属性</span><span class="sxs-lookup"><span data-stu-id="c55c5-106">Property</span></span>                       | <span data-ttu-id="c55c5-107">类型</span><span class="sxs-lookup"><span data-stu-id="c55c5-107">Type</span></span>                        | <span data-ttu-id="c55c5-108">说明</span><span class="sxs-lookup"><span data-stu-id="c55c5-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c55c5-109">适用</span><span class="sxs-lookup"><span data-stu-id="c55c5-109">clientContext</span></span>                  | <span data-ttu-id="c55c5-110">String</span><span class="sxs-lookup"><span data-stu-id="c55c5-110">String</span></span>                      | <span data-ttu-id="c55c5-111">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="c55c5-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="c55c5-112">id</span><span class="sxs-lookup"><span data-stu-id="c55c5-112">id</span></span>                             | <span data-ttu-id="c55c5-113">String</span><span class="sxs-lookup"><span data-stu-id="c55c5-113">String</span></span>                      | <span data-ttu-id="c55c5-114">服务器操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="c55c5-114">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="c55c5-115">participants</span><span class="sxs-lookup"><span data-stu-id="c55c5-115">participants</span></span> | <span data-ttu-id="c55c5-116">[invitationParticipantInfo](invitationParticipantInfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="c55c5-116">[invitationParticipantInfo](invitationParticipantInfo.md) collection</span></span> | <span data-ttu-id="c55c5-117">要邀请的参与者。</span><span class="sxs-lookup"><span data-stu-id="c55c5-117">The participants to invite.</span></span> |
| <span data-ttu-id="c55c5-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c55c5-118">resultInfo</span></span>                     | [<span data-ttu-id="c55c5-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c55c5-119">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="c55c5-120">结果信息。</span><span class="sxs-lookup"><span data-stu-id="c55c5-120">The result information.</span></span>  <span data-ttu-id="c55c5-121">只读。</span><span class="sxs-lookup"><span data-stu-id="c55c5-121">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="c55c5-122">状态</span><span class="sxs-lookup"><span data-stu-id="c55c5-122">status</span></span>                         | <span data-ttu-id="c55c5-123">String</span><span class="sxs-lookup"><span data-stu-id="c55c5-123">String</span></span>                      | <span data-ttu-id="c55c5-124">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="c55c5-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="c55c5-125">只读。</span><span class="sxs-lookup"><span data-stu-id="c55c5-125">Read-only.</span></span>                                                  |

## <a name="json-representation"></a><span data-ttu-id="c55c5-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c55c5-126">JSON representation</span></span>

<span data-ttu-id="c55c5-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c55c5-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "participants": [{"@odata.type": "#microsoft.graph.invitationParticipantInfo"}],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inviteParticipantsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
