---
title: inviteParticipantsOperation 资源类型
description: 表示长时间运行的参与者邀请操作的状态，通过调用参与者-邀请 API 触发。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a974bd22ddd9e1ac8c6ab90cdedb9dda9f1a1bb5
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36793021"
---
# <a name="inviteparticipantsoperation-resource-type"></a><span data-ttu-id="1462a-103">inviteParticipantsOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="1462a-103">inviteParticipantsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1462a-104">表示长时间运行的参与者邀请操作的状态，通过调用参与者-邀请 API 触发。</span><span class="sxs-lookup"><span data-stu-id="1462a-104">Represents the status of a long-running participant invitation operation, triggered by a call to the participant-invite API.</span></span>

## <a name="properties"></a><span data-ttu-id="1462a-105">属性</span><span class="sxs-lookup"><span data-stu-id="1462a-105">Properties</span></span>

| <span data-ttu-id="1462a-106">属性</span><span class="sxs-lookup"><span data-stu-id="1462a-106">Property</span></span>                       | <span data-ttu-id="1462a-107">类型</span><span class="sxs-lookup"><span data-stu-id="1462a-107">Type</span></span>                        | <span data-ttu-id="1462a-108">说明</span><span class="sxs-lookup"><span data-stu-id="1462a-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1462a-109">适用</span><span class="sxs-lookup"><span data-stu-id="1462a-109">clientContext</span></span>                  | <span data-ttu-id="1462a-110">String</span><span class="sxs-lookup"><span data-stu-id="1462a-110">String</span></span>                      | <span data-ttu-id="1462a-111">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="1462a-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="1462a-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1462a-112">createdDateTime</span></span>                | <span data-ttu-id="1462a-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1462a-113">DateTimeOffset</span></span>              | <span data-ttu-id="1462a-114">创建录制的时间。</span><span class="sxs-lookup"><span data-stu-id="1462a-114">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="1462a-115">id</span><span class="sxs-lookup"><span data-stu-id="1462a-115">id</span></span>                             | <span data-ttu-id="1462a-116">String</span><span class="sxs-lookup"><span data-stu-id="1462a-116">String</span></span>                      | <span data-ttu-id="1462a-117">服务器操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="1462a-117">The server operation id. Read-only.</span></span> <span data-ttu-id="1462a-118">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="1462a-118">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="1462a-119">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="1462a-119">lastActionDateTime</span></span>             | <span data-ttu-id="1462a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1462a-120">DateTimeOffset</span></span>              | <span data-ttu-id="1462a-121">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="1462a-121">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="1462a-122">participants</span><span class="sxs-lookup"><span data-stu-id="1462a-122">participants</span></span> | <span data-ttu-id="1462a-123">[invitationParticipantInfo](invitationParticipantInfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="1462a-123">[invitationParticipantInfo](invitationParticipantInfo.md) collection</span></span> | <span data-ttu-id="1462a-124">要邀请的参与者。</span><span class="sxs-lookup"><span data-stu-id="1462a-124">The participants to invite.</span></span> |
| <span data-ttu-id="1462a-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="1462a-125">resultInfo</span></span>                     | [<span data-ttu-id="1462a-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="1462a-126">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="1462a-127">结果信息。</span><span class="sxs-lookup"><span data-stu-id="1462a-127">The result information.</span></span>  <span data-ttu-id="1462a-128">只读。</span><span class="sxs-lookup"><span data-stu-id="1462a-128">Read-only.</span></span> <span data-ttu-id="1462a-129">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="1462a-129">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="1462a-130">status</span><span class="sxs-lookup"><span data-stu-id="1462a-130">status</span></span>                         | <span data-ttu-id="1462a-131">String</span><span class="sxs-lookup"><span data-stu-id="1462a-131">String</span></span>                      | <span data-ttu-id="1462a-132">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="1462a-132">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="1462a-133">只读。</span><span class="sxs-lookup"><span data-stu-id="1462a-133">Read-only.</span></span> <span data-ttu-id="1462a-134">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="1462a-134">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="1462a-135">关系</span><span class="sxs-lookup"><span data-stu-id="1462a-135">Relationships</span></span>
<span data-ttu-id="1462a-136">无</span><span class="sxs-lookup"><span data-stu-id="1462a-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1462a-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1462a-137">JSON representation</span></span>

<span data-ttu-id="1462a-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1462a-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
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
