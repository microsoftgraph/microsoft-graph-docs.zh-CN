---
title: commsOperation 资源类型
description: 某个长时间运行的操作的状态。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b7914bd9692b4d9a94294f9a09659467e10550a6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460595"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="ad59b-103">commsOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad59b-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad59b-104">某个长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="ad59b-104">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="ad59b-105">方法</span><span class="sxs-lookup"><span data-stu-id="ad59b-105">Methods</span></span>
<span data-ttu-id="ad59b-106">无</span><span class="sxs-lookup"><span data-stu-id="ad59b-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="ad59b-107">属性</span><span class="sxs-lookup"><span data-stu-id="ad59b-107">Properties</span></span>

| <span data-ttu-id="ad59b-108">属性</span><span class="sxs-lookup"><span data-stu-id="ad59b-108">Property</span></span>           | <span data-ttu-id="ad59b-109">类型</span><span class="sxs-lookup"><span data-stu-id="ad59b-109">Type</span></span>                        | <span data-ttu-id="ad59b-110">说明</span><span class="sxs-lookup"><span data-stu-id="ad59b-110">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="ad59b-111">适用</span><span class="sxs-lookup"><span data-stu-id="ad59b-111">clientContext</span></span>      | <span data-ttu-id="ad59b-112">字符串</span><span class="sxs-lookup"><span data-stu-id="ad59b-112">String</span></span>                      | <span data-ttu-id="ad59b-113">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="ad59b-113">The client context.</span></span>                                                             |
| <span data-ttu-id="ad59b-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad59b-114">createdDateTime</span></span>    | <span data-ttu-id="ad59b-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad59b-115">DateTimeOffset</span></span>              | <span data-ttu-id="ad59b-116">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="ad59b-116">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="ad59b-117">id</span><span class="sxs-lookup"><span data-stu-id="ad59b-117">id</span></span>                 | <span data-ttu-id="ad59b-118">String</span><span class="sxs-lookup"><span data-stu-id="ad59b-118">String</span></span>                      | <span data-ttu-id="ad59b-119">操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="ad59b-119">The operation id. Read-only.</span></span> <span data-ttu-id="ad59b-120">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="ad59b-120">Server generated.</span></span>                                  |
| <span data-ttu-id="ad59b-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="ad59b-121">lastActionDateTime</span></span> | <span data-ttu-id="ad59b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad59b-122">DateTimeOffset</span></span>              | <span data-ttu-id="ad59b-123">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="ad59b-123">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="ad59b-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="ad59b-124">resultInfo</span></span>         | [<span data-ttu-id="ad59b-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="ad59b-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="ad59b-126">结果信息。</span><span class="sxs-lookup"><span data-stu-id="ad59b-126">The result information.</span></span> <span data-ttu-id="ad59b-127">只读。</span><span class="sxs-lookup"><span data-stu-id="ad59b-127">Read-only.</span></span> <span data-ttu-id="ad59b-128">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="ad59b-128">Server generated.</span></span>                            |
| <span data-ttu-id="ad59b-129">status</span><span class="sxs-lookup"><span data-stu-id="ad59b-129">status</span></span>             | <span data-ttu-id="ad59b-130">String</span><span class="sxs-lookup"><span data-stu-id="ad59b-130">String</span></span>                      | <span data-ttu-id="ad59b-131">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="ad59b-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="ad59b-132">只读。</span><span class="sxs-lookup"><span data-stu-id="ad59b-132">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ad59b-133">关系</span><span class="sxs-lookup"><span data-stu-id="ad59b-133">Relationships</span></span>
<span data-ttu-id="ad59b-134">无</span><span class="sxs-lookup"><span data-stu-id="ad59b-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad59b-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad59b-135">JSON representation</span></span>

<span data-ttu-id="ad59b-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad59b-136">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="ad59b-137">示例</span><span class="sxs-lookup"><span data-stu-id="ad59b-137">Example</span></span>

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
