---
title: recordOperation 资源类型
description: RecordOperation 类型
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6b9deb566e5b527a9f20db69441fa96908212a38
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512505"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="3e82c-103">recordOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e82c-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e82c-104">RecordOperation 类型</span><span class="sxs-lookup"><span data-stu-id="3e82c-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="3e82c-105">属性</span><span class="sxs-lookup"><span data-stu-id="3e82c-105">Properties</span></span>

| <span data-ttu-id="3e82c-106">属性</span><span class="sxs-lookup"><span data-stu-id="3e82c-106">Property</span></span>                       | <span data-ttu-id="3e82c-107">类型</span><span class="sxs-lookup"><span data-stu-id="3e82c-107">Type</span></span>                        | <span data-ttu-id="3e82c-108">说明</span><span class="sxs-lookup"><span data-stu-id="3e82c-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3e82c-109">ClientContext</span><span class="sxs-lookup"><span data-stu-id="3e82c-109">clientContext</span></span>                  | <span data-ttu-id="3e82c-110">String</span><span class="sxs-lookup"><span data-stu-id="3e82c-110">String</span></span>                      | <span data-ttu-id="3e82c-111">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="3e82c-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="3e82c-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="3e82c-112">completionReason</span></span>               | <span data-ttu-id="3e82c-113">String</span><span class="sxs-lookup"><span data-stu-id="3e82c-113">String</span></span>                      | <span data-ttu-id="3e82c-114">可取值为：`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="3e82c-114">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="3e82c-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e82c-115">createdDateTime</span></span>                | <span data-ttu-id="3e82c-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e82c-116">DateTimeOffset</span></span>              | <span data-ttu-id="3e82c-117">录制已创建的时间。</span><span class="sxs-lookup"><span data-stu-id="3e82c-117">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="3e82c-118">id</span><span class="sxs-lookup"><span data-stu-id="3e82c-118">id</span></span>                             | <span data-ttu-id="3e82c-119">字串符号</span><span class="sxs-lookup"><span data-stu-id="3e82c-119">String</span></span>                      | <span data-ttu-id="3e82c-120">服务器操作 id。只读的。</span><span class="sxs-lookup"><span data-stu-id="3e82c-120">The server operation id. Read-only.</span></span> <span data-ttu-id="3e82c-121">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="3e82c-121">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="3e82c-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="3e82c-122">lastActionDateTime</span></span>             | <span data-ttu-id="3e82c-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e82c-123">DateTimeOffset</span></span>              | <span data-ttu-id="3e82c-124">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="3e82c-124">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="3e82c-125">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="3e82c-125">recordResourceAccessToken</span></span>      | <span data-ttu-id="3e82c-126">String</span><span class="sxs-lookup"><span data-stu-id="3e82c-126">String</span></span>                      | <span data-ttu-id="3e82c-127">要检索录制，需要访问令牌。</span><span class="sxs-lookup"><span data-stu-id="3e82c-127">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="3e82c-128">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="3e82c-128">recordResourceLocation</span></span>         | <span data-ttu-id="3e82c-129">String</span><span class="sxs-lookup"><span data-stu-id="3e82c-129">String</span></span>                      | <span data-ttu-id="3e82c-130">录制所在位置。</span><span class="sxs-lookup"><span data-stu-id="3e82c-130">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="3e82c-131">resultInfo</span><span class="sxs-lookup"><span data-stu-id="3e82c-131">resultInfo</span></span>                     | [<span data-ttu-id="3e82c-132">resultInfo</span><span class="sxs-lookup"><span data-stu-id="3e82c-132">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="3e82c-133">结果的信息。</span><span class="sxs-lookup"><span data-stu-id="3e82c-133">The result information.</span></span>  <span data-ttu-id="3e82c-134">只读。</span><span class="sxs-lookup"><span data-stu-id="3e82c-134">Read-only.</span></span> <span data-ttu-id="3e82c-135">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="3e82c-135">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="3e82c-136">status</span><span class="sxs-lookup"><span data-stu-id="3e82c-136">status</span></span>                         | <span data-ttu-id="3e82c-137">String</span><span class="sxs-lookup"><span data-stu-id="3e82c-137">String</span></span>                      | <span data-ttu-id="3e82c-138">可取值为 `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="3e82c-138">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="3e82c-139">只读。</span><span class="sxs-lookup"><span data-stu-id="3e82c-139">Read-only.</span></span> <span data-ttu-id="3e82c-140">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="3e82c-140">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="3e82c-141">关系</span><span class="sxs-lookup"><span data-stu-id="3e82c-141">Relationships</span></span>
<span data-ttu-id="3e82c-142">无</span><span class="sxs-lookup"><span data-stu-id="3e82c-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e82c-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e82c-143">JSON representation</span></span>

<span data-ttu-id="3e82c-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e82c-144">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="3e82c-145">示例</span><span class="sxs-lookup"><span data-stu-id="3e82c-145">Example</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/recordoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
