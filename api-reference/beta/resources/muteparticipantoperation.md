---
title: MuteParticipantOperation 资源类型
description: 描述呼叫参与者静音操作的响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2b7eb9821f21af7a037723815a9b670ac3c41041
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522601"
---
# <a name="muteparticipantoperation-resource-type"></a><span data-ttu-id="a21b5-103">MuteParticipantOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="a21b5-103">MuteParticipantOperation resource type</span></span>

<span data-ttu-id="a21b5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a21b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a21b5-105">描述呼叫参与者静音操作的响应格式。</span><span class="sxs-lookup"><span data-stu-id="a21b5-105">Describes the response format of a call participant mute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="a21b5-106">属性</span><span class="sxs-lookup"><span data-stu-id="a21b5-106">Properties</span></span>

| <span data-ttu-id="a21b5-107">属性</span><span class="sxs-lookup"><span data-stu-id="a21b5-107">Property</span></span>                       | <span data-ttu-id="a21b5-108">类型</span><span class="sxs-lookup"><span data-stu-id="a21b5-108">Type</span></span>                        | <span data-ttu-id="a21b5-109">说明</span><span class="sxs-lookup"><span data-stu-id="a21b5-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a21b5-110">适用</span><span class="sxs-lookup"><span data-stu-id="a21b5-110">clientContext</span></span>                  | <span data-ttu-id="a21b5-111">String</span><span class="sxs-lookup"><span data-stu-id="a21b5-111">String</span></span>                      | <span data-ttu-id="a21b5-112">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="a21b5-112">Unique client context string.</span></span> <span data-ttu-id="a21b5-113">最多可以有256个字符。</span><span class="sxs-lookup"><span data-stu-id="a21b5-113">Can have a maximum of 256 characters.</span></span>                                                                               |
| <span data-ttu-id="a21b5-114">id</span><span class="sxs-lookup"><span data-stu-id="a21b5-114">id</span></span>                             | <span data-ttu-id="a21b5-115">String</span><span class="sxs-lookup"><span data-stu-id="a21b5-115">String</span></span>                      | <span data-ttu-id="a21b5-116">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="a21b5-116">The server operation ID.</span></span> <span data-ttu-id="a21b5-117">只读。</span><span class="sxs-lookup"><span data-stu-id="a21b5-117">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="a21b5-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="a21b5-118">resultInfo</span></span>                     | [<span data-ttu-id="a21b5-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="a21b5-119">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="a21b5-120">结果信息。</span><span class="sxs-lookup"><span data-stu-id="a21b5-120">The result information.</span></span>  <span data-ttu-id="a21b5-121">只读。</span><span class="sxs-lookup"><span data-stu-id="a21b5-121">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="a21b5-122">status</span><span class="sxs-lookup"><span data-stu-id="a21b5-122">status</span></span>                         | <span data-ttu-id="a21b5-123">String</span><span class="sxs-lookup"><span data-stu-id="a21b5-123">String</span></span>                      | <span data-ttu-id="a21b5-124">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="a21b5-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="a21b5-125">只读。</span><span class="sxs-lookup"><span data-stu-id="a21b5-125">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="a21b5-126">关系</span><span class="sxs-lookup"><span data-stu-id="a21b5-126">Relationships</span></span>
<span data-ttu-id="a21b5-127">无</span><span class="sxs-lookup"><span data-stu-id="a21b5-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a21b5-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a21b5-128">JSON representation</span></span>

<span data-ttu-id="a21b5-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a21b5-129">The following is a JSON representation of the resource.</span></span>

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
