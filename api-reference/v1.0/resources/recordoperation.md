---
title: recordOperation 资源类型
description: 此资源类型包含与音频录音相关的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b4f0a62204a6ee1db7e75caf9044288f705a5529
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865768"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="03352-103">recordOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="03352-103">recordOperation resource type</span></span>

<span data-ttu-id="03352-104">此资源类型包含与音频录音相关的信息。</span><span class="sxs-lookup"><span data-stu-id="03352-104">This resource type contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="03352-105">属性</span><span class="sxs-lookup"><span data-stu-id="03352-105">Properties</span></span>

| <span data-ttu-id="03352-106">属性</span><span class="sxs-lookup"><span data-stu-id="03352-106">Property</span></span>                       | <span data-ttu-id="03352-107">类型</span><span class="sxs-lookup"><span data-stu-id="03352-107">Type</span></span>                        | <span data-ttu-id="03352-108">说明</span><span class="sxs-lookup"><span data-stu-id="03352-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="03352-109">适用</span><span class="sxs-lookup"><span data-stu-id="03352-109">clientContext</span></span>                  | <span data-ttu-id="03352-110">String</span><span class="sxs-lookup"><span data-stu-id="03352-110">String</span></span>                      | <span data-ttu-id="03352-111">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="03352-111">Unique Client Context string.</span></span> <span data-ttu-id="03352-112">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="03352-112">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="03352-113">id</span><span class="sxs-lookup"><span data-stu-id="03352-113">id</span></span>                             | <span data-ttu-id="03352-114">String</span><span class="sxs-lookup"><span data-stu-id="03352-114">String</span></span>                      | <span data-ttu-id="03352-115">服务器操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="03352-115">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="03352-116">recordingAccessToken</span><span class="sxs-lookup"><span data-stu-id="03352-116">recordingAccessToken</span></span>           | <span data-ttu-id="03352-117">String</span><span class="sxs-lookup"><span data-stu-id="03352-117">String</span></span>                      | <span data-ttu-id="03352-118">检索录制所需的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="03352-118">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="03352-119">recordingLocation</span><span class="sxs-lookup"><span data-stu-id="03352-119">recordingLocation</span></span>              | <span data-ttu-id="03352-120">String</span><span class="sxs-lookup"><span data-stu-id="03352-120">String</span></span>                      | <span data-ttu-id="03352-121">录制所在的位置。</span><span class="sxs-lookup"><span data-stu-id="03352-121">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="03352-122">resultInfo</span><span class="sxs-lookup"><span data-stu-id="03352-122">resultInfo</span></span>                     | [<span data-ttu-id="03352-123">resultInfo</span><span class="sxs-lookup"><span data-stu-id="03352-123">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="03352-124">结果信息。</span><span class="sxs-lookup"><span data-stu-id="03352-124">The result information.</span></span>  <span data-ttu-id="03352-125">只读。</span><span class="sxs-lookup"><span data-stu-id="03352-125">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="03352-126">状态</span><span class="sxs-lookup"><span data-stu-id="03352-126">status</span></span>                         | <span data-ttu-id="03352-127">String</span><span class="sxs-lookup"><span data-stu-id="03352-127">String</span></span>                      | <span data-ttu-id="03352-128">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="03352-128">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="03352-129">只读。</span><span class="sxs-lookup"><span data-stu-id="03352-129">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="03352-130">关系</span><span class="sxs-lookup"><span data-stu-id="03352-130">Relationships</span></span>
<span data-ttu-id="03352-131">无</span><span class="sxs-lookup"><span data-stu-id="03352-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03352-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03352-132">JSON representation</span></span>

<span data-ttu-id="03352-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03352-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "recordingAccessToken": "String",
  "recordingLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
