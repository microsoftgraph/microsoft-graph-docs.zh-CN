---
title: unmuteParticipantOperation 资源类型
description: 描述呼叫参与者取消静音操作的响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2b4c0ff8132eddadebaedb7e62965a0808c96210
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075393"
---
# <a name="unmuteparticipantoperation-resource-type"></a><span data-ttu-id="17cb6-103">unmuteParticipantOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="17cb6-103">unmuteParticipantOperation resource type</span></span>

<span data-ttu-id="17cb6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17cb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17cb6-105">描述呼叫参与者取消静音操作的响应格式。</span><span class="sxs-lookup"><span data-stu-id="17cb6-105">Describes the response format of a call participant unmute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="17cb6-106">属性</span><span class="sxs-lookup"><span data-stu-id="17cb6-106">Properties</span></span>

| <span data-ttu-id="17cb6-107">属性</span><span class="sxs-lookup"><span data-stu-id="17cb6-107">Property</span></span>                       | <span data-ttu-id="17cb6-108">类型</span><span class="sxs-lookup"><span data-stu-id="17cb6-108">Type</span></span>                        | <span data-ttu-id="17cb6-109">说明</span><span class="sxs-lookup"><span data-stu-id="17cb6-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="17cb6-110">适用</span><span class="sxs-lookup"><span data-stu-id="17cb6-110">clientContext</span></span>                  | <span data-ttu-id="17cb6-111">String</span><span class="sxs-lookup"><span data-stu-id="17cb6-111">String</span></span>                      | <span data-ttu-id="17cb6-112">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="17cb6-112">Unique client context string.</span></span> <span data-ttu-id="17cb6-113">最多可以有256个字符。</span><span class="sxs-lookup"><span data-stu-id="17cb6-113">Can have a maximum of 256 characters.</span></span>                                                                               |
| <span data-ttu-id="17cb6-114">id</span><span class="sxs-lookup"><span data-stu-id="17cb6-114">id</span></span>                             | <span data-ttu-id="17cb6-115">String</span><span class="sxs-lookup"><span data-stu-id="17cb6-115">String</span></span>                      | <span data-ttu-id="17cb6-116">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="17cb6-116">The server operation ID.</span></span> <span data-ttu-id="17cb6-117">只读。</span><span class="sxs-lookup"><span data-stu-id="17cb6-117">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="17cb6-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="17cb6-118">resultInfo</span></span>                     | [<span data-ttu-id="17cb6-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="17cb6-119">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="17cb6-120">结果信息。</span><span class="sxs-lookup"><span data-stu-id="17cb6-120">The result information.</span></span>  <span data-ttu-id="17cb6-121">只读。</span><span class="sxs-lookup"><span data-stu-id="17cb6-121">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="17cb6-122">状态</span><span class="sxs-lookup"><span data-stu-id="17cb6-122">status</span></span>                         | <span data-ttu-id="17cb6-123">String</span><span class="sxs-lookup"><span data-stu-id="17cb6-123">String</span></span>                      | <span data-ttu-id="17cb6-124">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="17cb6-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="17cb6-125">只读。</span><span class="sxs-lookup"><span data-stu-id="17cb6-125">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="17cb6-126">关系</span><span class="sxs-lookup"><span data-stu-id="17cb6-126">Relationships</span></span>
<span data-ttu-id="17cb6-127">无。</span><span class="sxs-lookup"><span data-stu-id="17cb6-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="17cb6-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17cb6-128">JSON representation</span></span>

<span data-ttu-id="17cb6-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17cb6-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unmuteParticipantOperation"
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
  "description": "unmuteParticipantOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


