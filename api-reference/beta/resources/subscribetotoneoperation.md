---
title: SubscribeToToneOperation 资源类型
description: 描述用于接收 DTMF 声音的订阅的创建响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e35b3fe674c9f92b7dab723325d658facf13962f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520287"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="b3aea-103">SubscribeToToneOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3aea-103">SubscribeToToneOperation resource type</span></span>

<span data-ttu-id="b3aea-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b3aea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3aea-105">描述用于接收 DTMF 声音的订阅的创建响应格式。</span><span class="sxs-lookup"><span data-stu-id="b3aea-105">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="b3aea-106">属性</span><span class="sxs-lookup"><span data-stu-id="b3aea-106">Properties</span></span>

| <span data-ttu-id="b3aea-107">属性</span><span class="sxs-lookup"><span data-stu-id="b3aea-107">Property</span></span>                       | <span data-ttu-id="b3aea-108">类型</span><span class="sxs-lookup"><span data-stu-id="b3aea-108">Type</span></span>                        | <span data-ttu-id="b3aea-109">说明</span><span class="sxs-lookup"><span data-stu-id="b3aea-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b3aea-110">适用</span><span class="sxs-lookup"><span data-stu-id="b3aea-110">clientContext</span></span>                  | <span data-ttu-id="b3aea-111">String</span><span class="sxs-lookup"><span data-stu-id="b3aea-111">String</span></span>                      | <span data-ttu-id="b3aea-112">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="b3aea-112">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="b3aea-113">id</span><span class="sxs-lookup"><span data-stu-id="b3aea-113">id</span></span>                             | <span data-ttu-id="b3aea-114">String</span><span class="sxs-lookup"><span data-stu-id="b3aea-114">String</span></span>                      | <span data-ttu-id="b3aea-115">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="b3aea-115">The server operation ID.</span></span> <span data-ttu-id="b3aea-116">只读。</span><span class="sxs-lookup"><span data-stu-id="b3aea-116">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="b3aea-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b3aea-117">resultInfo</span></span>                     | [<span data-ttu-id="b3aea-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b3aea-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="b3aea-119">结果信息。</span><span class="sxs-lookup"><span data-stu-id="b3aea-119">The result information.</span></span>  <span data-ttu-id="b3aea-120">只读。</span><span class="sxs-lookup"><span data-stu-id="b3aea-120">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="b3aea-121">status</span><span class="sxs-lookup"><span data-stu-id="b3aea-121">status</span></span>                         | <span data-ttu-id="b3aea-122">String</span><span class="sxs-lookup"><span data-stu-id="b3aea-122">String</span></span>                      | <span data-ttu-id="b3aea-123">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b3aea-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="b3aea-124">只读。</span><span class="sxs-lookup"><span data-stu-id="b3aea-124">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="b3aea-125">关系</span><span class="sxs-lookup"><span data-stu-id="b3aea-125">Relationships</span></span>
<span data-ttu-id="b3aea-126">无</span><span class="sxs-lookup"><span data-stu-id="b3aea-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3aea-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3aea-127">JSON representation</span></span>

<span data-ttu-id="b3aea-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3aea-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscribeToToneOperation"
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
  "description": "subscribeToToneOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
