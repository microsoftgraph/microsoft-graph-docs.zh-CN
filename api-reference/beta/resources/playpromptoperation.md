---
title: playPromptOperation 资源类型
description: 用于获取 playPrompt 操作的结果的 playPrompt 操作。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 89a47fc8400d2f0d426ef6f683eb566f9c2376d4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344360"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="6d8ef-103">playPromptOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d8ef-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d8ef-104">用于获取 playPrompt 操作的结果的 playPrompt 操作。</span><span class="sxs-lookup"><span data-stu-id="6d8ef-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="6d8ef-105">属性</span><span class="sxs-lookup"><span data-stu-id="6d8ef-105">Properties</span></span>

| <span data-ttu-id="6d8ef-106">属性</span><span class="sxs-lookup"><span data-stu-id="6d8ef-106">Property</span></span>            | <span data-ttu-id="6d8ef-107">类型</span><span class="sxs-lookup"><span data-stu-id="6d8ef-107">Type</span></span>                        | <span data-ttu-id="6d8ef-108">说明</span><span class="sxs-lookup"><span data-stu-id="6d8ef-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="6d8ef-109">适用</span><span class="sxs-lookup"><span data-stu-id="6d8ef-109">clientContext</span></span>       | <span data-ttu-id="6d8ef-110">String</span><span class="sxs-lookup"><span data-stu-id="6d8ef-110">String</span></span>                      | <span data-ttu-id="6d8ef-111">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="6d8ef-111">The client context.</span></span>                                                                |
| <span data-ttu-id="6d8ef-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="6d8ef-112">completionReason</span></span>    | <span data-ttu-id="6d8ef-113">String</span><span class="sxs-lookup"><span data-stu-id="6d8ef-113">String</span></span>                      | <span data-ttu-id="6d8ef-114">可取值为：`unknown`、`completedSuccessfully`、`mediaOperationCanceled`。</span><span class="sxs-lookup"><span data-stu-id="6d8ef-114">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="6d8ef-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d8ef-115">createdDateTime</span></span>     | <span data-ttu-id="6d8ef-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d8ef-116">DateTimeOffset</span></span>              | <span data-ttu-id="6d8ef-117">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="6d8ef-117">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="6d8ef-118">id</span><span class="sxs-lookup"><span data-stu-id="6d8ef-118">id</span></span>                  | <span data-ttu-id="6d8ef-119">String</span><span class="sxs-lookup"><span data-stu-id="6d8ef-119">String</span></span>                      | <span data-ttu-id="6d8ef-120">只读。</span><span class="sxs-lookup"><span data-stu-id="6d8ef-120">Read-only.</span></span>                                                                         |
| <span data-ttu-id="6d8ef-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="6d8ef-121">lastActionDateTime</span></span>  | <span data-ttu-id="6d8ef-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d8ef-122">DateTimeOffset</span></span>              | <span data-ttu-id="6d8ef-123">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="6d8ef-123">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="6d8ef-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="6d8ef-124">resultInfo</span></span>          | [<span data-ttu-id="6d8ef-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="6d8ef-125">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="6d8ef-126">结果信息。</span><span class="sxs-lookup"><span data-stu-id="6d8ef-126">The result information.</span></span> <span data-ttu-id="6d8ef-127">只读。</span><span class="sxs-lookup"><span data-stu-id="6d8ef-127">Read-only.</span></span> <span data-ttu-id="6d8ef-128">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="6d8ef-128">Server generated.</span></span>                               |
| <span data-ttu-id="6d8ef-129">status</span><span class="sxs-lookup"><span data-stu-id="6d8ef-129">status</span></span>              | <span data-ttu-id="6d8ef-130">String</span><span class="sxs-lookup"><span data-stu-id="6d8ef-130">String</span></span>                      | <span data-ttu-id="6d8ef-131">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="6d8ef-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="6d8ef-132">关系</span><span class="sxs-lookup"><span data-stu-id="6d8ef-132">Relationships</span></span>
<span data-ttu-id="6d8ef-133">无</span><span class="sxs-lookup"><span data-stu-id="6d8ef-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d8ef-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d8ef-134">JSON representation</span></span>

<span data-ttu-id="6d8ef-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d8ef-135">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
