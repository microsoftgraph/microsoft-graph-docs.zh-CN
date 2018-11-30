---
title: recordOperation 资源类型
description: RecordOperation 类型
ms.openlocfilehash: 5863e5ef84b00c65cd0806af8a3364fe3d1ab73f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042826"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="6ed17-103">recordOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ed17-103">recordOperation resource type</span></span>

> <span data-ttu-id="6ed17-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6ed17-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ed17-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6ed17-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ed17-106">RecordOperation 类型</span><span class="sxs-lookup"><span data-stu-id="6ed17-106">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="6ed17-107">属性</span><span class="sxs-lookup"><span data-stu-id="6ed17-107">Properties</span></span>

| <span data-ttu-id="6ed17-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ed17-108">Property</span></span>                       | <span data-ttu-id="6ed17-109">类型</span><span class="sxs-lookup"><span data-stu-id="6ed17-109">Type</span></span>                        | <span data-ttu-id="6ed17-110">说明</span><span class="sxs-lookup"><span data-stu-id="6ed17-110">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6ed17-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="6ed17-111">clientContext</span></span>                  | <span data-ttu-id="6ed17-112">字符串</span><span class="sxs-lookup"><span data-stu-id="6ed17-112">String</span></span>                      | <span data-ttu-id="6ed17-113">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="6ed17-113">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="6ed17-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="6ed17-114">completionReason</span></span>               | <span data-ttu-id="6ed17-115">字符串</span><span class="sxs-lookup"><span data-stu-id="6ed17-115">String</span></span>                      | <span data-ttu-id="6ed17-116">可取值为：`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`。</span><span class="sxs-lookup"><span data-stu-id="6ed17-116">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`.</span></span> |
| <span data-ttu-id="6ed17-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ed17-117">createdDateTime</span></span>                | <span data-ttu-id="6ed17-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ed17-118">DateTimeOffset</span></span>              | <span data-ttu-id="6ed17-119">录制已创建的时间。</span><span class="sxs-lookup"><span data-stu-id="6ed17-119">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="6ed17-120">id</span><span class="sxs-lookup"><span data-stu-id="6ed17-120">id</span></span>                             | <span data-ttu-id="6ed17-121">字符串</span><span class="sxs-lookup"><span data-stu-id="6ed17-121">String</span></span>                      | <span data-ttu-id="6ed17-122">服务器操作 id。只读的。</span><span class="sxs-lookup"><span data-stu-id="6ed17-122">The server operation id. Read-only.</span></span> <span data-ttu-id="6ed17-123">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="6ed17-123">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="6ed17-124">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="6ed17-124">lastActionDateTime</span></span>             | <span data-ttu-id="6ed17-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ed17-125">DateTimeOffset</span></span>              | <span data-ttu-id="6ed17-126">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="6ed17-126">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="6ed17-127">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="6ed17-127">recordResourceLocation</span></span>         | <span data-ttu-id="6ed17-128">字符串</span><span class="sxs-lookup"><span data-stu-id="6ed17-128">String</span></span>                      | <span data-ttu-id="6ed17-129">录制所在位置。</span><span class="sxs-lookup"><span data-stu-id="6ed17-129">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="6ed17-130">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="6ed17-130">recordResourceAccessToken</span></span>      | <span data-ttu-id="6ed17-131">字符串</span><span class="sxs-lookup"><span data-stu-id="6ed17-131">String</span></span>                      | <span data-ttu-id="6ed17-132">要检索录制，需要访问令牌。</span><span class="sxs-lookup"><span data-stu-id="6ed17-132">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="6ed17-133">resultInfo</span><span class="sxs-lookup"><span data-stu-id="6ed17-133">resultInfo</span></span>                     | [<span data-ttu-id="6ed17-134">resultInfo</span><span class="sxs-lookup"><span data-stu-id="6ed17-134">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="6ed17-135">结果的信息。</span><span class="sxs-lookup"><span data-stu-id="6ed17-135">The result information.</span></span>  <span data-ttu-id="6ed17-136">只读。</span><span class="sxs-lookup"><span data-stu-id="6ed17-136">Read-only.</span></span> <span data-ttu-id="6ed17-137">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="6ed17-137">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="6ed17-138">状态</span><span class="sxs-lookup"><span data-stu-id="6ed17-138">status</span></span>                         | <span data-ttu-id="6ed17-139">String</span><span class="sxs-lookup"><span data-stu-id="6ed17-139">String</span></span>                      | <span data-ttu-id="6ed17-140">可取值为 `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="6ed17-140">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="6ed17-141">只读。</span><span class="sxs-lookup"><span data-stu-id="6ed17-141">Read-only.</span></span> <span data-ttu-id="6ed17-142">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="6ed17-142">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="6ed17-143">Relationships</span><span class="sxs-lookup"><span data-stu-id="6ed17-143">Relationships</span></span>
<span data-ttu-id="6ed17-144">无</span><span class="sxs-lookup"><span data-stu-id="6ed17-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ed17-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ed17-145">JSON representation</span></span>

<span data-ttu-id="6ed17-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ed17-146">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceLocation": "String",
  "recordResourceAccessToken": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="6ed17-147">示例</span><span class="sxs-lookup"><span data-stu-id="6ed17-147">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.recordOperation",
  "truncated": true
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceLocation": "https://resource.location/ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceAccessToken": "<access-token>",
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
