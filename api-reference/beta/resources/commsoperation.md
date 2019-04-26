---
title: commsOperation 资源类型
description: 某个长时间运行的操作的状态。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 34e6ff32c250308e71e05cb5d5c4d04d5671535d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341356"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="c0b01-103">commsOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="c0b01-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0b01-104">某个长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="c0b01-104">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="c0b01-105">方法</span><span class="sxs-lookup"><span data-stu-id="c0b01-105">Methods</span></span>
<span data-ttu-id="c0b01-106">无</span><span class="sxs-lookup"><span data-stu-id="c0b01-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="c0b01-107">属性</span><span class="sxs-lookup"><span data-stu-id="c0b01-107">Properties</span></span>

| <span data-ttu-id="c0b01-108">属性</span><span class="sxs-lookup"><span data-stu-id="c0b01-108">Property</span></span>           | <span data-ttu-id="c0b01-109">类型</span><span class="sxs-lookup"><span data-stu-id="c0b01-109">Type</span></span>                        | <span data-ttu-id="c0b01-110">说明</span><span class="sxs-lookup"><span data-stu-id="c0b01-110">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="c0b01-111">适用</span><span class="sxs-lookup"><span data-stu-id="c0b01-111">clientContext</span></span>      | <span data-ttu-id="c0b01-112">String</span><span class="sxs-lookup"><span data-stu-id="c0b01-112">String</span></span>                      | <span data-ttu-id="c0b01-113">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="c0b01-113">The client context.</span></span>                                                             |
| <span data-ttu-id="c0b01-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0b01-114">createdDateTime</span></span>    | <span data-ttu-id="c0b01-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0b01-115">DateTimeOffset</span></span>              | <span data-ttu-id="c0b01-116">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="c0b01-116">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="c0b01-117">id</span><span class="sxs-lookup"><span data-stu-id="c0b01-117">id</span></span>                 | <span data-ttu-id="c0b01-118">String</span><span class="sxs-lookup"><span data-stu-id="c0b01-118">String</span></span>                      | <span data-ttu-id="c0b01-119">操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="c0b01-119">The operation id. Read-only.</span></span> <span data-ttu-id="c0b01-120">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="c0b01-120">Server generated.</span></span>                                  |
| <span data-ttu-id="c0b01-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="c0b01-121">lastActionDateTime</span></span> | <span data-ttu-id="c0b01-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0b01-122">DateTimeOffset</span></span>              | <span data-ttu-id="c0b01-123">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="c0b01-123">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="c0b01-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c0b01-124">resultInfo</span></span>         | [<span data-ttu-id="c0b01-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c0b01-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="c0b01-126">结果信息。</span><span class="sxs-lookup"><span data-stu-id="c0b01-126">The result information.</span></span> <span data-ttu-id="c0b01-127">只读。</span><span class="sxs-lookup"><span data-stu-id="c0b01-127">Read-only.</span></span> <span data-ttu-id="c0b01-128">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="c0b01-128">Server generated.</span></span>                            |
| <span data-ttu-id="c0b01-129">status</span><span class="sxs-lookup"><span data-stu-id="c0b01-129">status</span></span>             | <span data-ttu-id="c0b01-130">String</span><span class="sxs-lookup"><span data-stu-id="c0b01-130">String</span></span>                      | <span data-ttu-id="c0b01-131">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="c0b01-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="c0b01-132">只读。</span><span class="sxs-lookup"><span data-stu-id="c0b01-132">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c0b01-133">关系</span><span class="sxs-lookup"><span data-stu-id="c0b01-133">Relationships</span></span>
<span data-ttu-id="c0b01-134">无</span><span class="sxs-lookup"><span data-stu-id="c0b01-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0b01-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0b01-135">JSON representation</span></span>

<span data-ttu-id="c0b01-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0b01-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="c0b01-137">示例</span><span class="sxs-lookup"><span data-stu-id="c0b01-137">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo",
    "code": "200"
  },
  "status": "completed"
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
