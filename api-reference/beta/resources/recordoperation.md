---
title: recordOperation 资源类型
description: RecordOperation 类型
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 23fb116a80dcd90206d7a0ae5eeec5d756272c3d
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/02/2019
ms.locfileid: "36061996"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="378ff-103">recordOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="378ff-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="378ff-104">RecordOperation 类型</span><span class="sxs-lookup"><span data-stu-id="378ff-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="378ff-105">属性</span><span class="sxs-lookup"><span data-stu-id="378ff-105">Properties</span></span>

| <span data-ttu-id="378ff-106">属性</span><span class="sxs-lookup"><span data-stu-id="378ff-106">Property</span></span>                       | <span data-ttu-id="378ff-107">类型</span><span class="sxs-lookup"><span data-stu-id="378ff-107">Type</span></span>                        | <span data-ttu-id="378ff-108">说明</span><span class="sxs-lookup"><span data-stu-id="378ff-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="378ff-109">适用</span><span class="sxs-lookup"><span data-stu-id="378ff-109">clientContext</span></span>                  | <span data-ttu-id="378ff-110">String</span><span class="sxs-lookup"><span data-stu-id="378ff-110">String</span></span>                      | <span data-ttu-id="378ff-111">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="378ff-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="378ff-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="378ff-112">completionReason</span></span>               | <span data-ttu-id="378ff-113">String</span><span class="sxs-lookup"><span data-stu-id="378ff-113">String</span></span>                      | <span data-ttu-id="378ff-114">可取值为：`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="378ff-114">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="378ff-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="378ff-115">createdDateTime</span></span>                | <span data-ttu-id="378ff-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="378ff-116">DateTimeOffset</span></span>              | <span data-ttu-id="378ff-117">创建录制的时间。</span><span class="sxs-lookup"><span data-stu-id="378ff-117">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="378ff-118">id</span><span class="sxs-lookup"><span data-stu-id="378ff-118">id</span></span>                             | <span data-ttu-id="378ff-119">String</span><span class="sxs-lookup"><span data-stu-id="378ff-119">String</span></span>                      | <span data-ttu-id="378ff-120">服务器操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="378ff-120">The server operation id. Read-only.</span></span> <span data-ttu-id="378ff-121">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="378ff-121">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="378ff-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="378ff-122">lastActionDateTime</span></span>             | <span data-ttu-id="378ff-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="378ff-123">DateTimeOffset</span></span>              | <span data-ttu-id="378ff-124">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="378ff-124">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="378ff-125">recordingAccessToken</span><span class="sxs-lookup"><span data-stu-id="378ff-125">recordingAccessToken</span></span>           | <span data-ttu-id="378ff-126">String</span><span class="sxs-lookup"><span data-stu-id="378ff-126">String</span></span>                      | <span data-ttu-id="378ff-127">检索录制所需的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="378ff-127">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="378ff-128">recordingLocation</span><span class="sxs-lookup"><span data-stu-id="378ff-128">recordingLocation</span></span>              | <span data-ttu-id="378ff-129">String</span><span class="sxs-lookup"><span data-stu-id="378ff-129">String</span></span>                      | <span data-ttu-id="378ff-130">录制所在的位置。</span><span class="sxs-lookup"><span data-stu-id="378ff-130">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="378ff-131">resultInfo</span><span class="sxs-lookup"><span data-stu-id="378ff-131">resultInfo</span></span>                     | [<span data-ttu-id="378ff-132">resultInfo</span><span class="sxs-lookup"><span data-stu-id="378ff-132">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="378ff-133">结果信息。</span><span class="sxs-lookup"><span data-stu-id="378ff-133">The result information.</span></span>  <span data-ttu-id="378ff-134">只读。</span><span class="sxs-lookup"><span data-stu-id="378ff-134">Read-only.</span></span> <span data-ttu-id="378ff-135">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="378ff-135">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="378ff-136">status</span><span class="sxs-lookup"><span data-stu-id="378ff-136">status</span></span>                         | <span data-ttu-id="378ff-137">String</span><span class="sxs-lookup"><span data-stu-id="378ff-137">String</span></span>                      | <span data-ttu-id="378ff-138">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="378ff-138">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="378ff-139">只读。</span><span class="sxs-lookup"><span data-stu-id="378ff-139">Read-only.</span></span> <span data-ttu-id="378ff-140">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="378ff-140">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="378ff-141">关系</span><span class="sxs-lookup"><span data-stu-id="378ff-141">Relationships</span></span>
<span data-ttu-id="378ff-142">无</span><span class="sxs-lookup"><span data-stu-id="378ff-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="378ff-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="378ff-143">JSON representation</span></span>

<span data-ttu-id="378ff-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="378ff-144">The following is a JSON representation of the resource.</span></span>

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
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordingAccessToken": "String",
  "recordingLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="378ff-145">示例</span><span class="sxs-lookup"><span data-stu-id="378ff-145">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.recordOperation",
  "truncated": true
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordingAccessToken": "<access-token>",
  "recordingLocation": "https://resource.location/ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "status": "completed"
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
