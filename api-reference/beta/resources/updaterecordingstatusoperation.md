---
title: updateRecordingStatusOperation 资源类型
description: 介绍更新录制状态操作的响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 302ea2c5ce0cfb54168bf936f8c6e5829e0867c7
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913280"
---
# <a name="updaterecordingstatusoperation-resource-type"></a><span data-ttu-id="ddc98-103">updateRecordingStatusOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ddc98-103">updateRecordingStatusOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddc98-104">介绍更新录制状态操作的响应格式。</span><span class="sxs-lookup"><span data-stu-id="ddc98-104">Describes the response format of an update recording status action.</span></span>

## <a name="properties"></a><span data-ttu-id="ddc98-105">属性</span><span class="sxs-lookup"><span data-stu-id="ddc98-105">Properties</span></span>

| <span data-ttu-id="ddc98-106">属性</span><span class="sxs-lookup"><span data-stu-id="ddc98-106">Property</span></span>            | <span data-ttu-id="ddc98-107">类型</span><span class="sxs-lookup"><span data-stu-id="ddc98-107">Type</span></span>                        | <span data-ttu-id="ddc98-108">说明</span><span class="sxs-lookup"><span data-stu-id="ddc98-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="ddc98-109">适用</span><span class="sxs-lookup"><span data-stu-id="ddc98-109">clientContext</span></span>       | <span data-ttu-id="ddc98-110">String</span><span class="sxs-lookup"><span data-stu-id="ddc98-110">String</span></span>                      | <span data-ttu-id="ddc98-111">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="ddc98-111">Unique Client Context string.</span></span> <span data-ttu-id="ddc98-112">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="ddc98-112">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="ddc98-113">id</span><span class="sxs-lookup"><span data-stu-id="ddc98-113">id</span></span>                  | <span data-ttu-id="ddc98-114">字符串</span><span class="sxs-lookup"><span data-stu-id="ddc98-114">String</span></span>                      | <span data-ttu-id="ddc98-115">只读。</span><span class="sxs-lookup"><span data-stu-id="ddc98-115">Read-only.</span></span>                                                                         |
| <span data-ttu-id="ddc98-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="ddc98-116">resultInfo</span></span>          | [<span data-ttu-id="ddc98-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="ddc98-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="ddc98-118">结果信息。</span><span class="sxs-lookup"><span data-stu-id="ddc98-118">The result information.</span></span> <span data-ttu-id="ddc98-119">只读。</span><span class="sxs-lookup"><span data-stu-id="ddc98-119">Read-only.</span></span>                                                 |
| <span data-ttu-id="ddc98-120">状态</span><span class="sxs-lookup"><span data-stu-id="ddc98-120">status</span></span>              | <span data-ttu-id="ddc98-121">String</span><span class="sxs-lookup"><span data-stu-id="ddc98-121">String</span></span>                      | <span data-ttu-id="ddc98-122">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="ddc98-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="ddc98-123">关系</span><span class="sxs-lookup"><span data-stu-id="ddc98-123">Relationships</span></span>
<span data-ttu-id="ddc98-124">无</span><span class="sxs-lookup"><span data-stu-id="ddc98-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddc98-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ddc98-125">JSON representation</span></span>

<span data-ttu-id="ddc98-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ddc98-126">The following is a JSON representation of the resource.</span></span>

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
