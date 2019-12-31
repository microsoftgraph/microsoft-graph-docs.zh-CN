---
title: MuteParticipantOperation 资源类型
description: 描述呼叫参与者静音操作的响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 291af6799d744fc717f15dcbdcddcbdc98518d34
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913210"
---
# <a name="muteparticipantoperation-resource-type"></a><span data-ttu-id="167a4-103">MuteParticipantOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="167a4-103">MuteParticipantOperation resource type</span></span>

<span data-ttu-id="167a4-104">描述呼叫参与者静音操作的响应格式。</span><span class="sxs-lookup"><span data-stu-id="167a4-104">Describes the response format of a call participant mute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="167a4-105">属性</span><span class="sxs-lookup"><span data-stu-id="167a4-105">Properties</span></span>

| <span data-ttu-id="167a4-106">属性</span><span class="sxs-lookup"><span data-stu-id="167a4-106">Property</span></span>                       | <span data-ttu-id="167a4-107">类型</span><span class="sxs-lookup"><span data-stu-id="167a4-107">Type</span></span>                        | <span data-ttu-id="167a4-108">说明</span><span class="sxs-lookup"><span data-stu-id="167a4-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="167a4-109">适用</span><span class="sxs-lookup"><span data-stu-id="167a4-109">clientContext</span></span>                  | <span data-ttu-id="167a4-110">String</span><span class="sxs-lookup"><span data-stu-id="167a4-110">String</span></span>                      | <span data-ttu-id="167a4-111">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="167a4-111">Unique client context string.</span></span> <span data-ttu-id="167a4-112">最多可以有256个字符。</span><span class="sxs-lookup"><span data-stu-id="167a4-112">Can have a maximum of 256 characters.</span></span>                                                                               |
| <span data-ttu-id="167a4-113">id</span><span class="sxs-lookup"><span data-stu-id="167a4-113">id</span></span>                             | <span data-ttu-id="167a4-114">String</span><span class="sxs-lookup"><span data-stu-id="167a4-114">String</span></span>                      | <span data-ttu-id="167a4-115">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="167a4-115">The server operation ID.</span></span> <span data-ttu-id="167a4-116">只读。</span><span class="sxs-lookup"><span data-stu-id="167a4-116">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="167a4-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="167a4-117">resultInfo</span></span>                     | [<span data-ttu-id="167a4-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="167a4-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="167a4-119">结果信息。</span><span class="sxs-lookup"><span data-stu-id="167a4-119">The result information.</span></span>  <span data-ttu-id="167a4-120">只读。</span><span class="sxs-lookup"><span data-stu-id="167a4-120">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="167a4-121">状态</span><span class="sxs-lookup"><span data-stu-id="167a4-121">status</span></span>                         | <span data-ttu-id="167a4-122">String</span><span class="sxs-lookup"><span data-stu-id="167a4-122">String</span></span>                      | <span data-ttu-id="167a4-123">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="167a4-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="167a4-124">只读。</span><span class="sxs-lookup"><span data-stu-id="167a4-124">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="167a4-125">关系</span><span class="sxs-lookup"><span data-stu-id="167a4-125">Relationships</span></span>
<span data-ttu-id="167a4-126">无。</span><span class="sxs-lookup"><span data-stu-id="167a4-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="167a4-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="167a4-127">JSON representation</span></span>

<span data-ttu-id="167a4-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="167a4-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.muteParticipantOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "muteParticipantOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
