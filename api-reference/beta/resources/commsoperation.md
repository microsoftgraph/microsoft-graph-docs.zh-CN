---
title: commsOperation 资源类型
description: 某个长时间运行的操作的状态。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f0b10fc1871f4991f339ff643f450dbfefa3b85c
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913343"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="9d75e-103">commsOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d75e-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d75e-104">表示某个长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="9d75e-104">Represents the status of certain long-running operations.</span></span>

<span data-ttu-id="9d75e-105">此资源可以作为对操作的响应返回，也可以作为[commsNotification](commsNotification.md)的内容返回。</span><span class="sxs-lookup"><span data-stu-id="9d75e-105">This resource can be returned as the response to an action, or as the content of a [commsNotification](commsNotification.md).</span></span>  

<span data-ttu-id="9d75e-106">如果作为操作的响应返回，则状态指示是否会出现后续通知。</span><span class="sxs-lookup"><span data-stu-id="9d75e-106">When it is returned as a response to an action, the status indicates whether there will be subsequent notifications.</span></span> <span data-ttu-id="9d75e-107">例如，如果返回状态为`completed`或`failed`的操作，则不会通过通知通道进行任何后续操作。</span><span class="sxs-lookup"><span data-stu-id="9d75e-107">If, for example, an operation with status of `completed` or `failed` is returned,  there will not be any subsequent operation via the notification channel.</span></span> 

<span data-ttu-id="9d75e-108">如果`null`操作或返回状态为`notStarted`或`running`的操作，后续更新将通过通知通道发出。</span><span class="sxs-lookup"><span data-stu-id="9d75e-108">If a `null` operation, or an operation with a status of `notStarted` or `running` is returned, subsequent updates will come via the notification channel.</span></span>

## <a name="properties"></a><span data-ttu-id="9d75e-109">属性</span><span class="sxs-lookup"><span data-stu-id="9d75e-109">Properties</span></span>

| <span data-ttu-id="9d75e-110">属性</span><span class="sxs-lookup"><span data-stu-id="9d75e-110">Property</span></span>           | <span data-ttu-id="9d75e-111">类型</span><span class="sxs-lookup"><span data-stu-id="9d75e-111">Type</span></span>                        | <span data-ttu-id="9d75e-112">说明</span><span class="sxs-lookup"><span data-stu-id="9d75e-112">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="9d75e-113">适用</span><span class="sxs-lookup"><span data-stu-id="9d75e-113">clientContext</span></span>      | <span data-ttu-id="9d75e-114">String</span><span class="sxs-lookup"><span data-stu-id="9d75e-114">String</span></span>                      | <span data-ttu-id="9d75e-115">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="9d75e-115">Unique Client Context string.</span></span> <span data-ttu-id="9d75e-116">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="9d75e-116">Max limit is 256 chars.</span></span>                           |
| <span data-ttu-id="9d75e-117">id</span><span class="sxs-lookup"><span data-stu-id="9d75e-117">id</span></span>                 | <span data-ttu-id="9d75e-118">String</span><span class="sxs-lookup"><span data-stu-id="9d75e-118">String</span></span>                      | <span data-ttu-id="9d75e-119">操作 ID。</span><span class="sxs-lookup"><span data-stu-id="9d75e-119">The operation ID.</span></span> <span data-ttu-id="9d75e-120">只读。</span><span class="sxs-lookup"><span data-stu-id="9d75e-120">Read-only.</span></span>                                                    |
| <span data-ttu-id="9d75e-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9d75e-121">resultInfo</span></span>         | [<span data-ttu-id="9d75e-122">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9d75e-122">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="9d75e-123">结果信息。</span><span class="sxs-lookup"><span data-stu-id="9d75e-123">The result information.</span></span> <span data-ttu-id="9d75e-124">只读。</span><span class="sxs-lookup"><span data-stu-id="9d75e-124">Read-only.</span></span>                                              |
| <span data-ttu-id="9d75e-125">状态</span><span class="sxs-lookup"><span data-stu-id="9d75e-125">status</span></span>             | <span data-ttu-id="9d75e-126">String</span><span class="sxs-lookup"><span data-stu-id="9d75e-126">String</span></span>                      | <span data-ttu-id="9d75e-127">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="9d75e-127">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="9d75e-128">只读。</span><span class="sxs-lookup"><span data-stu-id="9d75e-128">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9d75e-129">关系</span><span class="sxs-lookup"><span data-stu-id="9d75e-129">Relationships</span></span>
<span data-ttu-id="9d75e-130">无</span><span class="sxs-lookup"><span data-stu-id="9d75e-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d75e-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d75e-131">JSON representation</span></span>

<span data-ttu-id="9d75e-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d75e-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
