---
title: CancelMediaProcessingOperation 资源类型
description: 此资源类型用于描述媒体处理取消操作的响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 20da55c068f6e0f0a69b876cfd23181eac1391a4
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913497"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a><span data-ttu-id="91feb-103">CancelMediaProcessingOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="91feb-103">CancelMediaProcessingOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91feb-104">描述媒体处理取消操作的响应格式。</span><span class="sxs-lookup"><span data-stu-id="91feb-104">Describes the response format of media processing cancel operation.</span></span>

## <a name="properties"></a><span data-ttu-id="91feb-105">属性</span><span class="sxs-lookup"><span data-stu-id="91feb-105">Properties</span></span>

| <span data-ttu-id="91feb-106">属性</span><span class="sxs-lookup"><span data-stu-id="91feb-106">Property</span></span>                       | <span data-ttu-id="91feb-107">类型</span><span class="sxs-lookup"><span data-stu-id="91feb-107">Type</span></span>                        | <span data-ttu-id="91feb-108">说明</span><span class="sxs-lookup"><span data-stu-id="91feb-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="91feb-109">各种</span><span class="sxs-lookup"><span data-stu-id="91feb-109">all</span></span>                            | <span data-ttu-id="91feb-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="91feb-110">Boolean</span></span>                     | <span data-ttu-id="91feb-111">指示是否停止所有操作或当前操作。</span><span class="sxs-lookup"><span data-stu-id="91feb-111">Indicates whether to stop all operations or current.</span></span>                                                                                    |
| <span data-ttu-id="91feb-112">适用</span><span class="sxs-lookup"><span data-stu-id="91feb-112">clientContext</span></span>                  | <span data-ttu-id="91feb-113">String</span><span class="sxs-lookup"><span data-stu-id="91feb-113">String</span></span>                      | <span data-ttu-id="91feb-114">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="91feb-114">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="91feb-115">id</span><span class="sxs-lookup"><span data-stu-id="91feb-115">id</span></span>                             | <span data-ttu-id="91feb-116">String</span><span class="sxs-lookup"><span data-stu-id="91feb-116">String</span></span>                      | <span data-ttu-id="91feb-117">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="91feb-117">The server operation ID.</span></span> <span data-ttu-id="91feb-118">只读。</span><span class="sxs-lookup"><span data-stu-id="91feb-118">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="91feb-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="91feb-119">resultInfo</span></span>                     | [<span data-ttu-id="91feb-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="91feb-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="91feb-121">结果信息。</span><span class="sxs-lookup"><span data-stu-id="91feb-121">The result information.</span></span>  <span data-ttu-id="91feb-122">只读。</span><span class="sxs-lookup"><span data-stu-id="91feb-122">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="91feb-123">状态</span><span class="sxs-lookup"><span data-stu-id="91feb-123">status</span></span>                         | <span data-ttu-id="91feb-124">String</span><span class="sxs-lookup"><span data-stu-id="91feb-124">String</span></span>                      | <span data-ttu-id="91feb-125">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="91feb-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="91feb-126">只读。</span><span class="sxs-lookup"><span data-stu-id="91feb-126">Read-only.</span></span>                                                  |

## <a name="relationships"></a><span data-ttu-id="91feb-127">关系</span><span class="sxs-lookup"><span data-stu-id="91feb-127">Relationships</span></span>
<span data-ttu-id="91feb-128">无</span><span class="sxs-lookup"><span data-stu-id="91feb-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91feb-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91feb-129">JSON representation</span></span>

<span data-ttu-id="91feb-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91feb-130">The following is a JSON representation of the resource.</span></span>

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
