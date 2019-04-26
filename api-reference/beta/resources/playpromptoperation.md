---
title: playPromptOperation 资源类型
description: 用于获取 playPrompt 操作的结果的 playPrompt 操作。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6ecdb06c910923d35f9d36590ad09fd7835fccb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563664"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="7c0f0-103">playPromptOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c0f0-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c0f0-104">用于获取 playPrompt 操作的结果的 playPrompt 操作。</span><span class="sxs-lookup"><span data-stu-id="7c0f0-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="7c0f0-105">属性</span><span class="sxs-lookup"><span data-stu-id="7c0f0-105">Properties</span></span>

| <span data-ttu-id="7c0f0-106">属性</span><span class="sxs-lookup"><span data-stu-id="7c0f0-106">Property</span></span>            | <span data-ttu-id="7c0f0-107">类型</span><span class="sxs-lookup"><span data-stu-id="7c0f0-107">Type</span></span>                        | <span data-ttu-id="7c0f0-108">说明</span><span class="sxs-lookup"><span data-stu-id="7c0f0-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="7c0f0-109">适用</span><span class="sxs-lookup"><span data-stu-id="7c0f0-109">clientContext</span></span>       | <span data-ttu-id="7c0f0-110">String</span><span class="sxs-lookup"><span data-stu-id="7c0f0-110">String</span></span>                      | <span data-ttu-id="7c0f0-111">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="7c0f0-111">The client context.</span></span>                                                                |
| <span data-ttu-id="7c0f0-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="7c0f0-112">completionReason</span></span>    | <span data-ttu-id="7c0f0-113">String</span><span class="sxs-lookup"><span data-stu-id="7c0f0-113">String</span></span>                      | <span data-ttu-id="7c0f0-114">可取值为：`unknown`、`completedSuccessfully`、`mediaOperationCanceled`。</span><span class="sxs-lookup"><span data-stu-id="7c0f0-114">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="7c0f0-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c0f0-115">createdDateTime</span></span>     | <span data-ttu-id="7c0f0-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c0f0-116">DateTimeOffset</span></span>              | <span data-ttu-id="7c0f0-117">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="7c0f0-117">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="7c0f0-118">id</span><span class="sxs-lookup"><span data-stu-id="7c0f0-118">id</span></span>                  | <span data-ttu-id="7c0f0-119">String</span><span class="sxs-lookup"><span data-stu-id="7c0f0-119">String</span></span>                      | <span data-ttu-id="7c0f0-120">只读。</span><span class="sxs-lookup"><span data-stu-id="7c0f0-120">Read-only.</span></span>                                                                         |
| <span data-ttu-id="7c0f0-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="7c0f0-121">lastActionDateTime</span></span>  | <span data-ttu-id="7c0f0-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c0f0-122">DateTimeOffset</span></span>              | <span data-ttu-id="7c0f0-123">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="7c0f0-123">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="7c0f0-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="7c0f0-124">resultInfo</span></span>          | [<span data-ttu-id="7c0f0-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="7c0f0-125">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="7c0f0-126">结果信息。</span><span class="sxs-lookup"><span data-stu-id="7c0f0-126">The result information.</span></span> <span data-ttu-id="7c0f0-127">只读。</span><span class="sxs-lookup"><span data-stu-id="7c0f0-127">Read-only.</span></span> <span data-ttu-id="7c0f0-128">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="7c0f0-128">Server generated.</span></span>                               |
| <span data-ttu-id="7c0f0-129">状态</span><span class="sxs-lookup"><span data-stu-id="7c0f0-129">status</span></span>              | <span data-ttu-id="7c0f0-130">String</span><span class="sxs-lookup"><span data-stu-id="7c0f0-130">String</span></span>                      | <span data-ttu-id="7c0f0-131">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="7c0f0-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="7c0f0-132">关系</span><span class="sxs-lookup"><span data-stu-id="7c0f0-132">Relationships</span></span>
<span data-ttu-id="7c0f0-133">无</span><span class="sxs-lookup"><span data-stu-id="7c0f0-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c0f0-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c0f0-134">JSON representation</span></span>

<span data-ttu-id="7c0f0-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c0f0-135">The following is a JSON representation of the resource.</span></span>

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
