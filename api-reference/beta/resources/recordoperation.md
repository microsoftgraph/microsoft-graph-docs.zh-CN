---
title: recordOperation 资源类型
description: RecordOperation 类型
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 914b8d819fdbcc132d4e04cd12f5c0db9980f659
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577184"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="c4e3b-103">recordOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4e3b-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4e3b-104">RecordOperation 类型</span><span class="sxs-lookup"><span data-stu-id="c4e3b-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="c4e3b-105">属性</span><span class="sxs-lookup"><span data-stu-id="c4e3b-105">Properties</span></span>

| <span data-ttu-id="c4e3b-106">属性</span><span class="sxs-lookup"><span data-stu-id="c4e3b-106">Property</span></span>                       | <span data-ttu-id="c4e3b-107">类型</span><span class="sxs-lookup"><span data-stu-id="c4e3b-107">Type</span></span>                        | <span data-ttu-id="c4e3b-108">说明</span><span class="sxs-lookup"><span data-stu-id="c4e3b-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c4e3b-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="c4e3b-109">clientContext</span></span>                  | <span data-ttu-id="c4e3b-110">String</span><span class="sxs-lookup"><span data-stu-id="c4e3b-110">String</span></span>                      | <span data-ttu-id="c4e3b-111">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="c4e3b-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="c4e3b-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="c4e3b-112">completionReason</span></span>               | <span data-ttu-id="c4e3b-113">String</span><span class="sxs-lookup"><span data-stu-id="c4e3b-113">String</span></span>                      | <span data-ttu-id="c4e3b-114">可取值为：`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="c4e3b-114">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="c4e3b-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4e3b-115">createdDateTime</span></span>                | <span data-ttu-id="c4e3b-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4e3b-116">DateTimeOffset</span></span>              | <span data-ttu-id="c4e3b-117">录制已创建的时间。</span><span class="sxs-lookup"><span data-stu-id="c4e3b-117">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="c4e3b-118">id</span><span class="sxs-lookup"><span data-stu-id="c4e3b-118">id</span></span>                             | <span data-ttu-id="c4e3b-119">String</span><span class="sxs-lookup"><span data-stu-id="c4e3b-119">String</span></span>                      | <span data-ttu-id="c4e3b-120">服务器操作 id。只读的。</span><span class="sxs-lookup"><span data-stu-id="c4e3b-120">The server operation id. Read-only.</span></span> <span data-ttu-id="c4e3b-121">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="c4e3b-121">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="c4e3b-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="c4e3b-122">lastActionDateTime</span></span>             | <span data-ttu-id="c4e3b-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4e3b-123">DateTimeOffset</span></span>              | <span data-ttu-id="c4e3b-124">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="c4e3b-124">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="c4e3b-125">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="c4e3b-125">recordResourceAccessToken</span></span>      | <span data-ttu-id="c4e3b-126">String</span><span class="sxs-lookup"><span data-stu-id="c4e3b-126">String</span></span>                      | <span data-ttu-id="c4e3b-127">要检索录制，需要访问令牌。</span><span class="sxs-lookup"><span data-stu-id="c4e3b-127">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="c4e3b-128">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="c4e3b-128">recordResourceLocation</span></span>         | <span data-ttu-id="c4e3b-129">String</span><span class="sxs-lookup"><span data-stu-id="c4e3b-129">String</span></span>                      | <span data-ttu-id="c4e3b-130">录制所在位置。</span><span class="sxs-lookup"><span data-stu-id="c4e3b-130">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="c4e3b-131">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c4e3b-131">resultInfo</span></span>                     | [<span data-ttu-id="c4e3b-132">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c4e3b-132">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="c4e3b-133">结果信息。</span><span class="sxs-lookup"><span data-stu-id="c4e3b-133">The result information.</span></span>  <span data-ttu-id="c4e3b-134">只读。</span><span class="sxs-lookup"><span data-stu-id="c4e3b-134">Read-only.</span></span> <span data-ttu-id="c4e3b-135">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="c4e3b-135">Server generated.</span></span>                                                                                             |

## <a name="relationships"></a><span data-ttu-id="c4e3b-136">关系</span><span class="sxs-lookup"><span data-stu-id="c4e3b-136">Relationships</span></span>
<span data-ttu-id="c4e3b-137">无</span><span class="sxs-lookup"><span data-stu-id="c4e3b-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4e3b-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4e3b-138">JSON representation</span></span>

<span data-ttu-id="c4e3b-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4e3b-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "recordCompletionReason",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceAccessToken": "String",
  "recordResourceLocation": "String",
  "resultInfo": {"@odata.type": "microsoft.graph.resultInfo"}
}
```

## <a name="example"></a><span data-ttu-id="c4e3b-140">示例</span><span class="sxs-lookup"><span data-stu-id="c4e3b-140">Example</span></span>

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
