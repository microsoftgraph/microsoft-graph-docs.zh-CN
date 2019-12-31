---
title: SubscribeToToneOperation 资源类型
description: 描述用于接收 DTMF 声音的订阅的创建响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0b10062ed51aae20d6d4268da349b9b429d6c528
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913686"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="9df5a-103">SubscribeToToneOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="9df5a-103">SubscribeToToneOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9df5a-104">描述用于接收 DTMF 声音的订阅的创建响应格式。</span><span class="sxs-lookup"><span data-stu-id="9df5a-104">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="9df5a-105">属性</span><span class="sxs-lookup"><span data-stu-id="9df5a-105">Properties</span></span>

| <span data-ttu-id="9df5a-106">属性</span><span class="sxs-lookup"><span data-stu-id="9df5a-106">Property</span></span>                       | <span data-ttu-id="9df5a-107">类型</span><span class="sxs-lookup"><span data-stu-id="9df5a-107">Type</span></span>                        | <span data-ttu-id="9df5a-108">说明</span><span class="sxs-lookup"><span data-stu-id="9df5a-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9df5a-109">适用</span><span class="sxs-lookup"><span data-stu-id="9df5a-109">clientContext</span></span>                  | <span data-ttu-id="9df5a-110">String</span><span class="sxs-lookup"><span data-stu-id="9df5a-110">String</span></span>                      | <span data-ttu-id="9df5a-111">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="9df5a-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="9df5a-112">id</span><span class="sxs-lookup"><span data-stu-id="9df5a-112">id</span></span>                             | <span data-ttu-id="9df5a-113">String</span><span class="sxs-lookup"><span data-stu-id="9df5a-113">String</span></span>                      | <span data-ttu-id="9df5a-114">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="9df5a-114">The server operation ID.</span></span> <span data-ttu-id="9df5a-115">只读。</span><span class="sxs-lookup"><span data-stu-id="9df5a-115">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="9df5a-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9df5a-116">resultInfo</span></span>                     | [<span data-ttu-id="9df5a-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9df5a-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="9df5a-118">结果信息。</span><span class="sxs-lookup"><span data-stu-id="9df5a-118">The result information.</span></span>  <span data-ttu-id="9df5a-119">只读。</span><span class="sxs-lookup"><span data-stu-id="9df5a-119">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="9df5a-120">状态</span><span class="sxs-lookup"><span data-stu-id="9df5a-120">status</span></span>                         | <span data-ttu-id="9df5a-121">String</span><span class="sxs-lookup"><span data-stu-id="9df5a-121">String</span></span>                      | <span data-ttu-id="9df5a-122">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="9df5a-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="9df5a-123">只读。</span><span class="sxs-lookup"><span data-stu-id="9df5a-123">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="9df5a-124">关系</span><span class="sxs-lookup"><span data-stu-id="9df5a-124">Relationships</span></span>
<span data-ttu-id="9df5a-125">无</span><span class="sxs-lookup"><span data-stu-id="9df5a-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9df5a-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9df5a-126">JSON representation</span></span>

<span data-ttu-id="9df5a-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9df5a-127">The following is a JSON representation of the resource.</span></span>

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
