---
title: recordOperation 资源类型
description: RecordOperation 类型
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 22b1fbd157b6b13d0b839a898440ee289aa2ec73
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006555"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="06dcf-103">recordOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="06dcf-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06dcf-104">RecordOperation 类型</span><span class="sxs-lookup"><span data-stu-id="06dcf-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="06dcf-105">属性</span><span class="sxs-lookup"><span data-stu-id="06dcf-105">Properties</span></span>

| <span data-ttu-id="06dcf-106">属性</span><span class="sxs-lookup"><span data-stu-id="06dcf-106">Property</span></span>                       | <span data-ttu-id="06dcf-107">类型</span><span class="sxs-lookup"><span data-stu-id="06dcf-107">Type</span></span>                        | <span data-ttu-id="06dcf-108">说明</span><span class="sxs-lookup"><span data-stu-id="06dcf-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="06dcf-109">适用</span><span class="sxs-lookup"><span data-stu-id="06dcf-109">clientContext</span></span>                  | <span data-ttu-id="06dcf-110">String</span><span class="sxs-lookup"><span data-stu-id="06dcf-110">String</span></span>                      | <span data-ttu-id="06dcf-111">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="06dcf-111">Unique Client Context string.</span></span> <span data-ttu-id="06dcf-112">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="06dcf-112">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="06dcf-113">completionReason</span><span class="sxs-lookup"><span data-stu-id="06dcf-113">completionReason</span></span>               | <span data-ttu-id="06dcf-114">String</span><span class="sxs-lookup"><span data-stu-id="06dcf-114">String</span></span>                      | <span data-ttu-id="06dcf-115">可取值为：`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="06dcf-115">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="06dcf-116">id</span><span class="sxs-lookup"><span data-stu-id="06dcf-116">id</span></span>                             | <span data-ttu-id="06dcf-117">String</span><span class="sxs-lookup"><span data-stu-id="06dcf-117">String</span></span>                      | <span data-ttu-id="06dcf-118">服务器操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="06dcf-118">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="06dcf-119">recordingAccessToken</span><span class="sxs-lookup"><span data-stu-id="06dcf-119">recordingAccessToken</span></span>           | <span data-ttu-id="06dcf-120">String</span><span class="sxs-lookup"><span data-stu-id="06dcf-120">String</span></span>                      | <span data-ttu-id="06dcf-121">检索录制所需的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="06dcf-121">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="06dcf-122">recordingLocation</span><span class="sxs-lookup"><span data-stu-id="06dcf-122">recordingLocation</span></span>              | <span data-ttu-id="06dcf-123">String</span><span class="sxs-lookup"><span data-stu-id="06dcf-123">String</span></span>                      | <span data-ttu-id="06dcf-124">录制所在的位置。</span><span class="sxs-lookup"><span data-stu-id="06dcf-124">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="06dcf-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="06dcf-125">resultInfo</span></span>                     | [<span data-ttu-id="06dcf-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="06dcf-126">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="06dcf-127">结果信息。</span><span class="sxs-lookup"><span data-stu-id="06dcf-127">The result information.</span></span>  <span data-ttu-id="06dcf-128">只读。</span><span class="sxs-lookup"><span data-stu-id="06dcf-128">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="06dcf-129">状态</span><span class="sxs-lookup"><span data-stu-id="06dcf-129">status</span></span>                         | <span data-ttu-id="06dcf-130">String</span><span class="sxs-lookup"><span data-stu-id="06dcf-130">String</span></span>                      | <span data-ttu-id="06dcf-131">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="06dcf-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="06dcf-132">只读。</span><span class="sxs-lookup"><span data-stu-id="06dcf-132">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="06dcf-133">关系</span><span class="sxs-lookup"><span data-stu-id="06dcf-133">Relationships</span></span>
<span data-ttu-id="06dcf-134">无</span><span class="sxs-lookup"><span data-stu-id="06dcf-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06dcf-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06dcf-135">JSON representation</span></span>

<span data-ttu-id="06dcf-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06dcf-136">The following is a JSON representation of the resource.</span></span>

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
