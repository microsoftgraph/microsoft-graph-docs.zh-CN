---
title: commsOperation 资源类型
description: 某些长时间运行操作的状态。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b7914bd9692b4d9a94294f9a09659467e10550a6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515746"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="18d66-103">commsOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="18d66-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18d66-104">某些长时间运行操作的状态。</span><span class="sxs-lookup"><span data-stu-id="18d66-104">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="18d66-105">方法</span><span class="sxs-lookup"><span data-stu-id="18d66-105">Methods</span></span>
<span data-ttu-id="18d66-106">无</span><span class="sxs-lookup"><span data-stu-id="18d66-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="18d66-107">属性</span><span class="sxs-lookup"><span data-stu-id="18d66-107">Properties</span></span>

| <span data-ttu-id="18d66-108">属性</span><span class="sxs-lookup"><span data-stu-id="18d66-108">Property</span></span>           | <span data-ttu-id="18d66-109">类型</span><span class="sxs-lookup"><span data-stu-id="18d66-109">Type</span></span>                        | <span data-ttu-id="18d66-110">说明</span><span class="sxs-lookup"><span data-stu-id="18d66-110">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="18d66-111">ClientContext</span><span class="sxs-lookup"><span data-stu-id="18d66-111">clientContext</span></span>      | <span data-ttu-id="18d66-112">String</span><span class="sxs-lookup"><span data-stu-id="18d66-112">String</span></span>                      | <span data-ttu-id="18d66-113">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="18d66-113">The client context.</span></span>                                                             |
| <span data-ttu-id="18d66-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18d66-114">createdDateTime</span></span>    | <span data-ttu-id="18d66-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18d66-115">DateTimeOffset</span></span>              | <span data-ttu-id="18d66-116">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="18d66-116">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="18d66-117">id</span><span class="sxs-lookup"><span data-stu-id="18d66-117">id</span></span>                 | <span data-ttu-id="18d66-118">字串符号</span><span class="sxs-lookup"><span data-stu-id="18d66-118">String</span></span>                      | <span data-ttu-id="18d66-119">操作 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="18d66-119">The operation id. Read-only.</span></span> <span data-ttu-id="18d66-120">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="18d66-120">Server generated.</span></span>                                  |
| <span data-ttu-id="18d66-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="18d66-121">lastActionDateTime</span></span> | <span data-ttu-id="18d66-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18d66-122">DateTimeOffset</span></span>              | <span data-ttu-id="18d66-123">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="18d66-123">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="18d66-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="18d66-124">resultInfo</span></span>         | [<span data-ttu-id="18d66-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="18d66-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="18d66-126">结果的信息。</span><span class="sxs-lookup"><span data-stu-id="18d66-126">The result information.</span></span> <span data-ttu-id="18d66-127">只读。</span><span class="sxs-lookup"><span data-stu-id="18d66-127">Read-only.</span></span> <span data-ttu-id="18d66-128">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="18d66-128">Server generated.</span></span>                            |
| <span data-ttu-id="18d66-129">status</span><span class="sxs-lookup"><span data-stu-id="18d66-129">status</span></span>             | <span data-ttu-id="18d66-130">String</span><span class="sxs-lookup"><span data-stu-id="18d66-130">String</span></span>                      | <span data-ttu-id="18d66-131">可取值为 `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="18d66-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="18d66-132">只读。</span><span class="sxs-lookup"><span data-stu-id="18d66-132">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="18d66-133">关系</span><span class="sxs-lookup"><span data-stu-id="18d66-133">Relationships</span></span>
<span data-ttu-id="18d66-134">无</span><span class="sxs-lookup"><span data-stu-id="18d66-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18d66-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="18d66-135">JSON representation</span></span>

<span data-ttu-id="18d66-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18d66-136">The following is a JSON representation of the resource.</span></span>

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
  "resultInfo": { "@odata.type": "#microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="18d66-137">示例</span><span class="sxs-lookup"><span data-stu-id="18d66-137">Example</span></span>

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
    "@odata.type": "#microsoft.graph.resultInfo",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/commsoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
