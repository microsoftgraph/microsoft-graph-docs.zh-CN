---
title: recordOperation 资源类型
description: 此资源类型包含与音频录音相关的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 508404a3360b2b59656dc31df6ec44f16f682cf4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991892"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="60490-103">recordOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="60490-103">recordOperation resource type</span></span>

<span data-ttu-id="60490-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60490-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60490-105">此资源类型包含与音频录音相关的信息。</span><span class="sxs-lookup"><span data-stu-id="60490-105">This resource type contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="60490-106">属性</span><span class="sxs-lookup"><span data-stu-id="60490-106">Properties</span></span>

| <span data-ttu-id="60490-107">属性</span><span class="sxs-lookup"><span data-stu-id="60490-107">Property</span></span>                       | <span data-ttu-id="60490-108">类型</span><span class="sxs-lookup"><span data-stu-id="60490-108">Type</span></span>                        | <span data-ttu-id="60490-109">说明</span><span class="sxs-lookup"><span data-stu-id="60490-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="60490-110">适用</span><span class="sxs-lookup"><span data-stu-id="60490-110">clientContext</span></span>                  | <span data-ttu-id="60490-111">String</span><span class="sxs-lookup"><span data-stu-id="60490-111">String</span></span>                      | <span data-ttu-id="60490-112">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="60490-112">Unique Client Context string.</span></span> <span data-ttu-id="60490-113">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="60490-113">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="60490-114">id</span><span class="sxs-lookup"><span data-stu-id="60490-114">id</span></span>                             | <span data-ttu-id="60490-115">String</span><span class="sxs-lookup"><span data-stu-id="60490-115">String</span></span>                      | <span data-ttu-id="60490-116">服务器操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="60490-116">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="60490-117">recordingAccessToken</span><span class="sxs-lookup"><span data-stu-id="60490-117">recordingAccessToken</span></span>           | <span data-ttu-id="60490-118">String</span><span class="sxs-lookup"><span data-stu-id="60490-118">String</span></span>                      | <span data-ttu-id="60490-119">检索录制所需的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="60490-119">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="60490-120">recordingLocation</span><span class="sxs-lookup"><span data-stu-id="60490-120">recordingLocation</span></span>              | <span data-ttu-id="60490-121">String</span><span class="sxs-lookup"><span data-stu-id="60490-121">String</span></span>                      | <span data-ttu-id="60490-122">录制所在的位置。</span><span class="sxs-lookup"><span data-stu-id="60490-122">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="60490-123">resultInfo</span><span class="sxs-lookup"><span data-stu-id="60490-123">resultInfo</span></span>                     | [<span data-ttu-id="60490-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="60490-124">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="60490-125">结果信息。</span><span class="sxs-lookup"><span data-stu-id="60490-125">The result information.</span></span>  <span data-ttu-id="60490-126">只读。</span><span class="sxs-lookup"><span data-stu-id="60490-126">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="60490-127">状态</span><span class="sxs-lookup"><span data-stu-id="60490-127">status</span></span>                         | <span data-ttu-id="60490-128">String</span><span class="sxs-lookup"><span data-stu-id="60490-128">String</span></span>                      | <span data-ttu-id="60490-129">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="60490-129">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="60490-130">只读。</span><span class="sxs-lookup"><span data-stu-id="60490-130">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="60490-131">关系</span><span class="sxs-lookup"><span data-stu-id="60490-131">Relationships</span></span>
<span data-ttu-id="60490-132">无</span><span class="sxs-lookup"><span data-stu-id="60490-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60490-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60490-133">JSON representation</span></span>

<span data-ttu-id="60490-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60490-134">The following is a JSON representation of the resource.</span></span>

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

