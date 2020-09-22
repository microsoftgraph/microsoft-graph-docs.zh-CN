---
title: SubscribeToToneOperation 资源类型
description: 描述用于接收 DTMF 声音的订阅的创建响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a53405f58c568d17d040dd7368f39cef6838510c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094160"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="753ac-103">SubscribeToToneOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="753ac-103">SubscribeToToneOperation resource type</span></span>

<span data-ttu-id="753ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="753ac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="753ac-105">描述用于接收 DTMF 声音的订阅的创建响应格式。</span><span class="sxs-lookup"><span data-stu-id="753ac-105">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="753ac-106">属性</span><span class="sxs-lookup"><span data-stu-id="753ac-106">Properties</span></span>

| <span data-ttu-id="753ac-107">属性</span><span class="sxs-lookup"><span data-stu-id="753ac-107">Property</span></span>                       | <span data-ttu-id="753ac-108">类型</span><span class="sxs-lookup"><span data-stu-id="753ac-108">Type</span></span>                        | <span data-ttu-id="753ac-109">说明</span><span class="sxs-lookup"><span data-stu-id="753ac-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="753ac-110">适用</span><span class="sxs-lookup"><span data-stu-id="753ac-110">clientContext</span></span>                  | <span data-ttu-id="753ac-111">String</span><span class="sxs-lookup"><span data-stu-id="753ac-111">String</span></span>                      | <span data-ttu-id="753ac-112">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="753ac-112">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="753ac-113">id</span><span class="sxs-lookup"><span data-stu-id="753ac-113">id</span></span>                             | <span data-ttu-id="753ac-114">String</span><span class="sxs-lookup"><span data-stu-id="753ac-114">String</span></span>                      | <span data-ttu-id="753ac-115">服务器操作 ID。</span><span class="sxs-lookup"><span data-stu-id="753ac-115">The server operation ID.</span></span> <span data-ttu-id="753ac-116">只读。</span><span class="sxs-lookup"><span data-stu-id="753ac-116">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="753ac-117">status</span><span class="sxs-lookup"><span data-stu-id="753ac-117">status</span></span>                         | <span data-ttu-id="753ac-118">String</span><span class="sxs-lookup"><span data-stu-id="753ac-118">String</span></span>                      | <span data-ttu-id="753ac-119">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="753ac-119">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="753ac-120">只读。</span><span class="sxs-lookup"><span data-stu-id="753ac-120">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="753ac-121">关系</span><span class="sxs-lookup"><span data-stu-id="753ac-121">Relationships</span></span>
<span data-ttu-id="753ac-122">无</span><span class="sxs-lookup"><span data-stu-id="753ac-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="753ac-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="753ac-123">JSON representation</span></span>

<span data-ttu-id="753ac-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="753ac-124">The following is a JSON representation of the resource.</span></span>

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

