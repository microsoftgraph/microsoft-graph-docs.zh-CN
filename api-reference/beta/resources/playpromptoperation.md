---
title: playPromptOperation 资源类型
description: 用于获取 playPrompt 操作的结果的 playPrompt 操作。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 84b54fbce830f5b505decee7e2d25618700728b3
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006576"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="23431-103">playPromptOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="23431-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23431-104">用于获取 playPrompt 操作的结果的 playPrompt 操作。</span><span class="sxs-lookup"><span data-stu-id="23431-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="23431-105">属性</span><span class="sxs-lookup"><span data-stu-id="23431-105">Properties</span></span>

| <span data-ttu-id="23431-106">属性</span><span class="sxs-lookup"><span data-stu-id="23431-106">Property</span></span>            | <span data-ttu-id="23431-107">类型</span><span class="sxs-lookup"><span data-stu-id="23431-107">Type</span></span>                        | <span data-ttu-id="23431-108">说明</span><span class="sxs-lookup"><span data-stu-id="23431-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="23431-109">适用</span><span class="sxs-lookup"><span data-stu-id="23431-109">clientContext</span></span>       | <span data-ttu-id="23431-110">String</span><span class="sxs-lookup"><span data-stu-id="23431-110">String</span></span>                      | <span data-ttu-id="23431-111">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="23431-111">Unique Client Context string.</span></span> <span data-ttu-id="23431-112">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="23431-112">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="23431-113">completionReason</span><span class="sxs-lookup"><span data-stu-id="23431-113">completionReason</span></span>    | <span data-ttu-id="23431-114">String</span><span class="sxs-lookup"><span data-stu-id="23431-114">String</span></span>                      | <span data-ttu-id="23431-115">可取值为：`unknown`、`completedSuccessfully`、`mediaOperationCanceled`。</span><span class="sxs-lookup"><span data-stu-id="23431-115">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="23431-116">id</span><span class="sxs-lookup"><span data-stu-id="23431-116">id</span></span>                  | <span data-ttu-id="23431-117">字符串</span><span class="sxs-lookup"><span data-stu-id="23431-117">String</span></span>                      | <span data-ttu-id="23431-118">只读。</span><span class="sxs-lookup"><span data-stu-id="23431-118">Read-only.</span></span>                                                                         |
| <span data-ttu-id="23431-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="23431-119">resultInfo</span></span>          | [<span data-ttu-id="23431-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="23431-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="23431-121">结果信息。</span><span class="sxs-lookup"><span data-stu-id="23431-121">The result information.</span></span> <span data-ttu-id="23431-122">只读。</span><span class="sxs-lookup"><span data-stu-id="23431-122">Read-only.</span></span>                                |
| <span data-ttu-id="23431-123">状态</span><span class="sxs-lookup"><span data-stu-id="23431-123">status</span></span>              | <span data-ttu-id="23431-124">String</span><span class="sxs-lookup"><span data-stu-id="23431-124">String</span></span>                      | <span data-ttu-id="23431-125">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="23431-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="23431-126">关系</span><span class="sxs-lookup"><span data-stu-id="23431-126">Relationships</span></span>
<span data-ttu-id="23431-127">无</span><span class="sxs-lookup"><span data-stu-id="23431-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23431-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23431-128">JSON representation</span></span>

<span data-ttu-id="23431-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23431-129">The following is a JSON representation of the resource.</span></span>

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
  "id": "String (identifier)",
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
