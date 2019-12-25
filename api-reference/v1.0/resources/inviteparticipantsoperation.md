---
title: inviteParticipantsOperation 资源类型
description: 表示长时间运行的参与者邀请操作的状态，通过调用参与者-邀请 API 触发。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d0198ae992dc3e741c2962ed4e2c9534f5a76757
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865780"
---
# <a name="inviteparticipantsoperation-resource-type"></a><span data-ttu-id="ba99f-103">inviteParticipantsOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba99f-103">inviteParticipantsOperation resource type</span></span>

<span data-ttu-id="ba99f-104">表示长时间运行的参与者邀请操作的状态，通过调用参与者-邀请 API 触发。</span><span class="sxs-lookup"><span data-stu-id="ba99f-104">Represents the status of a long-running participant invitation operation, triggered by a call to the participant-invite API.</span></span>

## <a name="properties"></a><span data-ttu-id="ba99f-105">属性</span><span class="sxs-lookup"><span data-stu-id="ba99f-105">Properties</span></span>

| <span data-ttu-id="ba99f-106">属性</span><span class="sxs-lookup"><span data-stu-id="ba99f-106">Property</span></span>                       | <span data-ttu-id="ba99f-107">类型</span><span class="sxs-lookup"><span data-stu-id="ba99f-107">Type</span></span>                        | <span data-ttu-id="ba99f-108">说明</span><span class="sxs-lookup"><span data-stu-id="ba99f-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ba99f-109">适用</span><span class="sxs-lookup"><span data-stu-id="ba99f-109">clientContext</span></span>                  | <span data-ttu-id="ba99f-110">String</span><span class="sxs-lookup"><span data-stu-id="ba99f-110">String</span></span>                      | <span data-ttu-id="ba99f-111">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="ba99f-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="ba99f-112">id</span><span class="sxs-lookup"><span data-stu-id="ba99f-112">id</span></span>                             | <span data-ttu-id="ba99f-113">String</span><span class="sxs-lookup"><span data-stu-id="ba99f-113">String</span></span>                      | <span data-ttu-id="ba99f-114">服务器操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="ba99f-114">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="ba99f-115">participants</span><span class="sxs-lookup"><span data-stu-id="ba99f-115">participants</span></span> | <span data-ttu-id="ba99f-116">[invitationParticipantInfo](invitationParticipantInfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ba99f-116">[invitationParticipantInfo](invitationParticipantInfo.md) collection</span></span> | <span data-ttu-id="ba99f-117">要邀请的参与者。</span><span class="sxs-lookup"><span data-stu-id="ba99f-117">The participants to invite.</span></span> |
| <span data-ttu-id="ba99f-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="ba99f-118">resultInfo</span></span>                     | [<span data-ttu-id="ba99f-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="ba99f-119">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="ba99f-120">结果信息。</span><span class="sxs-lookup"><span data-stu-id="ba99f-120">The result information.</span></span>  <span data-ttu-id="ba99f-121">只读。</span><span class="sxs-lookup"><span data-stu-id="ba99f-121">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="ba99f-122">状态</span><span class="sxs-lookup"><span data-stu-id="ba99f-122">status</span></span>                         | <span data-ttu-id="ba99f-123">String</span><span class="sxs-lookup"><span data-stu-id="ba99f-123">String</span></span>                      | <span data-ttu-id="ba99f-124">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="ba99f-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="ba99f-125">只读。</span><span class="sxs-lookup"><span data-stu-id="ba99f-125">Read-only.</span></span>                                                  |

## <a name="json-representation"></a><span data-ttu-id="ba99f-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba99f-126">JSON representation</span></span>

<span data-ttu-id="ba99f-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba99f-127">The following is a JSON representation of the resource.</span></span>

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
