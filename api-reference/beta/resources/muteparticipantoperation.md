---
title: MuteParticipantOperation 资源类型
description: 描述呼叫参与者静音操作的响应格式。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c5d5e716e4d8266d97139c1283415994f6206aea
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006618"
---
# <a name="muteparticipantoperation-resource-type"></a><span data-ttu-id="68b52-103">MuteParticipantOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="68b52-103">MuteParticipantOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68b52-104">描述呼叫参与者静音操作的响应格式。</span><span class="sxs-lookup"><span data-stu-id="68b52-104">Describes the response format of a call participant mute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="68b52-105">属性</span><span class="sxs-lookup"><span data-stu-id="68b52-105">Properties</span></span>

| <span data-ttu-id="68b52-106">属性</span><span class="sxs-lookup"><span data-stu-id="68b52-106">Property</span></span>                       | <span data-ttu-id="68b52-107">类型</span><span class="sxs-lookup"><span data-stu-id="68b52-107">Type</span></span>                        | <span data-ttu-id="68b52-108">说明</span><span class="sxs-lookup"><span data-stu-id="68b52-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="68b52-109">适用</span><span class="sxs-lookup"><span data-stu-id="68b52-109">clientContext</span></span>                  | <span data-ttu-id="68b52-110">String</span><span class="sxs-lookup"><span data-stu-id="68b52-110">String</span></span>                      | <span data-ttu-id="68b52-111">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="68b52-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="68b52-112">id</span><span class="sxs-lookup"><span data-stu-id="68b52-112">id</span></span>                             | <span data-ttu-id="68b52-113">String</span><span class="sxs-lookup"><span data-stu-id="68b52-113">String</span></span>                      | <span data-ttu-id="68b52-114">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="68b52-114">The server operation ID.</span></span> <span data-ttu-id="68b52-115">只读。</span><span class="sxs-lookup"><span data-stu-id="68b52-115">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="68b52-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="68b52-116">resultInfo</span></span>                     | [<span data-ttu-id="68b52-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="68b52-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="68b52-118">结果信息。</span><span class="sxs-lookup"><span data-stu-id="68b52-118">The result information.</span></span>  <span data-ttu-id="68b52-119">只读。</span><span class="sxs-lookup"><span data-stu-id="68b52-119">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="68b52-120">状态</span><span class="sxs-lookup"><span data-stu-id="68b52-120">status</span></span>                         | <span data-ttu-id="68b52-121">String</span><span class="sxs-lookup"><span data-stu-id="68b52-121">String</span></span>                      | <span data-ttu-id="68b52-122">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="68b52-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="68b52-123">只读。</span><span class="sxs-lookup"><span data-stu-id="68b52-123">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="68b52-124">关系</span><span class="sxs-lookup"><span data-stu-id="68b52-124">Relationships</span></span>
<span data-ttu-id="68b52-125">无</span><span class="sxs-lookup"><span data-stu-id="68b52-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68b52-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68b52-126">JSON representation</span></span>

<span data-ttu-id="68b52-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68b52-127">The following is a JSON representation of the resource.</span></span>

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
