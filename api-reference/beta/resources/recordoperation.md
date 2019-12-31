---
title: recordOperation 资源类型
description: 包含与音频录音相关的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: aece896ffba60ca6b42a05569406a0646748039d
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912942"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="b9803-103">recordOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9803-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9803-104">包含与音频录音相关的信息。</span><span class="sxs-lookup"><span data-stu-id="b9803-104">Contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="b9803-105">属性</span><span class="sxs-lookup"><span data-stu-id="b9803-105">Properties</span></span>

| <span data-ttu-id="b9803-106">属性</span><span class="sxs-lookup"><span data-stu-id="b9803-106">Property</span></span>                       | <span data-ttu-id="b9803-107">类型</span><span class="sxs-lookup"><span data-stu-id="b9803-107">Type</span></span>                        | <span data-ttu-id="b9803-108">说明</span><span class="sxs-lookup"><span data-stu-id="b9803-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b9803-109">适用</span><span class="sxs-lookup"><span data-stu-id="b9803-109">clientContext</span></span>                  | <span data-ttu-id="b9803-110">String</span><span class="sxs-lookup"><span data-stu-id="b9803-110">String</span></span>                      | <span data-ttu-id="b9803-111">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="b9803-111">Unique Client Context string.</span></span> <span data-ttu-id="b9803-112">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="b9803-112">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="b9803-113">completionReason</span><span class="sxs-lookup"><span data-stu-id="b9803-113">completionReason</span></span>               | <span data-ttu-id="b9803-114">String</span><span class="sxs-lookup"><span data-stu-id="b9803-114">String</span></span>                      | <span data-ttu-id="b9803-115">可取值为：`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="b9803-115">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="b9803-116">id</span><span class="sxs-lookup"><span data-stu-id="b9803-116">id</span></span>                             | <span data-ttu-id="b9803-117">String</span><span class="sxs-lookup"><span data-stu-id="b9803-117">String</span></span>                      | <span data-ttu-id="b9803-118">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="b9803-118">The server operation ID.</span></span> <span data-ttu-id="b9803-119">只读。</span><span class="sxs-lookup"><span data-stu-id="b9803-119">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="b9803-120">recordingAccessToken</span><span class="sxs-lookup"><span data-stu-id="b9803-120">recordingAccessToken</span></span>           | <span data-ttu-id="b9803-121">String</span><span class="sxs-lookup"><span data-stu-id="b9803-121">String</span></span>                      | <span data-ttu-id="b9803-122">检索录制所需的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="b9803-122">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="b9803-123">recordingLocation</span><span class="sxs-lookup"><span data-stu-id="b9803-123">recordingLocation</span></span>              | <span data-ttu-id="b9803-124">String</span><span class="sxs-lookup"><span data-stu-id="b9803-124">String</span></span>                      | <span data-ttu-id="b9803-125">录制所在的位置。</span><span class="sxs-lookup"><span data-stu-id="b9803-125">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="b9803-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b9803-126">resultInfo</span></span>                     | [<span data-ttu-id="b9803-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b9803-127">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="b9803-128">结果信息。</span><span class="sxs-lookup"><span data-stu-id="b9803-128">The result information.</span></span>  <span data-ttu-id="b9803-129">只读。</span><span class="sxs-lookup"><span data-stu-id="b9803-129">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="b9803-130">状态</span><span class="sxs-lookup"><span data-stu-id="b9803-130">status</span></span>                         | <span data-ttu-id="b9803-131">String</span><span class="sxs-lookup"><span data-stu-id="b9803-131">String</span></span>                      | <span data-ttu-id="b9803-132">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b9803-132">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="b9803-133">只读。</span><span class="sxs-lookup"><span data-stu-id="b9803-133">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="b9803-134">关系</span><span class="sxs-lookup"><span data-stu-id="b9803-134">Relationships</span></span>
<span data-ttu-id="b9803-135">无。</span><span class="sxs-lookup"><span data-stu-id="b9803-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9803-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9803-136">JSON representation</span></span>

<span data-ttu-id="b9803-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9803-137">The following is a JSON representation of the resource.</span></span>

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
