---
title: recordOperation 资源类型
description: RecordOperation 类型
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: be6a124fcd7175489679a8c2392218530d510e9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880015"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="31d04-103">recordOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="31d04-103">recordOperation resource type</span></span>

> <span data-ttu-id="31d04-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="31d04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31d04-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="31d04-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="31d04-106">RecordOperation 类型</span><span class="sxs-lookup"><span data-stu-id="31d04-106">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="31d04-107">属性</span><span class="sxs-lookup"><span data-stu-id="31d04-107">Properties</span></span>

| <span data-ttu-id="31d04-108">属性</span><span class="sxs-lookup"><span data-stu-id="31d04-108">Property</span></span>                       | <span data-ttu-id="31d04-109">类型</span><span class="sxs-lookup"><span data-stu-id="31d04-109">Type</span></span>                        | <span data-ttu-id="31d04-110">Description</span><span class="sxs-lookup"><span data-stu-id="31d04-110">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="31d04-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="31d04-111">clientContext</span></span>                  | <span data-ttu-id="31d04-112">字符串</span><span class="sxs-lookup"><span data-stu-id="31d04-112">String</span></span>                      | <span data-ttu-id="31d04-113">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="31d04-113">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="31d04-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="31d04-114">completionReason</span></span>               | <span data-ttu-id="31d04-115">字符串</span><span class="sxs-lookup"><span data-stu-id="31d04-115">String</span></span>                      | <span data-ttu-id="31d04-116">可取值为：`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="31d04-116">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="31d04-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31d04-117">createdDateTime</span></span>                | <span data-ttu-id="31d04-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31d04-118">DateTimeOffset</span></span>              | <span data-ttu-id="31d04-119">录制已创建的时间。</span><span class="sxs-lookup"><span data-stu-id="31d04-119">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="31d04-120">id</span><span class="sxs-lookup"><span data-stu-id="31d04-120">id</span></span>                             | <span data-ttu-id="31d04-121">字符串</span><span class="sxs-lookup"><span data-stu-id="31d04-121">String</span></span>                      | <span data-ttu-id="31d04-122">服务器操作 id。只读的。</span><span class="sxs-lookup"><span data-stu-id="31d04-122">The server operation id. Read-only.</span></span> <span data-ttu-id="31d04-123">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="31d04-123">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="31d04-124">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="31d04-124">lastActionDateTime</span></span>             | <span data-ttu-id="31d04-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31d04-125">DateTimeOffset</span></span>              | <span data-ttu-id="31d04-126">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="31d04-126">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="31d04-127">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="31d04-127">recordResourceAccessToken</span></span>      | <span data-ttu-id="31d04-128">字符串</span><span class="sxs-lookup"><span data-stu-id="31d04-128">String</span></span>                      | <span data-ttu-id="31d04-129">要检索录制，需要访问令牌。</span><span class="sxs-lookup"><span data-stu-id="31d04-129">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="31d04-130">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="31d04-130">recordResourceLocation</span></span>         | <span data-ttu-id="31d04-131">字符串</span><span class="sxs-lookup"><span data-stu-id="31d04-131">String</span></span>                      | <span data-ttu-id="31d04-132">录制所在位置。</span><span class="sxs-lookup"><span data-stu-id="31d04-132">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="31d04-133">resultInfo</span><span class="sxs-lookup"><span data-stu-id="31d04-133">resultInfo</span></span>                     | [<span data-ttu-id="31d04-134">resultInfo</span><span class="sxs-lookup"><span data-stu-id="31d04-134">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="31d04-135">结果的信息。</span><span class="sxs-lookup"><span data-stu-id="31d04-135">The result information.</span></span>  <span data-ttu-id="31d04-136">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="31d04-136">Read-only.</span></span> <span data-ttu-id="31d04-137">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="31d04-137">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="31d04-138">status</span><span class="sxs-lookup"><span data-stu-id="31d04-138">status</span></span>                         | <span data-ttu-id="31d04-139">String</span><span class="sxs-lookup"><span data-stu-id="31d04-139">String</span></span>                      | <span data-ttu-id="31d04-140">可取值为 `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="31d04-140">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="31d04-141">只读。</span><span class="sxs-lookup"><span data-stu-id="31d04-141">Read-only.</span></span> <span data-ttu-id="31d04-142">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="31d04-142">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="31d04-143">Relationships</span><span class="sxs-lookup"><span data-stu-id="31d04-143">Relationships</span></span>
<span data-ttu-id="31d04-144">无</span><span class="sxs-lookup"><span data-stu-id="31d04-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31d04-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31d04-145">JSON representation</span></span>

<span data-ttu-id="31d04-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31d04-146">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="31d04-147">示例</span><span class="sxs-lookup"><span data-stu-id="31d04-147">Example</span></span>

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
