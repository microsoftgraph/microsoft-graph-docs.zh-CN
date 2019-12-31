---
title: playPromptOperation 资源类型
description: 用于获取 playPrompt 操作的结果的 playPrompt 操作。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3aff109b152be328e6923f6fdb36f116e63a9c16
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913308"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="40e18-103">playPromptOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="40e18-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40e18-104">用于获取 playPrompt 操作的结果的 playPrompt 操作。</span><span class="sxs-lookup"><span data-stu-id="40e18-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="40e18-105">属性</span><span class="sxs-lookup"><span data-stu-id="40e18-105">Properties</span></span>

| <span data-ttu-id="40e18-106">属性</span><span class="sxs-lookup"><span data-stu-id="40e18-106">Property</span></span>            | <span data-ttu-id="40e18-107">类型</span><span class="sxs-lookup"><span data-stu-id="40e18-107">Type</span></span>                        | <span data-ttu-id="40e18-108">说明</span><span class="sxs-lookup"><span data-stu-id="40e18-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="40e18-109">适用</span><span class="sxs-lookup"><span data-stu-id="40e18-109">clientContext</span></span>       | <span data-ttu-id="40e18-110">String</span><span class="sxs-lookup"><span data-stu-id="40e18-110">String</span></span>                      | <span data-ttu-id="40e18-111">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="40e18-111">Unique Client Context string.</span></span> <span data-ttu-id="40e18-112">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="40e18-112">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="40e18-113">completionReason</span><span class="sxs-lookup"><span data-stu-id="40e18-113">completionReason</span></span>    | <span data-ttu-id="40e18-114">String</span><span class="sxs-lookup"><span data-stu-id="40e18-114">String</span></span>                      | <span data-ttu-id="40e18-115">可取值为：`unknown`、`completedSuccessfully`、`mediaOperationCanceled`。</span><span class="sxs-lookup"><span data-stu-id="40e18-115">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="40e18-116">id</span><span class="sxs-lookup"><span data-stu-id="40e18-116">id</span></span>                  | <span data-ttu-id="40e18-117">字符串</span><span class="sxs-lookup"><span data-stu-id="40e18-117">String</span></span>                      | <span data-ttu-id="40e18-118">只读。</span><span class="sxs-lookup"><span data-stu-id="40e18-118">Read-only.</span></span>                                                                         |
| <span data-ttu-id="40e18-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="40e18-119">resultInfo</span></span>          | [<span data-ttu-id="40e18-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="40e18-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="40e18-121">结果信息。</span><span class="sxs-lookup"><span data-stu-id="40e18-121">The result information.</span></span> <span data-ttu-id="40e18-122">只读。</span><span class="sxs-lookup"><span data-stu-id="40e18-122">Read-only.</span></span>                                |
| <span data-ttu-id="40e18-123">状态</span><span class="sxs-lookup"><span data-stu-id="40e18-123">status</span></span>              | <span data-ttu-id="40e18-124">String</span><span class="sxs-lookup"><span data-stu-id="40e18-124">String</span></span>                      | <span data-ttu-id="40e18-125">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="40e18-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="40e18-126">关系</span><span class="sxs-lookup"><span data-stu-id="40e18-126">Relationships</span></span>
<span data-ttu-id="40e18-127">无</span><span class="sxs-lookup"><span data-stu-id="40e18-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40e18-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40e18-128">JSON representation</span></span>

<span data-ttu-id="40e18-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40e18-129">The following is a JSON representation of the resource.</span></span>

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
