---
title: inviteParticipantsOperation 资源类型
description: 表示长时间运行的参与者邀请操作的状态，通过调用参与者-邀请 API 触发。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 54223a5b9e807dc45a9868b3251b8d8b1a0fcd72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447687"
---
# <a name="inviteparticipantsoperation-resource-type"></a><span data-ttu-id="8488e-103">inviteParticipantsOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="8488e-103">inviteParticipantsOperation resource type</span></span>

<span data-ttu-id="8488e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8488e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8488e-105">表示长时间运行的参与者邀请操作的状态，通过调用参与者-邀请 API 触发。</span><span class="sxs-lookup"><span data-stu-id="8488e-105">Represents the status of a long-running participant invitation operation, triggered by a call to the participant-invite API.</span></span>

## <a name="properties"></a><span data-ttu-id="8488e-106">属性</span><span class="sxs-lookup"><span data-stu-id="8488e-106">Properties</span></span>

| <span data-ttu-id="8488e-107">属性</span><span class="sxs-lookup"><span data-stu-id="8488e-107">Property</span></span>                       | <span data-ttu-id="8488e-108">类型</span><span class="sxs-lookup"><span data-stu-id="8488e-108">Type</span></span>                        | <span data-ttu-id="8488e-109">说明</span><span class="sxs-lookup"><span data-stu-id="8488e-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8488e-110">适用</span><span class="sxs-lookup"><span data-stu-id="8488e-110">clientContext</span></span>                  | <span data-ttu-id="8488e-111">String</span><span class="sxs-lookup"><span data-stu-id="8488e-111">String</span></span>                      | <span data-ttu-id="8488e-112">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="8488e-112">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="8488e-113">id</span><span class="sxs-lookup"><span data-stu-id="8488e-113">id</span></span>                             | <span data-ttu-id="8488e-114">String</span><span class="sxs-lookup"><span data-stu-id="8488e-114">String</span></span>                      | <span data-ttu-id="8488e-115">服务器操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="8488e-115">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="8488e-116">participants</span><span class="sxs-lookup"><span data-stu-id="8488e-116">participants</span></span> | <span data-ttu-id="8488e-117">[invitationParticipantInfo](invitationParticipantInfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8488e-117">[invitationParticipantInfo](invitationParticipantInfo.md) collection</span></span> | <span data-ttu-id="8488e-118">要邀请的参与者。</span><span class="sxs-lookup"><span data-stu-id="8488e-118">The participants to invite.</span></span> |
| <span data-ttu-id="8488e-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="8488e-119">resultInfo</span></span>                     | [<span data-ttu-id="8488e-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="8488e-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="8488e-121">结果信息。</span><span class="sxs-lookup"><span data-stu-id="8488e-121">The result information.</span></span>  <span data-ttu-id="8488e-122">只读。</span><span class="sxs-lookup"><span data-stu-id="8488e-122">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="8488e-123">status</span><span class="sxs-lookup"><span data-stu-id="8488e-123">status</span></span>                         | <span data-ttu-id="8488e-124">String</span><span class="sxs-lookup"><span data-stu-id="8488e-124">String</span></span>                      | <span data-ttu-id="8488e-125">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="8488e-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="8488e-126">只读。</span><span class="sxs-lookup"><span data-stu-id="8488e-126">Read-only.</span></span>                                                  |

## <a name="json-representation"></a><span data-ttu-id="8488e-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8488e-127">JSON representation</span></span>

<span data-ttu-id="8488e-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8488e-128">The following is a JSON representation of the resource.</span></span>

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
