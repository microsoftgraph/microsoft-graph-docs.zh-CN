---
title: printOperation 资源类型
description: 表示长时间运行的通用打印操作。 操作类型（如 printerCreateOperation）的基类。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 970ac3dd06e5af1478600166ffdd4c84815aa5b5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048720"
---
# <a name="printoperation-resource-type"></a><span data-ttu-id="27177-104">printOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="27177-104">printOperation resource type</span></span>

<span data-ttu-id="27177-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27177-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27177-106">表示长时间运行的通用打印操作。</span><span class="sxs-lookup"><span data-stu-id="27177-106">Represents a long-running Universal Print operation.</span></span> <span data-ttu-id="27177-107">操作类型（如 [printerCreateOperation](printercreateoperation.md)）的基类。</span><span class="sxs-lookup"><span data-stu-id="27177-107">Base class for operation types such as [printerCreateOperation](printercreateoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="27177-108">方法</span><span class="sxs-lookup"><span data-stu-id="27177-108">Methods</span></span>

| <span data-ttu-id="27177-109">方法</span><span class="sxs-lookup"><span data-stu-id="27177-109">Method</span></span>       | <span data-ttu-id="27177-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="27177-110">Return Type</span></span> | <span data-ttu-id="27177-111">说明</span><span class="sxs-lookup"><span data-stu-id="27177-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="27177-112">Get 操作</span><span class="sxs-lookup"><span data-stu-id="27177-112">Get operation</span></span>](../api/printoperation-get.md) | [<span data-ttu-id="27177-113">printOperation</span><span class="sxs-lookup"><span data-stu-id="27177-113">printOperation</span></span>](printoperation.md) | <span data-ttu-id="27177-114">在当前用户或应用程序的租户内检索长时间运行的操作。</span><span class="sxs-lookup"><span data-stu-id="27177-114">Retrieve a long-running operation within current user or app's tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="27177-115">属性</span><span class="sxs-lookup"><span data-stu-id="27177-115">Properties</span></span>
| <span data-ttu-id="27177-116">属性</span><span class="sxs-lookup"><span data-stu-id="27177-116">Property</span></span>     | <span data-ttu-id="27177-117">类型</span><span class="sxs-lookup"><span data-stu-id="27177-117">Type</span></span>        | <span data-ttu-id="27177-118">说明</span><span class="sxs-lookup"><span data-stu-id="27177-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="27177-119">id</span><span class="sxs-lookup"><span data-stu-id="27177-119">id</span></span>|<span data-ttu-id="27177-120">String</span><span class="sxs-lookup"><span data-stu-id="27177-120">String</span></span>|<span data-ttu-id="27177-121">操作的标识符。</span><span class="sxs-lookup"><span data-stu-id="27177-121">The operation's identifier.</span></span> <span data-ttu-id="27177-122">只读。</span><span class="sxs-lookup"><span data-stu-id="27177-122">Read-only.</span></span>|
|<span data-ttu-id="27177-123">状态</span><span class="sxs-lookup"><span data-stu-id="27177-123">status</span></span>|[<span data-ttu-id="27177-124">printOperationStatus</span><span class="sxs-lookup"><span data-stu-id="27177-124">printOperationStatus</span></span>](printoperationstatus.md)|<span data-ttu-id="27177-125">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="27177-125">The status of the operation.</span></span> <span data-ttu-id="27177-126">只读。</span><span class="sxs-lookup"><span data-stu-id="27177-126">Read-only.</span></span>|
|<span data-ttu-id="27177-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27177-127">createdDateTime</span></span>|<span data-ttu-id="27177-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27177-128">DateTimeOffset</span></span>|<span data-ttu-id="27177-129">创建操作时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="27177-129">The DateTimeOffset when the operation was created.</span></span> <span data-ttu-id="27177-130">只读。</span><span class="sxs-lookup"><span data-stu-id="27177-130">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27177-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="27177-131">JSON representation</span></span>

<span data-ttu-id="27177-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27177-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printOperation",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
    "id": "String (identifier)",
    "status": {"@odata.type": "microsoft.graph.printOperationStatus"},
    "createdDateTime": "2020-06-15T19:54:14.853Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


