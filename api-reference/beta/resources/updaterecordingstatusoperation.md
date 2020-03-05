---
title: updateRecordingStatusOperation 资源类型
description: 介绍更新录制状态操作的响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b27aca68e159775bc9e4559d1ff6d5c005c9929a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519587"
---
# <a name="updaterecordingstatusoperation-resource-type"></a><span data-ttu-id="d2b76-103">updateRecordingStatusOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2b76-103">updateRecordingStatusOperation resource type</span></span>

<span data-ttu-id="d2b76-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d2b76-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2b76-105">介绍更新录制状态操作的响应格式。</span><span class="sxs-lookup"><span data-stu-id="d2b76-105">Describes the response format of an update recording status action.</span></span>

## <a name="properties"></a><span data-ttu-id="d2b76-106">属性</span><span class="sxs-lookup"><span data-stu-id="d2b76-106">Properties</span></span>

| <span data-ttu-id="d2b76-107">属性</span><span class="sxs-lookup"><span data-stu-id="d2b76-107">Property</span></span>            | <span data-ttu-id="d2b76-108">类型</span><span class="sxs-lookup"><span data-stu-id="d2b76-108">Type</span></span>                        | <span data-ttu-id="d2b76-109">说明</span><span class="sxs-lookup"><span data-stu-id="d2b76-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="d2b76-110">适用</span><span class="sxs-lookup"><span data-stu-id="d2b76-110">clientContext</span></span>       | <span data-ttu-id="d2b76-111">String</span><span class="sxs-lookup"><span data-stu-id="d2b76-111">String</span></span>                      | <span data-ttu-id="d2b76-112">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="d2b76-112">Unique Client Context string.</span></span> <span data-ttu-id="d2b76-113">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="d2b76-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="d2b76-114">id</span><span class="sxs-lookup"><span data-stu-id="d2b76-114">id</span></span>                  | <span data-ttu-id="d2b76-115">字符串</span><span class="sxs-lookup"><span data-stu-id="d2b76-115">String</span></span>                      | <span data-ttu-id="d2b76-116">只读。</span><span class="sxs-lookup"><span data-stu-id="d2b76-116">Read-only.</span></span>                                                                         |
| <span data-ttu-id="d2b76-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d2b76-117">resultInfo</span></span>          | [<span data-ttu-id="d2b76-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d2b76-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="d2b76-119">结果信息。</span><span class="sxs-lookup"><span data-stu-id="d2b76-119">The result information.</span></span> <span data-ttu-id="d2b76-120">只读。</span><span class="sxs-lookup"><span data-stu-id="d2b76-120">Read-only.</span></span>                                                 |
| <span data-ttu-id="d2b76-121">status</span><span class="sxs-lookup"><span data-stu-id="d2b76-121">status</span></span>              | <span data-ttu-id="d2b76-122">String</span><span class="sxs-lookup"><span data-stu-id="d2b76-122">String</span></span>                      | <span data-ttu-id="d2b76-123">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="d2b76-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="d2b76-124">关系</span><span class="sxs-lookup"><span data-stu-id="d2b76-124">Relationships</span></span>
<span data-ttu-id="d2b76-125">无</span><span class="sxs-lookup"><span data-stu-id="d2b76-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2b76-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2b76-126">JSON representation</span></span>

<span data-ttu-id="d2b76-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2b76-127">The following is a JSON representation of the resource.</span></span>

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
