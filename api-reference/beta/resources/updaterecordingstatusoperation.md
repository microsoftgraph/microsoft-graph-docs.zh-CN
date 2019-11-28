---
title: updateRecordingStatusOperation 资源类型
description: 介绍更新录制状态操作的响应格式。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 92cfc481d10cccd3752db29a0c1da7d46000ed3b
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636917"
---
# <a name="updaterecordingstatusoperation-resource-type"></a><span data-ttu-id="dc7f4-103">updateRecordingStatusOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc7f4-103">updateRecordingStatusOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc7f4-104">介绍更新录制状态操作的响应格式。</span><span class="sxs-lookup"><span data-stu-id="dc7f4-104">Describes the response format of an update recording status action.</span></span>

## <a name="properties"></a><span data-ttu-id="dc7f4-105">属性</span><span class="sxs-lookup"><span data-stu-id="dc7f4-105">Properties</span></span>

| <span data-ttu-id="dc7f4-106">属性</span><span class="sxs-lookup"><span data-stu-id="dc7f4-106">Property</span></span>            | <span data-ttu-id="dc7f4-107">类型</span><span class="sxs-lookup"><span data-stu-id="dc7f4-107">Type</span></span>                        | <span data-ttu-id="dc7f4-108">说明</span><span class="sxs-lookup"><span data-stu-id="dc7f4-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="dc7f4-109">适用</span><span class="sxs-lookup"><span data-stu-id="dc7f4-109">clientContext</span></span>       | <span data-ttu-id="dc7f4-110">String</span><span class="sxs-lookup"><span data-stu-id="dc7f4-110">String</span></span>                      | <span data-ttu-id="dc7f4-111">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="dc7f4-111">Unique Client Context string.</span></span> <span data-ttu-id="dc7f4-112">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="dc7f4-112">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="dc7f4-113">id</span><span class="sxs-lookup"><span data-stu-id="dc7f4-113">id</span></span>                  | <span data-ttu-id="dc7f4-114">字符串</span><span class="sxs-lookup"><span data-stu-id="dc7f4-114">String</span></span>                      | <span data-ttu-id="dc7f4-115">只读。</span><span class="sxs-lookup"><span data-stu-id="dc7f4-115">Read-only.</span></span>                                                                         |
| <span data-ttu-id="dc7f4-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="dc7f4-116">resultInfo</span></span>          | [<span data-ttu-id="dc7f4-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="dc7f4-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="dc7f4-118">结果信息。</span><span class="sxs-lookup"><span data-stu-id="dc7f4-118">The result information.</span></span> <span data-ttu-id="dc7f4-119">只读。</span><span class="sxs-lookup"><span data-stu-id="dc7f4-119">Read-only.</span></span>                                                 |
| <span data-ttu-id="dc7f4-120">状态</span><span class="sxs-lookup"><span data-stu-id="dc7f4-120">status</span></span>              | <span data-ttu-id="dc7f4-121">String</span><span class="sxs-lookup"><span data-stu-id="dc7f4-121">String</span></span>                      | <span data-ttu-id="dc7f4-122">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="dc7f4-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="dc7f4-123">关系</span><span class="sxs-lookup"><span data-stu-id="dc7f4-123">Relationships</span></span>
<span data-ttu-id="dc7f4-124">无</span><span class="sxs-lookup"><span data-stu-id="dc7f4-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc7f4-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc7f4-125">JSON representation</span></span>

<span data-ttu-id="dc7f4-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc7f4-126">The following is a JSON representation of the resource.</span></span>

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
