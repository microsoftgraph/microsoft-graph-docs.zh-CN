---
title: commsOperation 资源类型
description: 某个长时间运行的操作的状态。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7a73777ae8477275e9071645ce092ca1a4187527
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507588"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="d788f-103">commsOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="d788f-103">commsOperation resource type</span></span>

<span data-ttu-id="d788f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d788f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d788f-105">表示某个长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="d788f-105">Represents the status of certain long-running operations.</span></span>

<span data-ttu-id="d788f-106">此资源可以作为对操作的响应返回，也可以作为[commsNotification](commsNotification.md)的内容返回。</span><span class="sxs-lookup"><span data-stu-id="d788f-106">This resource can be returned as the response to an action, or as the content of a [commsNotification](commsNotification.md).</span></span>  

<span data-ttu-id="d788f-107">如果作为操作的响应返回，则状态指示是否会出现后续通知。</span><span class="sxs-lookup"><span data-stu-id="d788f-107">When it is returned as a response to an action, the status indicates whether there will be subsequent notifications.</span></span> <span data-ttu-id="d788f-108">例如，如果返回状态为`completed`或`failed`的操作，则不会通过通知通道进行任何后续操作。</span><span class="sxs-lookup"><span data-stu-id="d788f-108">If, for example, an operation with status of `completed` or `failed` is returned,  there will not be any subsequent operation via the notification channel.</span></span> 

<span data-ttu-id="d788f-109">如果`null`操作或返回状态为`notStarted`或`running`的操作，后续更新将通过通知通道发出。</span><span class="sxs-lookup"><span data-stu-id="d788f-109">If a `null` operation, or an operation with a status of `notStarted` or `running` is returned, subsequent updates will come via the notification channel.</span></span>

## <a name="properties"></a><span data-ttu-id="d788f-110">属性</span><span class="sxs-lookup"><span data-stu-id="d788f-110">Properties</span></span>

| <span data-ttu-id="d788f-111">属性</span><span class="sxs-lookup"><span data-stu-id="d788f-111">Property</span></span>           | <span data-ttu-id="d788f-112">类型</span><span class="sxs-lookup"><span data-stu-id="d788f-112">Type</span></span>                        | <span data-ttu-id="d788f-113">说明</span><span class="sxs-lookup"><span data-stu-id="d788f-113">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="d788f-114">适用</span><span class="sxs-lookup"><span data-stu-id="d788f-114">clientContext</span></span>      | <span data-ttu-id="d788f-115">String</span><span class="sxs-lookup"><span data-stu-id="d788f-115">String</span></span>                      | <span data-ttu-id="d788f-116">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="d788f-116">Unique Client Context string.</span></span> <span data-ttu-id="d788f-117">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="d788f-117">Max limit is 256 chars.</span></span>                           |
| <span data-ttu-id="d788f-118">id</span><span class="sxs-lookup"><span data-stu-id="d788f-118">id</span></span>                 | <span data-ttu-id="d788f-119">String</span><span class="sxs-lookup"><span data-stu-id="d788f-119">String</span></span>                      | <span data-ttu-id="d788f-120">操作 ID。</span><span class="sxs-lookup"><span data-stu-id="d788f-120">The operation ID.</span></span> <span data-ttu-id="d788f-121">只读。</span><span class="sxs-lookup"><span data-stu-id="d788f-121">Read-only.</span></span>                                                    |
| <span data-ttu-id="d788f-122">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d788f-122">resultInfo</span></span>         | [<span data-ttu-id="d788f-123">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d788f-123">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="d788f-124">结果信息。</span><span class="sxs-lookup"><span data-stu-id="d788f-124">The result information.</span></span> <span data-ttu-id="d788f-125">只读。</span><span class="sxs-lookup"><span data-stu-id="d788f-125">Read-only.</span></span>                                              |
| <span data-ttu-id="d788f-126">status</span><span class="sxs-lookup"><span data-stu-id="d788f-126">status</span></span>             | <span data-ttu-id="d788f-127">String</span><span class="sxs-lookup"><span data-stu-id="d788f-127">String</span></span>                      | <span data-ttu-id="d788f-128">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="d788f-128">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="d788f-129">只读。</span><span class="sxs-lookup"><span data-stu-id="d788f-129">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d788f-130">关系</span><span class="sxs-lookup"><span data-stu-id="d788f-130">Relationships</span></span>
<span data-ttu-id="d788f-131">无</span><span class="sxs-lookup"><span data-stu-id="d788f-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d788f-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d788f-132">JSON representation</span></span>

<span data-ttu-id="d788f-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d788f-133">The following is a JSON representation of the resource.</span></span>

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
