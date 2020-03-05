---
title: MuteParticipantOperation 资源类型
description: 描述呼叫参与者静音操作的响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: eb85ea8e1759dc948f764b391e25a51b97090566
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447372"
---
# <a name="muteparticipantoperation-resource-type"></a><span data-ttu-id="fd273-103">MuteParticipantOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd273-103">MuteParticipantOperation resource type</span></span>

<span data-ttu-id="fd273-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="fd273-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fd273-105">描述呼叫参与者静音操作的响应格式。</span><span class="sxs-lookup"><span data-stu-id="fd273-105">Describes the response format of a call participant mute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="fd273-106">属性</span><span class="sxs-lookup"><span data-stu-id="fd273-106">Properties</span></span>

| <span data-ttu-id="fd273-107">属性</span><span class="sxs-lookup"><span data-stu-id="fd273-107">Property</span></span>                       | <span data-ttu-id="fd273-108">类型</span><span class="sxs-lookup"><span data-stu-id="fd273-108">Type</span></span>                        | <span data-ttu-id="fd273-109">说明</span><span class="sxs-lookup"><span data-stu-id="fd273-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fd273-110">适用</span><span class="sxs-lookup"><span data-stu-id="fd273-110">clientContext</span></span>                  | <span data-ttu-id="fd273-111">String</span><span class="sxs-lookup"><span data-stu-id="fd273-111">String</span></span>                      | <span data-ttu-id="fd273-112">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="fd273-112">Unique client context string.</span></span> <span data-ttu-id="fd273-113">最多可以有256个字符。</span><span class="sxs-lookup"><span data-stu-id="fd273-113">Can have a maximum of 256 characters.</span></span>                                                                               |
| <span data-ttu-id="fd273-114">id</span><span class="sxs-lookup"><span data-stu-id="fd273-114">id</span></span>                             | <span data-ttu-id="fd273-115">String</span><span class="sxs-lookup"><span data-stu-id="fd273-115">String</span></span>                      | <span data-ttu-id="fd273-116">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="fd273-116">The server operation ID.</span></span> <span data-ttu-id="fd273-117">只读。</span><span class="sxs-lookup"><span data-stu-id="fd273-117">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="fd273-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="fd273-118">resultInfo</span></span>                     | [<span data-ttu-id="fd273-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="fd273-119">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="fd273-120">结果信息。</span><span class="sxs-lookup"><span data-stu-id="fd273-120">The result information.</span></span>  <span data-ttu-id="fd273-121">只读。</span><span class="sxs-lookup"><span data-stu-id="fd273-121">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="fd273-122">status</span><span class="sxs-lookup"><span data-stu-id="fd273-122">status</span></span>                         | <span data-ttu-id="fd273-123">String</span><span class="sxs-lookup"><span data-stu-id="fd273-123">String</span></span>                      | <span data-ttu-id="fd273-124">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="fd273-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="fd273-125">只读。</span><span class="sxs-lookup"><span data-stu-id="fd273-125">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="fd273-126">关系</span><span class="sxs-lookup"><span data-stu-id="fd273-126">Relationships</span></span>
<span data-ttu-id="fd273-127">无。</span><span class="sxs-lookup"><span data-stu-id="fd273-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd273-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd273-128">JSON representation</span></span>

<span data-ttu-id="fd273-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd273-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.muteParticipantOperation"
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
<!-- {
  "type": "#page.annotation",
  "description": "muteParticipantOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
