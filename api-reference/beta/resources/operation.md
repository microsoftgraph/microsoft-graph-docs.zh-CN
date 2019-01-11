---
title: 操作资源类型
description: 长时间运行操作的状态。
localization_priority: Normal
ms.openlocfilehash: 760aeedb67b987fc22a5eef969e2214f6dfd05b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830343"
---
# <a name="operation-resource-type"></a><span data-ttu-id="b8111-103">操作资源类型</span><span class="sxs-lookup"><span data-stu-id="b8111-103">operation resource type</span></span>

> <span data-ttu-id="b8111-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b8111-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8111-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b8111-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8111-106">长时间运行操作的状态。</span><span class="sxs-lookup"><span data-stu-id="b8111-106">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="b8111-107">方法</span><span class="sxs-lookup"><span data-stu-id="b8111-107">Methods</span></span>

<span data-ttu-id="b8111-108">无</span><span class="sxs-lookup"><span data-stu-id="b8111-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="b8111-109">属性</span><span class="sxs-lookup"><span data-stu-id="b8111-109">Properties</span></span>

| <span data-ttu-id="b8111-110">属性</span><span class="sxs-lookup"><span data-stu-id="b8111-110">Property</span></span>           | <span data-ttu-id="b8111-111">类型</span><span class="sxs-lookup"><span data-stu-id="b8111-111">Type</span></span>            | <span data-ttu-id="b8111-112">说明</span><span class="sxs-lookup"><span data-stu-id="b8111-112">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="b8111-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8111-113">createdDateTime</span></span>    | <span data-ttu-id="b8111-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8111-114">DateTimeOffset</span></span>  | <span data-ttu-id="b8111-115">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="b8111-115">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="b8111-116">id</span><span class="sxs-lookup"><span data-stu-id="b8111-116">id</span></span>                 | <span data-ttu-id="b8111-117">字符串</span><span class="sxs-lookup"><span data-stu-id="b8111-117">String</span></span>          | <span data-ttu-id="b8111-118">操作 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="b8111-118">The operation id. Read-only.</span></span> <span data-ttu-id="b8111-119">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="b8111-119">Server generated.</span></span>                                  |
| <span data-ttu-id="b8111-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="b8111-120">lastActionDateTime</span></span> | <span data-ttu-id="b8111-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8111-121">DateTimeOffset</span></span>  | <span data-ttu-id="b8111-122">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="b8111-122">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="b8111-123">status</span><span class="sxs-lookup"><span data-stu-id="b8111-123">status</span></span>             | <span data-ttu-id="b8111-124">String</span><span class="sxs-lookup"><span data-stu-id="b8111-124">String</span></span>          | <span data-ttu-id="b8111-125">可取值为 `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b8111-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="b8111-126">只读。</span><span class="sxs-lookup"><span data-stu-id="b8111-126">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b8111-127">Relationships</span><span class="sxs-lookup"><span data-stu-id="b8111-127">Relationships</span></span>

<span data-ttu-id="b8111-128">无</span><span class="sxs-lookup"><span data-stu-id="b8111-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8111-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8111-129">JSON representation</span></span>

<span data-ttu-id="b8111-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8111-130">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="b8111-131">示例</span><span class="sxs-lookup"><span data-stu-id="b8111-131">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
