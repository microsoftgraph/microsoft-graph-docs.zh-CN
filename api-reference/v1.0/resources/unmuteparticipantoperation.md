---
title: unmuteParticipantOperation 资源类型
description: 描述呼叫参与者取消静音操作的响应格式。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3091caf53c4840db5c12ef856908b172a767624f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865756"
---
# <a name="unmuteparticipantoperation-resource-type"></a><span data-ttu-id="79e9b-103">unmuteParticipantOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="79e9b-103">unmuteParticipantOperation resource type</span></span>

<span data-ttu-id="79e9b-104">描述呼叫参与者取消静音操作的响应格式。</span><span class="sxs-lookup"><span data-stu-id="79e9b-104">Describes the response format of a call participant unmute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="79e9b-105">属性</span><span class="sxs-lookup"><span data-stu-id="79e9b-105">Properties</span></span>

| <span data-ttu-id="79e9b-106">属性</span><span class="sxs-lookup"><span data-stu-id="79e9b-106">Property</span></span>                       | <span data-ttu-id="79e9b-107">类型</span><span class="sxs-lookup"><span data-stu-id="79e9b-107">Type</span></span>                        | <span data-ttu-id="79e9b-108">说明</span><span class="sxs-lookup"><span data-stu-id="79e9b-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="79e9b-109">适用</span><span class="sxs-lookup"><span data-stu-id="79e9b-109">clientContext</span></span>                  | <span data-ttu-id="79e9b-110">String</span><span class="sxs-lookup"><span data-stu-id="79e9b-110">String</span></span>                      | <span data-ttu-id="79e9b-111">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="79e9b-111">Unique client context string.</span></span> <span data-ttu-id="79e9b-112">最多可以有256个字符。</span><span class="sxs-lookup"><span data-stu-id="79e9b-112">Can have a maximum of 256 characters.</span></span>                                                                               |
| <span data-ttu-id="79e9b-113">id</span><span class="sxs-lookup"><span data-stu-id="79e9b-113">id</span></span>                             | <span data-ttu-id="79e9b-114">String</span><span class="sxs-lookup"><span data-stu-id="79e9b-114">String</span></span>                      | <span data-ttu-id="79e9b-115">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="79e9b-115">The server operation ID.</span></span> <span data-ttu-id="79e9b-116">只读。</span><span class="sxs-lookup"><span data-stu-id="79e9b-116">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="79e9b-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="79e9b-117">resultInfo</span></span>                     | [<span data-ttu-id="79e9b-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="79e9b-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="79e9b-119">结果信息。</span><span class="sxs-lookup"><span data-stu-id="79e9b-119">The result information.</span></span>  <span data-ttu-id="79e9b-120">只读。</span><span class="sxs-lookup"><span data-stu-id="79e9b-120">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="79e9b-121">状态</span><span class="sxs-lookup"><span data-stu-id="79e9b-121">status</span></span>                         | <span data-ttu-id="79e9b-122">String</span><span class="sxs-lookup"><span data-stu-id="79e9b-122">String</span></span>                      | <span data-ttu-id="79e9b-123">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="79e9b-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="79e9b-124">只读。</span><span class="sxs-lookup"><span data-stu-id="79e9b-124">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="79e9b-125">关系</span><span class="sxs-lookup"><span data-stu-id="79e9b-125">Relationships</span></span>
<span data-ttu-id="79e9b-126">无。</span><span class="sxs-lookup"><span data-stu-id="79e9b-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="79e9b-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79e9b-127">JSON representation</span></span>

<span data-ttu-id="79e9b-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79e9b-128">The following is a JSON representation of the resource.</span></span>

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
