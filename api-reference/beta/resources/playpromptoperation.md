---
title: playPromptOperation 资源类型
description: 要获取 playPrompt 操作的结果的 playPrompt 操作。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d451418482d1adf1a4b7e16dc8a6eb8ca7febdb7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937815"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="d29b2-103">playPromptOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="d29b2-103">playPromptOperation resource type</span></span>

> <span data-ttu-id="d29b2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d29b2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d29b2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d29b2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d29b2-106">要获取 playPrompt 操作的结果的 playPrompt 操作。</span><span class="sxs-lookup"><span data-stu-id="d29b2-106">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="d29b2-107">属性</span><span class="sxs-lookup"><span data-stu-id="d29b2-107">Properties</span></span>

| <span data-ttu-id="d29b2-108">属性</span><span class="sxs-lookup"><span data-stu-id="d29b2-108">Property</span></span>            | <span data-ttu-id="d29b2-109">类型</span><span class="sxs-lookup"><span data-stu-id="d29b2-109">Type</span></span>                        | <span data-ttu-id="d29b2-110">Description</span><span class="sxs-lookup"><span data-stu-id="d29b2-110">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="d29b2-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="d29b2-111">clientContext</span></span>       | <span data-ttu-id="d29b2-112">字符串</span><span class="sxs-lookup"><span data-stu-id="d29b2-112">String</span></span>                      | <span data-ttu-id="d29b2-113">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="d29b2-113">The client context.</span></span>                                                                |
| <span data-ttu-id="d29b2-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="d29b2-114">completionReason</span></span>    | <span data-ttu-id="d29b2-115">字符串</span><span class="sxs-lookup"><span data-stu-id="d29b2-115">String</span></span>                      | <span data-ttu-id="d29b2-116">可取值为：`unknown`、`completedSuccessfully`、`mediaOperationCanceled`。</span><span class="sxs-lookup"><span data-stu-id="d29b2-116">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="d29b2-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d29b2-117">createdDateTime</span></span>     | <span data-ttu-id="d29b2-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d29b2-118">DateTimeOffset</span></span>              | <span data-ttu-id="d29b2-119">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="d29b2-119">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="d29b2-120">id</span><span class="sxs-lookup"><span data-stu-id="d29b2-120">id</span></span>                  | <span data-ttu-id="d29b2-121">String</span><span class="sxs-lookup"><span data-stu-id="d29b2-121">String</span></span>                      | <span data-ttu-id="d29b2-122">只读。</span><span class="sxs-lookup"><span data-stu-id="d29b2-122">Read-only.</span></span>                                                                         |
| <span data-ttu-id="d29b2-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="d29b2-123">lastActionDateTime</span></span>  | <span data-ttu-id="d29b2-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d29b2-124">DateTimeOffset</span></span>              | <span data-ttu-id="d29b2-125">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="d29b2-125">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="d29b2-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d29b2-126">resultInfo</span></span>          | [<span data-ttu-id="d29b2-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d29b2-127">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="d29b2-128">结果的信息。</span><span class="sxs-lookup"><span data-stu-id="d29b2-128">The result information.</span></span> <span data-ttu-id="d29b2-129">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="d29b2-129">Read-only.</span></span> <span data-ttu-id="d29b2-130">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="d29b2-130">Server generated.</span></span>                               |
| <span data-ttu-id="d29b2-131">status</span><span class="sxs-lookup"><span data-stu-id="d29b2-131">status</span></span>              | <span data-ttu-id="d29b2-132">String</span><span class="sxs-lookup"><span data-stu-id="d29b2-132">String</span></span>                      | <span data-ttu-id="d29b2-133">可取值为：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="d29b2-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="d29b2-134">Relationships</span><span class="sxs-lookup"><span data-stu-id="d29b2-134">Relationships</span></span>
<span data-ttu-id="d29b2-135">无</span><span class="sxs-lookup"><span data-stu-id="d29b2-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d29b2-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d29b2-136">JSON representation</span></span>

<span data-ttu-id="d29b2-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d29b2-137">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
