---
title: recordOperation 资源类型
description: 包含与音频录音相关的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 837540c55bb6573828efe87ee0c7ae333335ea11
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870136"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="2a545-103">recordOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a545-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a545-104">包含与音频录音相关的信息。</span><span class="sxs-lookup"><span data-stu-id="2a545-104">Contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="2a545-105">属性</span><span class="sxs-lookup"><span data-stu-id="2a545-105">Properties</span></span>

| <span data-ttu-id="2a545-106">属性</span><span class="sxs-lookup"><span data-stu-id="2a545-106">Property</span></span>                       | <span data-ttu-id="2a545-107">类型</span><span class="sxs-lookup"><span data-stu-id="2a545-107">Type</span></span>                        | <span data-ttu-id="2a545-108">说明</span><span class="sxs-lookup"><span data-stu-id="2a545-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2a545-109">适用</span><span class="sxs-lookup"><span data-stu-id="2a545-109">clientContext</span></span>                  | <span data-ttu-id="2a545-110">String</span><span class="sxs-lookup"><span data-stu-id="2a545-110">String</span></span>                      | <span data-ttu-id="2a545-111">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="2a545-111">Unique Client Context string.</span></span> <span data-ttu-id="2a545-112">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="2a545-112">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="2a545-113">completionReason</span><span class="sxs-lookup"><span data-stu-id="2a545-113">completionReason</span></span>               | <span data-ttu-id="2a545-114">String</span><span class="sxs-lookup"><span data-stu-id="2a545-114">String</span></span>                      | <span data-ttu-id="2a545-115">可取值为：`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="2a545-115">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="2a545-116">id</span><span class="sxs-lookup"><span data-stu-id="2a545-116">id</span></span>                             | <span data-ttu-id="2a545-117">String</span><span class="sxs-lookup"><span data-stu-id="2a545-117">String</span></span>                      | <span data-ttu-id="2a545-118">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="2a545-118">The server operation ID.</span></span> <span data-ttu-id="2a545-119">只读。</span><span class="sxs-lookup"><span data-stu-id="2a545-119">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="2a545-120">recordingAccessToken</span><span class="sxs-lookup"><span data-stu-id="2a545-120">recordingAccessToken</span></span>           | <span data-ttu-id="2a545-121">String</span><span class="sxs-lookup"><span data-stu-id="2a545-121">String</span></span>                      | <span data-ttu-id="2a545-122">检索录制所需的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="2a545-122">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="2a545-123">recordingLocation</span><span class="sxs-lookup"><span data-stu-id="2a545-123">recordingLocation</span></span>              | <span data-ttu-id="2a545-124">String</span><span class="sxs-lookup"><span data-stu-id="2a545-124">String</span></span>                      | <span data-ttu-id="2a545-125">录制所在的位置。</span><span class="sxs-lookup"><span data-stu-id="2a545-125">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="2a545-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="2a545-126">resultInfo</span></span>                     | [<span data-ttu-id="2a545-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="2a545-127">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="2a545-128">结果信息。</span><span class="sxs-lookup"><span data-stu-id="2a545-128">The result information.</span></span>  <span data-ttu-id="2a545-129">只读。</span><span class="sxs-lookup"><span data-stu-id="2a545-129">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="2a545-130">状态</span><span class="sxs-lookup"><span data-stu-id="2a545-130">status</span></span>                         | <span data-ttu-id="2a545-131">String</span><span class="sxs-lookup"><span data-stu-id="2a545-131">String</span></span>                      | <span data-ttu-id="2a545-132">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="2a545-132">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="2a545-133">只读。</span><span class="sxs-lookup"><span data-stu-id="2a545-133">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="2a545-134">关系</span><span class="sxs-lookup"><span data-stu-id="2a545-134">Relationships</span></span>
<span data-ttu-id="2a545-135">无。</span><span class="sxs-lookup"><span data-stu-id="2a545-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a545-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a545-136">JSON representation</span></span>

<span data-ttu-id="2a545-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a545-137">The following is a JSON representation of the resource.</span></span>

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
