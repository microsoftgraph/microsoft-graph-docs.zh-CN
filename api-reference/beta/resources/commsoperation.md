---
title: commsOperation 资源类型
description: 某些长时间运行操作的状态。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5a82020741033f81d5a4394f2e32b3f0f76a6e03
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575644"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="229db-103">commsOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="229db-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="229db-104">某些长时间运行操作的状态。</span><span class="sxs-lookup"><span data-stu-id="229db-104">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="229db-105">方法</span><span class="sxs-lookup"><span data-stu-id="229db-105">Methods</span></span>
<span data-ttu-id="229db-106">无</span><span class="sxs-lookup"><span data-stu-id="229db-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="229db-107">属性</span><span class="sxs-lookup"><span data-stu-id="229db-107">Properties</span></span>

| <span data-ttu-id="229db-108">属性</span><span class="sxs-lookup"><span data-stu-id="229db-108">Property</span></span>           | <span data-ttu-id="229db-109">类型</span><span class="sxs-lookup"><span data-stu-id="229db-109">Type</span></span>                        | <span data-ttu-id="229db-110">说明</span><span class="sxs-lookup"><span data-stu-id="229db-110">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="229db-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="229db-111">clientContext</span></span>      | <span data-ttu-id="229db-112">String</span><span class="sxs-lookup"><span data-stu-id="229db-112">String</span></span>                      | <span data-ttu-id="229db-113">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="229db-113">The client context.</span></span>                                                             |
| <span data-ttu-id="229db-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="229db-114">createdDateTime</span></span>    | <span data-ttu-id="229db-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="229db-115">DateTimeOffset</span></span>              | <span data-ttu-id="229db-116">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="229db-116">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="229db-117">id</span><span class="sxs-lookup"><span data-stu-id="229db-117">id</span></span>                 | <span data-ttu-id="229db-118">字符串 （标识符）</span><span class="sxs-lookup"><span data-stu-id="229db-118">String (identifier)</span></span>         | <span data-ttu-id="229db-119">操作 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="229db-119">The operation id. Read-only.</span></span> <span data-ttu-id="229db-120">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="229db-120">Server generated.</span></span>                                  |
| <span data-ttu-id="229db-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="229db-121">lastActionDateTime</span></span> | <span data-ttu-id="229db-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="229db-122">DateTimeOffset</span></span>              | <span data-ttu-id="229db-123">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="229db-123">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="229db-124">errorInfo</span><span class="sxs-lookup"><span data-stu-id="229db-124">errorInfo</span></span>          | [<span data-ttu-id="229db-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="229db-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="229db-126">结果信息。</span><span class="sxs-lookup"><span data-stu-id="229db-126">The result information.</span></span> <span data-ttu-id="229db-127">只读。</span><span class="sxs-lookup"><span data-stu-id="229db-127">Read-only.</span></span> <span data-ttu-id="229db-128">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="229db-128">Server generated.</span></span>                            |
| <span data-ttu-id="229db-129">status</span><span class="sxs-lookup"><span data-stu-id="229db-129">status</span></span>             | <span data-ttu-id="229db-130">operationStatus</span><span class="sxs-lookup"><span data-stu-id="229db-130">operationStatus</span></span>             | <span data-ttu-id="229db-131">可取值为 `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="229db-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="229db-132">只读。</span><span class="sxs-lookup"><span data-stu-id="229db-132">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="229db-133">关系</span><span class="sxs-lookup"><span data-stu-id="229db-133">Relationships</span></span>
<span data-ttu-id="229db-134">无</span><span class="sxs-lookup"><span data-stu-id="229db-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="229db-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="229db-135">JSON representation</span></span>

<span data-ttu-id="229db-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="229db-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "errorInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "operationStatus"
}
```

## <a name="example"></a><span data-ttu-id="229db-137">示例</span><span class="sxs-lookup"><span data-stu-id="229db-137">Example</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/commsoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
