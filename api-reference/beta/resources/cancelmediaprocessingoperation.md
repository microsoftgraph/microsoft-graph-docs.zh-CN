---
title: CancelMediaProcessingOperation 资源类型
description: 此资源类型用于描述媒体处理取消操作的响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b1f74ba825bdd953803c3458882cbae051fae970
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042714"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a><span data-ttu-id="4f4ed-103">CancelMediaProcessingOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f4ed-103">CancelMediaProcessingOperation resource type</span></span>

<span data-ttu-id="4f4ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f4ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f4ed-105">描述媒体处理取消操作的响应格式。</span><span class="sxs-lookup"><span data-stu-id="4f4ed-105">Describes the response format of media processing cancel operation.</span></span>

## <a name="properties"></a><span data-ttu-id="4f4ed-106">属性</span><span class="sxs-lookup"><span data-stu-id="4f4ed-106">Properties</span></span>

| <span data-ttu-id="4f4ed-107">属性</span><span class="sxs-lookup"><span data-stu-id="4f4ed-107">Property</span></span>                       | <span data-ttu-id="4f4ed-108">类型</span><span class="sxs-lookup"><span data-stu-id="4f4ed-108">Type</span></span>                        | <span data-ttu-id="4f4ed-109">说明</span><span class="sxs-lookup"><span data-stu-id="4f4ed-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4f4ed-110">各种</span><span class="sxs-lookup"><span data-stu-id="4f4ed-110">all</span></span>                            | <span data-ttu-id="4f4ed-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f4ed-111">Boolean</span></span>                     | <span data-ttu-id="4f4ed-112">指示是否停止所有操作或当前操作。</span><span class="sxs-lookup"><span data-stu-id="4f4ed-112">Indicates whether to stop all operations or current.</span></span>                                                                                    |
| <span data-ttu-id="4f4ed-113">适用</span><span class="sxs-lookup"><span data-stu-id="4f4ed-113">clientContext</span></span>                  | <span data-ttu-id="4f4ed-114">String</span><span class="sxs-lookup"><span data-stu-id="4f4ed-114">String</span></span>                      | <span data-ttu-id="4f4ed-115">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="4f4ed-115">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="4f4ed-116">id</span><span class="sxs-lookup"><span data-stu-id="4f4ed-116">id</span></span>                             | <span data-ttu-id="4f4ed-117">String</span><span class="sxs-lookup"><span data-stu-id="4f4ed-117">String</span></span>                      | <span data-ttu-id="4f4ed-118">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="4f4ed-118">The server operation ID.</span></span> <span data-ttu-id="4f4ed-119">只读。</span><span class="sxs-lookup"><span data-stu-id="4f4ed-119">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="4f4ed-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="4f4ed-120">resultInfo</span></span>                     | [<span data-ttu-id="4f4ed-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="4f4ed-121">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="4f4ed-122">结果信息。</span><span class="sxs-lookup"><span data-stu-id="4f4ed-122">The result information.</span></span>  <span data-ttu-id="4f4ed-123">只读。</span><span class="sxs-lookup"><span data-stu-id="4f4ed-123">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="4f4ed-124">状态</span><span class="sxs-lookup"><span data-stu-id="4f4ed-124">status</span></span>                         | <span data-ttu-id="4f4ed-125">String</span><span class="sxs-lookup"><span data-stu-id="4f4ed-125">String</span></span>                      | <span data-ttu-id="4f4ed-126">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="4f4ed-126">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="4f4ed-127">只读。</span><span class="sxs-lookup"><span data-stu-id="4f4ed-127">Read-only.</span></span>                                                  |

## <a name="relationships"></a><span data-ttu-id="4f4ed-128">关系</span><span class="sxs-lookup"><span data-stu-id="4f4ed-128">Relationships</span></span>
<span data-ttu-id="4f4ed-129">无</span><span class="sxs-lookup"><span data-stu-id="4f4ed-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f4ed-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f4ed-130">JSON representation</span></span>

<span data-ttu-id="4f4ed-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f4ed-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cancelMediaProcessingOperation"
}-->
```json
{
  "all": true,
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
  "description": "cancelMediaProcessingOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


