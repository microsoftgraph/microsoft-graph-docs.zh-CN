---
title: commsOperation 资源类型
description: 某个长时间运行的操作的状态。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a10b652179a8a3d369c07d34cb2681c4986b3abf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012896"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="0ed8e-103">commsOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ed8e-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ed8e-104">某个长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="0ed8e-104">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="0ed8e-105">方法</span><span class="sxs-lookup"><span data-stu-id="0ed8e-105">Methods</span></span>
<span data-ttu-id="0ed8e-106">无</span><span class="sxs-lookup"><span data-stu-id="0ed8e-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="0ed8e-107">属性</span><span class="sxs-lookup"><span data-stu-id="0ed8e-107">Properties</span></span>

| <span data-ttu-id="0ed8e-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ed8e-108">Property</span></span>           | <span data-ttu-id="0ed8e-109">类型</span><span class="sxs-lookup"><span data-stu-id="0ed8e-109">Type</span></span>                        | <span data-ttu-id="0ed8e-110">说明</span><span class="sxs-lookup"><span data-stu-id="0ed8e-110">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="0ed8e-111">适用</span><span class="sxs-lookup"><span data-stu-id="0ed8e-111">clientContext</span></span>      | <span data-ttu-id="0ed8e-112">String</span><span class="sxs-lookup"><span data-stu-id="0ed8e-112">String</span></span>                      | <span data-ttu-id="0ed8e-113">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="0ed8e-113">The client context.</span></span>                                                             |
| <span data-ttu-id="0ed8e-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ed8e-114">createdDateTime</span></span>    | <span data-ttu-id="0ed8e-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ed8e-115">DateTimeOffset</span></span>              | <span data-ttu-id="0ed8e-116">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="0ed8e-116">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="0ed8e-117">id</span><span class="sxs-lookup"><span data-stu-id="0ed8e-117">id</span></span>                 | <span data-ttu-id="0ed8e-118">String</span><span class="sxs-lookup"><span data-stu-id="0ed8e-118">String</span></span>                      | <span data-ttu-id="0ed8e-119">操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="0ed8e-119">The operation id. Read-only.</span></span> <span data-ttu-id="0ed8e-120">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="0ed8e-120">Server generated.</span></span>                                  |
| <span data-ttu-id="0ed8e-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="0ed8e-121">lastActionDateTime</span></span> | <span data-ttu-id="0ed8e-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ed8e-122">DateTimeOffset</span></span>              | <span data-ttu-id="0ed8e-123">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="0ed8e-123">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="0ed8e-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0ed8e-124">resultInfo</span></span>         | [<span data-ttu-id="0ed8e-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0ed8e-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="0ed8e-126">结果信息。</span><span class="sxs-lookup"><span data-stu-id="0ed8e-126">The result information.</span></span> <span data-ttu-id="0ed8e-127">只读。</span><span class="sxs-lookup"><span data-stu-id="0ed8e-127">Read-only.</span></span> <span data-ttu-id="0ed8e-128">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="0ed8e-128">Server generated.</span></span>                            |
| <span data-ttu-id="0ed8e-129">status</span><span class="sxs-lookup"><span data-stu-id="0ed8e-129">status</span></span>             | <span data-ttu-id="0ed8e-130">String</span><span class="sxs-lookup"><span data-stu-id="0ed8e-130">String</span></span>                      | <span data-ttu-id="0ed8e-131">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="0ed8e-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="0ed8e-132">只读。</span><span class="sxs-lookup"><span data-stu-id="0ed8e-132">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0ed8e-133">关系</span><span class="sxs-lookup"><span data-stu-id="0ed8e-133">Relationships</span></span>
<span data-ttu-id="0ed8e-134">无</span><span class="sxs-lookup"><span data-stu-id="0ed8e-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ed8e-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ed8e-135">JSON representation</span></span>

<span data-ttu-id="0ed8e-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ed8e-136">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="0ed8e-137">示例</span><span class="sxs-lookup"><span data-stu-id="0ed8e-137">Example</span></span>

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
