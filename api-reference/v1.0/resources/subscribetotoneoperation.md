---
title: SubscribeToToneOperation 资源类型
description: 描述用于接收 DTMF 声音的订阅的创建响应格式。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e1251e4d62c9c1fb7f4806f6a0ec1e0ea0bf13a8
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865759"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="d1938-103">SubscribeToToneOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1938-103">SubscribeToToneOperation resource type</span></span>

<span data-ttu-id="d1938-104">描述用于接收 DTMF 声音的订阅的创建响应格式。</span><span class="sxs-lookup"><span data-stu-id="d1938-104">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="d1938-105">属性</span><span class="sxs-lookup"><span data-stu-id="d1938-105">Properties</span></span>

| <span data-ttu-id="d1938-106">属性</span><span class="sxs-lookup"><span data-stu-id="d1938-106">Property</span></span>                       | <span data-ttu-id="d1938-107">类型</span><span class="sxs-lookup"><span data-stu-id="d1938-107">Type</span></span>                        | <span data-ttu-id="d1938-108">说明</span><span class="sxs-lookup"><span data-stu-id="d1938-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d1938-109">适用</span><span class="sxs-lookup"><span data-stu-id="d1938-109">clientContext</span></span>                  | <span data-ttu-id="d1938-110">String</span><span class="sxs-lookup"><span data-stu-id="d1938-110">String</span></span>                      | <span data-ttu-id="d1938-111">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="d1938-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="d1938-112">id</span><span class="sxs-lookup"><span data-stu-id="d1938-112">id</span></span>                             | <span data-ttu-id="d1938-113">String</span><span class="sxs-lookup"><span data-stu-id="d1938-113">String</span></span>                      | <span data-ttu-id="d1938-114">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="d1938-114">The server operation ID.</span></span> <span data-ttu-id="d1938-115">只读。</span><span class="sxs-lookup"><span data-stu-id="d1938-115">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="d1938-116">状态</span><span class="sxs-lookup"><span data-stu-id="d1938-116">status</span></span>                         | <span data-ttu-id="d1938-117">String</span><span class="sxs-lookup"><span data-stu-id="d1938-117">String</span></span>                      | <span data-ttu-id="d1938-118">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="d1938-118">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="d1938-119">只读。</span><span class="sxs-lookup"><span data-stu-id="d1938-119">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="d1938-120">关系</span><span class="sxs-lookup"><span data-stu-id="d1938-120">Relationships</span></span>
<span data-ttu-id="d1938-121">无</span><span class="sxs-lookup"><span data-stu-id="d1938-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1938-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1938-122">JSON representation</span></span>

<span data-ttu-id="d1938-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1938-123">The following is a JSON representation of the resource.</span></span>

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
