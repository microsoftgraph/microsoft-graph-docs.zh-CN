---
title: recordOperation 资源类型
description: RecordOperation 类型
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2fdf8b6f1f00429e676d778c0095d4554fff4a18
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948742"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="cde82-103">recordOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="cde82-103">recordOperation resource type</span></span>

> <span data-ttu-id="cde82-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cde82-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cde82-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cde82-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cde82-106">RecordOperation 类型</span><span class="sxs-lookup"><span data-stu-id="cde82-106">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="cde82-107">属性</span><span class="sxs-lookup"><span data-stu-id="cde82-107">Properties</span></span>

| <span data-ttu-id="cde82-108">属性</span><span class="sxs-lookup"><span data-stu-id="cde82-108">Property</span></span>                       | <span data-ttu-id="cde82-109">类型</span><span class="sxs-lookup"><span data-stu-id="cde82-109">Type</span></span>                        | <span data-ttu-id="cde82-110">说明</span><span class="sxs-lookup"><span data-stu-id="cde82-110">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cde82-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="cde82-111">clientContext</span></span>                  | <span data-ttu-id="cde82-112">字符串</span><span class="sxs-lookup"><span data-stu-id="cde82-112">String</span></span>                      | <span data-ttu-id="cde82-113">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="cde82-113">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="cde82-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="cde82-114">completionReason</span></span>               | <span data-ttu-id="cde82-115">字符串</span><span class="sxs-lookup"><span data-stu-id="cde82-115">String</span></span>                      | <span data-ttu-id="cde82-116">可取值为：`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="cde82-116">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="cde82-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cde82-117">createdDateTime</span></span>                | <span data-ttu-id="cde82-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cde82-118">DateTimeOffset</span></span>              | <span data-ttu-id="cde82-119">录制已创建的时间。</span><span class="sxs-lookup"><span data-stu-id="cde82-119">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="cde82-120">id</span><span class="sxs-lookup"><span data-stu-id="cde82-120">id</span></span>                             | <span data-ttu-id="cde82-121">字符串</span><span class="sxs-lookup"><span data-stu-id="cde82-121">String</span></span>                      | <span data-ttu-id="cde82-122">服务器操作 id。只读的。</span><span class="sxs-lookup"><span data-stu-id="cde82-122">The server operation id. Read-only.</span></span> <span data-ttu-id="cde82-123">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="cde82-123">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="cde82-124">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="cde82-124">lastActionDateTime</span></span>             | <span data-ttu-id="cde82-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cde82-125">DateTimeOffset</span></span>              | <span data-ttu-id="cde82-126">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="cde82-126">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="cde82-127">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="cde82-127">recordResourceAccessToken</span></span>      | <span data-ttu-id="cde82-128">字符串</span><span class="sxs-lookup"><span data-stu-id="cde82-128">String</span></span>                      | <span data-ttu-id="cde82-129">要检索录制，需要访问令牌。</span><span class="sxs-lookup"><span data-stu-id="cde82-129">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="cde82-130">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="cde82-130">recordResourceLocation</span></span>         | <span data-ttu-id="cde82-131">字符串</span><span class="sxs-lookup"><span data-stu-id="cde82-131">String</span></span>                      | <span data-ttu-id="cde82-132">录制所在位置。</span><span class="sxs-lookup"><span data-stu-id="cde82-132">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="cde82-133">resultInfo</span><span class="sxs-lookup"><span data-stu-id="cde82-133">resultInfo</span></span>                     | [<span data-ttu-id="cde82-134">resultInfo</span><span class="sxs-lookup"><span data-stu-id="cde82-134">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="cde82-135">结果的信息。</span><span class="sxs-lookup"><span data-stu-id="cde82-135">The result information.</span></span>  <span data-ttu-id="cde82-136">只读。</span><span class="sxs-lookup"><span data-stu-id="cde82-136">Read-only.</span></span> <span data-ttu-id="cde82-137">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="cde82-137">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="cde82-138">status</span><span class="sxs-lookup"><span data-stu-id="cde82-138">status</span></span>                         | <span data-ttu-id="cde82-139">String</span><span class="sxs-lookup"><span data-stu-id="cde82-139">String</span></span>                      | <span data-ttu-id="cde82-140">可取值为 `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="cde82-140">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="cde82-141">只读。</span><span class="sxs-lookup"><span data-stu-id="cde82-141">Read-only.</span></span> <span data-ttu-id="cde82-142">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="cde82-142">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="cde82-143">Relationships</span><span class="sxs-lookup"><span data-stu-id="cde82-143">Relationships</span></span>
<span data-ttu-id="cde82-144">无</span><span class="sxs-lookup"><span data-stu-id="cde82-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cde82-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cde82-145">JSON representation</span></span>

<span data-ttu-id="cde82-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cde82-146">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="cde82-147">示例</span><span class="sxs-lookup"><span data-stu-id="cde82-147">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
