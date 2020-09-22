---
title: playPromptOperation 资源类型
description: 用于获取 playPrompt 操作的结果的 playPrompt 操作。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a1f5c72ed315714039d964c99437af28425bb064
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033648"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="fdd58-103">playPromptOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="fdd58-103">playPromptOperation resource type</span></span>

<span data-ttu-id="fdd58-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdd58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdd58-105">用于获取 playPrompt 操作的结果的 playPrompt 操作。</span><span class="sxs-lookup"><span data-stu-id="fdd58-105">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="fdd58-106">属性</span><span class="sxs-lookup"><span data-stu-id="fdd58-106">Properties</span></span>

| <span data-ttu-id="fdd58-107">属性</span><span class="sxs-lookup"><span data-stu-id="fdd58-107">Property</span></span>            | <span data-ttu-id="fdd58-108">类型</span><span class="sxs-lookup"><span data-stu-id="fdd58-108">Type</span></span>                        | <span data-ttu-id="fdd58-109">说明</span><span class="sxs-lookup"><span data-stu-id="fdd58-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="fdd58-110">适用</span><span class="sxs-lookup"><span data-stu-id="fdd58-110">clientContext</span></span>       | <span data-ttu-id="fdd58-111">String</span><span class="sxs-lookup"><span data-stu-id="fdd58-111">String</span></span>                      | <span data-ttu-id="fdd58-112">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="fdd58-112">Unique Client Context string.</span></span> <span data-ttu-id="fdd58-113">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="fdd58-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="fdd58-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="fdd58-114">completionReason</span></span>    | <span data-ttu-id="fdd58-115">String</span><span class="sxs-lookup"><span data-stu-id="fdd58-115">String</span></span>                      | <span data-ttu-id="fdd58-116">可取值为：`unknown`、`completedSuccessfully`、`mediaOperationCanceled`。</span><span class="sxs-lookup"><span data-stu-id="fdd58-116">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="fdd58-117">id</span><span class="sxs-lookup"><span data-stu-id="fdd58-117">id</span></span>                  | <span data-ttu-id="fdd58-118">String</span><span class="sxs-lookup"><span data-stu-id="fdd58-118">String</span></span>                      | <span data-ttu-id="fdd58-119">只读。</span><span class="sxs-lookup"><span data-stu-id="fdd58-119">Read-only.</span></span>                                                                         |
| <span data-ttu-id="fdd58-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="fdd58-120">resultInfo</span></span>          | [<span data-ttu-id="fdd58-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="fdd58-121">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="fdd58-122">结果信息。</span><span class="sxs-lookup"><span data-stu-id="fdd58-122">The result information.</span></span> <span data-ttu-id="fdd58-123">只读。</span><span class="sxs-lookup"><span data-stu-id="fdd58-123">Read-only.</span></span>                                |
| <span data-ttu-id="fdd58-124">状态</span><span class="sxs-lookup"><span data-stu-id="fdd58-124">status</span></span>              | <span data-ttu-id="fdd58-125">String</span><span class="sxs-lookup"><span data-stu-id="fdd58-125">String</span></span>                      | <span data-ttu-id="fdd58-126">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="fdd58-126">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="fdd58-127">关系</span><span class="sxs-lookup"><span data-stu-id="fdd58-127">Relationships</span></span>
<span data-ttu-id="fdd58-128">无</span><span class="sxs-lookup"><span data-stu-id="fdd58-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdd58-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fdd58-129">JSON representation</span></span>

<span data-ttu-id="fdd58-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdd58-130">The following is a JSON representation of the resource.</span></span>

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


