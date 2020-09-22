---
title: 操作资源类型
description: 长时间运行的操作的状态。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: billbliss
ms.openlocfilehash: f57b9f14603fdeae539e872d87b5af2645cedef0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998509"
---
# <a name="operation-resource-type"></a><span data-ttu-id="02bb0-103">操作资源类型</span><span class="sxs-lookup"><span data-stu-id="02bb0-103">operation resource type</span></span>

<span data-ttu-id="02bb0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02bb0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02bb0-105">长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="02bb0-105">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="02bb0-106">方法</span><span class="sxs-lookup"><span data-stu-id="02bb0-106">Methods</span></span>

<span data-ttu-id="02bb0-107">无</span><span class="sxs-lookup"><span data-stu-id="02bb0-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="02bb0-108">属性</span><span class="sxs-lookup"><span data-stu-id="02bb0-108">Properties</span></span>

| <span data-ttu-id="02bb0-109">属性</span><span class="sxs-lookup"><span data-stu-id="02bb0-109">Property</span></span>           | <span data-ttu-id="02bb0-110">类型</span><span class="sxs-lookup"><span data-stu-id="02bb0-110">Type</span></span>            | <span data-ttu-id="02bb0-111">说明</span><span class="sxs-lookup"><span data-stu-id="02bb0-111">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="02bb0-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02bb0-112">createdDateTime</span></span>    | <span data-ttu-id="02bb0-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02bb0-113">DateTimeOffset</span></span>  | <span data-ttu-id="02bb0-114">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="02bb0-114">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="02bb0-115">id</span><span class="sxs-lookup"><span data-stu-id="02bb0-115">id</span></span>                 | <span data-ttu-id="02bb0-116">String</span><span class="sxs-lookup"><span data-stu-id="02bb0-116">String</span></span>          | <span data-ttu-id="02bb0-117">操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="02bb0-117">The operation id. Read-only.</span></span> <span data-ttu-id="02bb0-118">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="02bb0-118">Server generated.</span></span>                                  |
| <span data-ttu-id="02bb0-119">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="02bb0-119">lastActionDateTime</span></span> | <span data-ttu-id="02bb0-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02bb0-120">DateTimeOffset</span></span>  | <span data-ttu-id="02bb0-121">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="02bb0-121">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="02bb0-122">状态</span><span class="sxs-lookup"><span data-stu-id="02bb0-122">status</span></span>             | <span data-ttu-id="02bb0-123">String</span><span class="sxs-lookup"><span data-stu-id="02bb0-123">String</span></span>          | <span data-ttu-id="02bb0-124">可能的值是：`notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="02bb0-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="02bb0-125">只读。</span><span class="sxs-lookup"><span data-stu-id="02bb0-125">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="02bb0-126">关系</span><span class="sxs-lookup"><span data-stu-id="02bb0-126">Relationships</span></span>

<span data-ttu-id="02bb0-127">无</span><span class="sxs-lookup"><span data-stu-id="02bb0-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02bb0-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02bb0-128">JSON representation</span></span>

<span data-ttu-id="02bb0-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02bb0-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="02bb0-130">示例</span><span class="sxs-lookup"><span data-stu-id="02bb0-130">Example</span></span>

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
  "suppressions": []
}
-->


