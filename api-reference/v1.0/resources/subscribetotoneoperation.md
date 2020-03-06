---
title: SubscribeToToneOperation 资源类型
description: 描述用于接收 DTMF 声音的订阅的创建响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f29d385060d93b8de54ee27f9f948f83e3ad2711
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533614"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="8a497-103">SubscribeToToneOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a497-103">SubscribeToToneOperation resource type</span></span>

<span data-ttu-id="8a497-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a497-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a497-105">描述用于接收 DTMF 声音的订阅的创建响应格式。</span><span class="sxs-lookup"><span data-stu-id="8a497-105">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="8a497-106">属性</span><span class="sxs-lookup"><span data-stu-id="8a497-106">Properties</span></span>

| <span data-ttu-id="8a497-107">属性</span><span class="sxs-lookup"><span data-stu-id="8a497-107">Property</span></span>                       | <span data-ttu-id="8a497-108">类型</span><span class="sxs-lookup"><span data-stu-id="8a497-108">Type</span></span>                        | <span data-ttu-id="8a497-109">说明</span><span class="sxs-lookup"><span data-stu-id="8a497-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8a497-110">适用</span><span class="sxs-lookup"><span data-stu-id="8a497-110">clientContext</span></span>                  | <span data-ttu-id="8a497-111">字符串</span><span class="sxs-lookup"><span data-stu-id="8a497-111">String</span></span>                      | <span data-ttu-id="8a497-112">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="8a497-112">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="8a497-113">id</span><span class="sxs-lookup"><span data-stu-id="8a497-113">id</span></span>                             | <span data-ttu-id="8a497-114">String</span><span class="sxs-lookup"><span data-stu-id="8a497-114">String</span></span>                      | <span data-ttu-id="8a497-115">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="8a497-115">The server operation ID.</span></span> <span data-ttu-id="8a497-116">只读。</span><span class="sxs-lookup"><span data-stu-id="8a497-116">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="8a497-117">状态</span><span class="sxs-lookup"><span data-stu-id="8a497-117">status</span></span>                         | <span data-ttu-id="8a497-118">String</span><span class="sxs-lookup"><span data-stu-id="8a497-118">String</span></span>                      | <span data-ttu-id="8a497-119">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="8a497-119">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="8a497-120">只读。</span><span class="sxs-lookup"><span data-stu-id="8a497-120">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="8a497-121">关系</span><span class="sxs-lookup"><span data-stu-id="8a497-121">Relationships</span></span>
<span data-ttu-id="8a497-122">无</span><span class="sxs-lookup"><span data-stu-id="8a497-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a497-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a497-123">JSON representation</span></span>

<span data-ttu-id="8a497-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a497-124">The following is a JSON representation of the resource.</span></span>

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
