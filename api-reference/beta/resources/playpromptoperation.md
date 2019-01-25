---
title: playPromptOperation 资源类型
description: 要获取 playPrompt 操作的结果的 playPrompt 操作。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6ecdb06c910923d35f9d36590ad09fd7835fccb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515200"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="548e3-103">playPromptOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="548e3-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="548e3-104">要获取 playPrompt 操作的结果的 playPrompt 操作。</span><span class="sxs-lookup"><span data-stu-id="548e3-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="548e3-105">属性</span><span class="sxs-lookup"><span data-stu-id="548e3-105">Properties</span></span>

| <span data-ttu-id="548e3-106">属性</span><span class="sxs-lookup"><span data-stu-id="548e3-106">Property</span></span>            | <span data-ttu-id="548e3-107">类型</span><span class="sxs-lookup"><span data-stu-id="548e3-107">Type</span></span>                        | <span data-ttu-id="548e3-108">说明</span><span class="sxs-lookup"><span data-stu-id="548e3-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="548e3-109">ClientContext</span><span class="sxs-lookup"><span data-stu-id="548e3-109">clientContext</span></span>       | <span data-ttu-id="548e3-110">String</span><span class="sxs-lookup"><span data-stu-id="548e3-110">String</span></span>                      | <span data-ttu-id="548e3-111">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="548e3-111">The client context.</span></span>                                                                |
| <span data-ttu-id="548e3-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="548e3-112">completionReason</span></span>    | <span data-ttu-id="548e3-113">String</span><span class="sxs-lookup"><span data-stu-id="548e3-113">String</span></span>                      | <span data-ttu-id="548e3-114">可取值为：`unknown`、`completedSuccessfully`、`mediaOperationCanceled`。</span><span class="sxs-lookup"><span data-stu-id="548e3-114">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="548e3-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="548e3-115">createdDateTime</span></span>     | <span data-ttu-id="548e3-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="548e3-116">DateTimeOffset</span></span>              | <span data-ttu-id="548e3-117">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="548e3-117">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="548e3-118">id</span><span class="sxs-lookup"><span data-stu-id="548e3-118">id</span></span>                  | <span data-ttu-id="548e3-119">String</span><span class="sxs-lookup"><span data-stu-id="548e3-119">String</span></span>                      | <span data-ttu-id="548e3-120">只读。</span><span class="sxs-lookup"><span data-stu-id="548e3-120">Read-only.</span></span>                                                                         |
| <span data-ttu-id="548e3-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="548e3-121">lastActionDateTime</span></span>  | <span data-ttu-id="548e3-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="548e3-122">DateTimeOffset</span></span>              | <span data-ttu-id="548e3-123">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="548e3-123">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="548e3-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="548e3-124">resultInfo</span></span>          | [<span data-ttu-id="548e3-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="548e3-125">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="548e3-126">结果的信息。</span><span class="sxs-lookup"><span data-stu-id="548e3-126">The result information.</span></span> <span data-ttu-id="548e3-127">只读。</span><span class="sxs-lookup"><span data-stu-id="548e3-127">Read-only.</span></span> <span data-ttu-id="548e3-128">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="548e3-128">Server generated.</span></span>                               |
| <span data-ttu-id="548e3-129">status</span><span class="sxs-lookup"><span data-stu-id="548e3-129">status</span></span>              | <span data-ttu-id="548e3-130">String</span><span class="sxs-lookup"><span data-stu-id="548e3-130">String</span></span>                      | <span data-ttu-id="548e3-131">可取值为：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="548e3-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="548e3-132">Relationships</span><span class="sxs-lookup"><span data-stu-id="548e3-132">Relationships</span></span>
<span data-ttu-id="548e3-133">无</span><span class="sxs-lookup"><span data-stu-id="548e3-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="548e3-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="548e3-134">JSON representation</span></span>

<span data-ttu-id="548e3-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="548e3-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "unknown | completedSuccessfully | mediaOperationCanceled",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/playpromptoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
