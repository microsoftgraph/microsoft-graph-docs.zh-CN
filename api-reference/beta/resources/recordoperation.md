---
title: recordOperation 资源类型
description: 包含与音频录音相关的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ccf7f4b196866ccc8f038047a29f4b3dabd96642
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055153"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="d2e45-103">recordOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2e45-103">recordOperation resource type</span></span>

<span data-ttu-id="d2e45-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2e45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2e45-105">包含与音频录音相关的信息。</span><span class="sxs-lookup"><span data-stu-id="d2e45-105">Contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="d2e45-106">属性</span><span class="sxs-lookup"><span data-stu-id="d2e45-106">Properties</span></span>

| <span data-ttu-id="d2e45-107">属性</span><span class="sxs-lookup"><span data-stu-id="d2e45-107">Property</span></span>                       | <span data-ttu-id="d2e45-108">类型</span><span class="sxs-lookup"><span data-stu-id="d2e45-108">Type</span></span>                        | <span data-ttu-id="d2e45-109">说明</span><span class="sxs-lookup"><span data-stu-id="d2e45-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d2e45-110">适用</span><span class="sxs-lookup"><span data-stu-id="d2e45-110">clientContext</span></span>                  | <span data-ttu-id="d2e45-111">String</span><span class="sxs-lookup"><span data-stu-id="d2e45-111">String</span></span>                      | <span data-ttu-id="d2e45-112">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="d2e45-112">Unique Client Context string.</span></span> <span data-ttu-id="d2e45-113">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="d2e45-113">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="d2e45-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="d2e45-114">completionReason</span></span>               | <span data-ttu-id="d2e45-115">String</span><span class="sxs-lookup"><span data-stu-id="d2e45-115">String</span></span>                      | <span data-ttu-id="d2e45-116">可取值为：`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="d2e45-116">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="d2e45-117">id</span><span class="sxs-lookup"><span data-stu-id="d2e45-117">id</span></span>                             | <span data-ttu-id="d2e45-118">String</span><span class="sxs-lookup"><span data-stu-id="d2e45-118">String</span></span>                      | <span data-ttu-id="d2e45-119">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="d2e45-119">The server operation ID.</span></span> <span data-ttu-id="d2e45-120">只读。</span><span class="sxs-lookup"><span data-stu-id="d2e45-120">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="d2e45-121">recordingAccessToken</span><span class="sxs-lookup"><span data-stu-id="d2e45-121">recordingAccessToken</span></span>           | <span data-ttu-id="d2e45-122">String</span><span class="sxs-lookup"><span data-stu-id="d2e45-122">String</span></span>                      | <span data-ttu-id="d2e45-123">检索录制所需的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="d2e45-123">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="d2e45-124">recordingLocation</span><span class="sxs-lookup"><span data-stu-id="d2e45-124">recordingLocation</span></span>              | <span data-ttu-id="d2e45-125">String</span><span class="sxs-lookup"><span data-stu-id="d2e45-125">String</span></span>                      | <span data-ttu-id="d2e45-126">录制所在的位置。</span><span class="sxs-lookup"><span data-stu-id="d2e45-126">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="d2e45-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d2e45-127">resultInfo</span></span>                     | [<span data-ttu-id="d2e45-128">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d2e45-128">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="d2e45-129">结果信息。</span><span class="sxs-lookup"><span data-stu-id="d2e45-129">The result information.</span></span>  <span data-ttu-id="d2e45-130">只读。</span><span class="sxs-lookup"><span data-stu-id="d2e45-130">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="d2e45-131">状态</span><span class="sxs-lookup"><span data-stu-id="d2e45-131">status</span></span>                         | <span data-ttu-id="d2e45-132">String</span><span class="sxs-lookup"><span data-stu-id="d2e45-132">String</span></span>                      | <span data-ttu-id="d2e45-133">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="d2e45-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="d2e45-134">只读。</span><span class="sxs-lookup"><span data-stu-id="d2e45-134">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="d2e45-135">关系</span><span class="sxs-lookup"><span data-stu-id="d2e45-135">Relationships</span></span>
<span data-ttu-id="d2e45-136">无。</span><span class="sxs-lookup"><span data-stu-id="d2e45-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2e45-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2e45-137">JSON representation</span></span>

<span data-ttu-id="d2e45-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2e45-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError | none",
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


