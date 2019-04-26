---
title: 操作资源类型
description: 长时间运行的操作的状态。
localization_priority: Normal
ms.openlocfilehash: 3ad9848387dab2de928f7ace2fa4b905720be615
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568896"
---
# <a name="operation-resource-type"></a><span data-ttu-id="015a4-103">操作资源类型</span><span class="sxs-lookup"><span data-stu-id="015a4-103">operation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="015a4-104">长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="015a4-104">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="015a4-105">方法</span><span class="sxs-lookup"><span data-stu-id="015a4-105">Methods</span></span>

<span data-ttu-id="015a4-106">无</span><span class="sxs-lookup"><span data-stu-id="015a4-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="015a4-107">属性</span><span class="sxs-lookup"><span data-stu-id="015a4-107">Properties</span></span>

| <span data-ttu-id="015a4-108">属性</span><span class="sxs-lookup"><span data-stu-id="015a4-108">Property</span></span>           | <span data-ttu-id="015a4-109">类型</span><span class="sxs-lookup"><span data-stu-id="015a4-109">Type</span></span>            | <span data-ttu-id="015a4-110">说明</span><span class="sxs-lookup"><span data-stu-id="015a4-110">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="015a4-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="015a4-111">createdDateTime</span></span>    | <span data-ttu-id="015a4-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="015a4-112">DateTimeOffset</span></span>  | <span data-ttu-id="015a4-113">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="015a4-113">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="015a4-114">id</span><span class="sxs-lookup"><span data-stu-id="015a4-114">id</span></span>                 | <span data-ttu-id="015a4-115">String</span><span class="sxs-lookup"><span data-stu-id="015a4-115">String</span></span>          | <span data-ttu-id="015a4-116">操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="015a4-116">The operation id. Read-only.</span></span> <span data-ttu-id="015a4-117">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="015a4-117">Server generated.</span></span>                                  |
| <span data-ttu-id="015a4-118">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="015a4-118">lastActionDateTime</span></span> | <span data-ttu-id="015a4-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="015a4-119">DateTimeOffset</span></span>  | <span data-ttu-id="015a4-120">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="015a4-120">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="015a4-121">状态</span><span class="sxs-lookup"><span data-stu-id="015a4-121">status</span></span>             | <span data-ttu-id="015a4-122">String</span><span class="sxs-lookup"><span data-stu-id="015a4-122">String</span></span>          | <span data-ttu-id="015a4-123">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="015a4-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="015a4-124">只读。</span><span class="sxs-lookup"><span data-stu-id="015a4-124">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="015a4-125">关系</span><span class="sxs-lookup"><span data-stu-id="015a4-125">Relationships</span></span>

<span data-ttu-id="015a4-126">无</span><span class="sxs-lookup"><span data-stu-id="015a4-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="015a4-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="015a4-127">JSON representation</span></span>

<span data-ttu-id="015a4-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="015a4-128">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="015a4-129">示例</span><span class="sxs-lookup"><span data-stu-id="015a4-129">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "status": "completed"
}
```

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/operation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
