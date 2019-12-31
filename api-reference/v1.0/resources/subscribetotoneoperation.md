---
title: SubscribeToToneOperation 资源类型
description: 描述用于接收 DTMF 声音的订阅的创建响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6d1e42d375dd53fcb71ae049622c59d2d31b3406
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913539"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="ece8f-103">SubscribeToToneOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ece8f-103">SubscribeToToneOperation resource type</span></span>

<span data-ttu-id="ece8f-104">描述用于接收 DTMF 声音的订阅的创建响应格式。</span><span class="sxs-lookup"><span data-stu-id="ece8f-104">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="ece8f-105">属性</span><span class="sxs-lookup"><span data-stu-id="ece8f-105">Properties</span></span>

| <span data-ttu-id="ece8f-106">属性</span><span class="sxs-lookup"><span data-stu-id="ece8f-106">Property</span></span>                       | <span data-ttu-id="ece8f-107">类型</span><span class="sxs-lookup"><span data-stu-id="ece8f-107">Type</span></span>                        | <span data-ttu-id="ece8f-108">说明</span><span class="sxs-lookup"><span data-stu-id="ece8f-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ece8f-109">适用</span><span class="sxs-lookup"><span data-stu-id="ece8f-109">clientContext</span></span>                  | <span data-ttu-id="ece8f-110">String</span><span class="sxs-lookup"><span data-stu-id="ece8f-110">String</span></span>                      | <span data-ttu-id="ece8f-111">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="ece8f-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="ece8f-112">id</span><span class="sxs-lookup"><span data-stu-id="ece8f-112">id</span></span>                             | <span data-ttu-id="ece8f-113">String</span><span class="sxs-lookup"><span data-stu-id="ece8f-113">String</span></span>                      | <span data-ttu-id="ece8f-114">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="ece8f-114">The server operation ID.</span></span> <span data-ttu-id="ece8f-115">只读。</span><span class="sxs-lookup"><span data-stu-id="ece8f-115">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="ece8f-116">状态</span><span class="sxs-lookup"><span data-stu-id="ece8f-116">status</span></span>                         | <span data-ttu-id="ece8f-117">String</span><span class="sxs-lookup"><span data-stu-id="ece8f-117">String</span></span>                      | <span data-ttu-id="ece8f-118">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="ece8f-118">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="ece8f-119">只读。</span><span class="sxs-lookup"><span data-stu-id="ece8f-119">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="ece8f-120">关系</span><span class="sxs-lookup"><span data-stu-id="ece8f-120">Relationships</span></span>
<span data-ttu-id="ece8f-121">无</span><span class="sxs-lookup"><span data-stu-id="ece8f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ece8f-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ece8f-122">JSON representation</span></span>

<span data-ttu-id="ece8f-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ece8f-123">The following is a JSON representation of the resource.</span></span>

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
