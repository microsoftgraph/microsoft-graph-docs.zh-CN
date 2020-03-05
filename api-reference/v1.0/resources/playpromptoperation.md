---
title: playPromptOperation 资源类型
description: 用于获取 playPrompt 操作的结果的 playPrompt 操作。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5adc385c5764371c1e2cab516bc33fd8504aecf5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447085"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="7674d-103">playPromptOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="7674d-103">playPromptOperation resource type</span></span>

<span data-ttu-id="7674d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7674d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7674d-105">用于获取 playPrompt 操作的结果的 playPrompt 操作。</span><span class="sxs-lookup"><span data-stu-id="7674d-105">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="7674d-106">属性</span><span class="sxs-lookup"><span data-stu-id="7674d-106">Properties</span></span>

| <span data-ttu-id="7674d-107">属性</span><span class="sxs-lookup"><span data-stu-id="7674d-107">Property</span></span>            | <span data-ttu-id="7674d-108">类型</span><span class="sxs-lookup"><span data-stu-id="7674d-108">Type</span></span>                        | <span data-ttu-id="7674d-109">说明</span><span class="sxs-lookup"><span data-stu-id="7674d-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="7674d-110">适用</span><span class="sxs-lookup"><span data-stu-id="7674d-110">clientContext</span></span>       | <span data-ttu-id="7674d-111">String</span><span class="sxs-lookup"><span data-stu-id="7674d-111">String</span></span>                      | <span data-ttu-id="7674d-112">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="7674d-112">Unique Client Context string.</span></span> <span data-ttu-id="7674d-113">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="7674d-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="7674d-114">id</span><span class="sxs-lookup"><span data-stu-id="7674d-114">id</span></span>                  | <span data-ttu-id="7674d-115">字符串</span><span class="sxs-lookup"><span data-stu-id="7674d-115">String</span></span>                      | <span data-ttu-id="7674d-116">只读。</span><span class="sxs-lookup"><span data-stu-id="7674d-116">Read-only.</span></span>                                                                         |
| <span data-ttu-id="7674d-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="7674d-117">resultInfo</span></span>          | [<span data-ttu-id="7674d-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="7674d-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="7674d-119">结果信息。</span><span class="sxs-lookup"><span data-stu-id="7674d-119">The result information.</span></span> <span data-ttu-id="7674d-120">只读。</span><span class="sxs-lookup"><span data-stu-id="7674d-120">Read-only.</span></span>                                |
| <span data-ttu-id="7674d-121">status</span><span class="sxs-lookup"><span data-stu-id="7674d-121">status</span></span>              | <span data-ttu-id="7674d-122">String</span><span class="sxs-lookup"><span data-stu-id="7674d-122">String</span></span>                      | <span data-ttu-id="7674d-123">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="7674d-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="7674d-124">关系</span><span class="sxs-lookup"><span data-stu-id="7674d-124">Relationships</span></span>
<span data-ttu-id="7674d-125">无</span><span class="sxs-lookup"><span data-stu-id="7674d-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7674d-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7674d-126">JSON representation</span></span>

<span data-ttu-id="7674d-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7674d-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
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
