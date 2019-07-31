---
title: recordOperation 资源类型
description: RecordOperation 类型
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 00b05cd86eeb9cf8be26cdc09fb8a9b254b510db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008801"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="d6427-103">recordOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6427-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6427-104">RecordOperation 类型</span><span class="sxs-lookup"><span data-stu-id="d6427-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="d6427-105">属性</span><span class="sxs-lookup"><span data-stu-id="d6427-105">Properties</span></span>

| <span data-ttu-id="d6427-106">属性</span><span class="sxs-lookup"><span data-stu-id="d6427-106">Property</span></span>                       | <span data-ttu-id="d6427-107">类型</span><span class="sxs-lookup"><span data-stu-id="d6427-107">Type</span></span>                        | <span data-ttu-id="d6427-108">说明</span><span class="sxs-lookup"><span data-stu-id="d6427-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d6427-109">适用</span><span class="sxs-lookup"><span data-stu-id="d6427-109">clientContext</span></span>                  | <span data-ttu-id="d6427-110">String</span><span class="sxs-lookup"><span data-stu-id="d6427-110">String</span></span>                      | <span data-ttu-id="d6427-111">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="d6427-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="d6427-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="d6427-112">completionReason</span></span>               | <span data-ttu-id="d6427-113">String</span><span class="sxs-lookup"><span data-stu-id="d6427-113">String</span></span>                      | <span data-ttu-id="d6427-114">可取值为：`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="d6427-114">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="d6427-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6427-115">createdDateTime</span></span>                | <span data-ttu-id="d6427-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6427-116">DateTimeOffset</span></span>              | <span data-ttu-id="d6427-117">创建录制的时间。</span><span class="sxs-lookup"><span data-stu-id="d6427-117">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="d6427-118">id</span><span class="sxs-lookup"><span data-stu-id="d6427-118">id</span></span>                             | <span data-ttu-id="d6427-119">String</span><span class="sxs-lookup"><span data-stu-id="d6427-119">String</span></span>                      | <span data-ttu-id="d6427-120">服务器操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="d6427-120">The server operation id. Read-only.</span></span> <span data-ttu-id="d6427-121">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="d6427-121">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="d6427-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="d6427-122">lastActionDateTime</span></span>             | <span data-ttu-id="d6427-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6427-123">DateTimeOffset</span></span>              | <span data-ttu-id="d6427-124">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="d6427-124">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="d6427-125">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="d6427-125">recordResourceAccessToken</span></span>      | <span data-ttu-id="d6427-126">String</span><span class="sxs-lookup"><span data-stu-id="d6427-126">String</span></span>                      | <span data-ttu-id="d6427-127">检索录制所需的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="d6427-127">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="d6427-128">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="d6427-128">recordResourceLocation</span></span>         | <span data-ttu-id="d6427-129">String</span><span class="sxs-lookup"><span data-stu-id="d6427-129">String</span></span>                      | <span data-ttu-id="d6427-130">录制所在的位置。</span><span class="sxs-lookup"><span data-stu-id="d6427-130">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="d6427-131">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d6427-131">resultInfo</span></span>                     | [<span data-ttu-id="d6427-132">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d6427-132">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="d6427-133">结果信息。</span><span class="sxs-lookup"><span data-stu-id="d6427-133">The result information.</span></span>  <span data-ttu-id="d6427-134">只读。</span><span class="sxs-lookup"><span data-stu-id="d6427-134">Read-only.</span></span> <span data-ttu-id="d6427-135">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="d6427-135">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="d6427-136">status</span><span class="sxs-lookup"><span data-stu-id="d6427-136">status</span></span>                         | <span data-ttu-id="d6427-137">String</span><span class="sxs-lookup"><span data-stu-id="d6427-137">String</span></span>                      | <span data-ttu-id="d6427-138">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="d6427-138">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="d6427-139">只读。</span><span class="sxs-lookup"><span data-stu-id="d6427-139">Read-only.</span></span> <span data-ttu-id="d6427-140">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="d6427-140">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="d6427-141">关系</span><span class="sxs-lookup"><span data-stu-id="d6427-141">Relationships</span></span>
<span data-ttu-id="d6427-142">无</span><span class="sxs-lookup"><span data-stu-id="d6427-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6427-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6427-143">JSON representation</span></span>

<span data-ttu-id="d6427-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6427-144">The following is a JSON representation of the resource.</span></span>

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
  "recordResourceAccessToken": "String",
  "recordResourceLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="d6427-145">示例</span><span class="sxs-lookup"><span data-stu-id="d6427-145">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.recordOperation",
  "truncated": true
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceAccessToken": "<access-token>",
  "recordResourceLocation": "https://resource.location/ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
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
