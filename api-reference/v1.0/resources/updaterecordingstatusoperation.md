---
title: updateRecordingStatusOperation 资源类型
description: 介绍更新录制状态操作的响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: de1cf2578f699fde25d8863d12fcf4e262d78000
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962523"
---
# <a name="updaterecordingstatusoperation-resource-type"></a><span data-ttu-id="5328e-103">updateRecordingStatusOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="5328e-103">updateRecordingStatusOperation resource type</span></span>

<span data-ttu-id="5328e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5328e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5328e-105">介绍更新录制状态操作的响应格式。</span><span class="sxs-lookup"><span data-stu-id="5328e-105">Describes the response format of an update recording status action.</span></span>

## <a name="properties"></a><span data-ttu-id="5328e-106">属性</span><span class="sxs-lookup"><span data-stu-id="5328e-106">Properties</span></span>

| <span data-ttu-id="5328e-107">属性</span><span class="sxs-lookup"><span data-stu-id="5328e-107">Property</span></span>            | <span data-ttu-id="5328e-108">类型</span><span class="sxs-lookup"><span data-stu-id="5328e-108">Type</span></span>                        | <span data-ttu-id="5328e-109">说明</span><span class="sxs-lookup"><span data-stu-id="5328e-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="5328e-110">适用</span><span class="sxs-lookup"><span data-stu-id="5328e-110">clientContext</span></span>       | <span data-ttu-id="5328e-111">String</span><span class="sxs-lookup"><span data-stu-id="5328e-111">String</span></span>                      | <span data-ttu-id="5328e-112">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="5328e-112">Unique client context string.</span></span> <span data-ttu-id="5328e-113">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="5328e-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="5328e-114">id</span><span class="sxs-lookup"><span data-stu-id="5328e-114">id</span></span>                  | <span data-ttu-id="5328e-115">字符串</span><span class="sxs-lookup"><span data-stu-id="5328e-115">String</span></span>                      | <span data-ttu-id="5328e-116">只读。</span><span class="sxs-lookup"><span data-stu-id="5328e-116">Read-only.</span></span>                                                                         |
| <span data-ttu-id="5328e-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="5328e-117">resultInfo</span></span>          | [<span data-ttu-id="5328e-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="5328e-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="5328e-119">结果信息。</span><span class="sxs-lookup"><span data-stu-id="5328e-119">The result information.</span></span> <span data-ttu-id="5328e-120">只读。</span><span class="sxs-lookup"><span data-stu-id="5328e-120">Read-only.</span></span>                                                 |
| <span data-ttu-id="5328e-121">状态</span><span class="sxs-lookup"><span data-stu-id="5328e-121">status</span></span>              | <span data-ttu-id="5328e-122">String</span><span class="sxs-lookup"><span data-stu-id="5328e-122">String</span></span>                      | <span data-ttu-id="5328e-123">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="5328e-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="5328e-124">关系</span><span class="sxs-lookup"><span data-stu-id="5328e-124">Relationships</span></span>
<span data-ttu-id="5328e-125">无。</span><span class="sxs-lookup"><span data-stu-id="5328e-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5328e-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5328e-126">JSON representation</span></span>

<span data-ttu-id="5328e-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5328e-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
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
<!--
{
  "type": "#page.annotation",
  "description": "updateRecordingStatusOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
