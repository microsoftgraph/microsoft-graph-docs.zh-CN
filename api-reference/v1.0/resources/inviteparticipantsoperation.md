---
title: inviteParticipantsOperation 资源类型
description: 表示长时间运行的参与者邀请操作的状态，通过调用参与者-邀请 API 触发。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7e729a572ceb69f59ed6cc00cd0a2e132765ed8a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967490"
---
# <a name="inviteparticipantsoperation-resource-type"></a><span data-ttu-id="d8134-103">inviteParticipantsOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8134-103">inviteParticipantsOperation resource type</span></span>

<span data-ttu-id="d8134-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8134-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d8134-105">表示长时间运行的参与者邀请操作的状态，通过调用参与者-邀请 API 触发。</span><span class="sxs-lookup"><span data-stu-id="d8134-105">Represents the status of a long-running participant invitation operation, triggered by a call to the participant-invite API.</span></span>

## <a name="properties"></a><span data-ttu-id="d8134-106">属性</span><span class="sxs-lookup"><span data-stu-id="d8134-106">Properties</span></span>

| <span data-ttu-id="d8134-107">属性</span><span class="sxs-lookup"><span data-stu-id="d8134-107">Property</span></span>                       | <span data-ttu-id="d8134-108">类型</span><span class="sxs-lookup"><span data-stu-id="d8134-108">Type</span></span>                        | <span data-ttu-id="d8134-109">说明</span><span class="sxs-lookup"><span data-stu-id="d8134-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d8134-110">适用</span><span class="sxs-lookup"><span data-stu-id="d8134-110">clientContext</span></span>                  | <span data-ttu-id="d8134-111">String</span><span class="sxs-lookup"><span data-stu-id="d8134-111">String</span></span>                      | <span data-ttu-id="d8134-112">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="d8134-112">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="d8134-113">id</span><span class="sxs-lookup"><span data-stu-id="d8134-113">id</span></span>                             | <span data-ttu-id="d8134-114">String</span><span class="sxs-lookup"><span data-stu-id="d8134-114">String</span></span>                      | <span data-ttu-id="d8134-115">服务器操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="d8134-115">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="d8134-116">participants</span><span class="sxs-lookup"><span data-stu-id="d8134-116">participants</span></span> | <span data-ttu-id="d8134-117">[invitationParticipantInfo](invitationParticipantInfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d8134-117">[invitationParticipantInfo](invitationParticipantInfo.md) collection</span></span> | <span data-ttu-id="d8134-118">要邀请的参与者。</span><span class="sxs-lookup"><span data-stu-id="d8134-118">The participants to invite.</span></span> |
| <span data-ttu-id="d8134-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d8134-119">resultInfo</span></span>                     | [<span data-ttu-id="d8134-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d8134-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="d8134-121">结果信息。</span><span class="sxs-lookup"><span data-stu-id="d8134-121">The result information.</span></span>  <span data-ttu-id="d8134-122">只读。</span><span class="sxs-lookup"><span data-stu-id="d8134-122">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="d8134-123">状态</span><span class="sxs-lookup"><span data-stu-id="d8134-123">status</span></span>                         | <span data-ttu-id="d8134-124">String</span><span class="sxs-lookup"><span data-stu-id="d8134-124">String</span></span>                      | <span data-ttu-id="d8134-125">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="d8134-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="d8134-126">只读。</span><span class="sxs-lookup"><span data-stu-id="d8134-126">Read-only.</span></span>                                                  |

## <a name="json-representation"></a><span data-ttu-id="d8134-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8134-127">JSON representation</span></span>

<span data-ttu-id="d8134-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8134-128">The following is a JSON representation of the resource.</span></span>

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

