---
title: workbookOperation 资源类型
description: 表示长时间运行的工作簿操作的状态。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 957f94087fa8c11cf3a5cc794bf194e21bbba346
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075376"
---
# <a name="workbookoperation-resource-type"></a><span data-ttu-id="c0b5a-103">workbookOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="c0b5a-103">workbookOperation resource type</span></span>

<span data-ttu-id="c0b5a-104">表示长时间运行的工作簿操作的状态。</span><span class="sxs-lookup"><span data-stu-id="c0b5a-104">Represents the status of a long-running workbook operation.</span></span>

## <a name="methods"></a><span data-ttu-id="c0b5a-105">方法</span><span class="sxs-lookup"><span data-stu-id="c0b5a-105">Methods</span></span>

| <span data-ttu-id="c0b5a-106">方法</span><span class="sxs-lookup"><span data-stu-id="c0b5a-106">Method</span></span>       | <span data-ttu-id="c0b5a-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="c0b5a-107">Return Type</span></span> | <span data-ttu-id="c0b5a-108">说明</span><span class="sxs-lookup"><span data-stu-id="c0b5a-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c0b5a-109">获取 workbookOperation</span><span class="sxs-lookup"><span data-stu-id="c0b5a-109">Get workbookOperation</span></span>](../api/workbookoperation-get.md) | [<span data-ttu-id="c0b5a-110">workbookOperation</span><span class="sxs-lookup"><span data-stu-id="c0b5a-110">workbookOperation</span></span>](workbookoperation.md) | <span data-ttu-id="c0b5a-111">检索 **workbookOperation** 对象的状态。</span><span class="sxs-lookup"><span data-stu-id="c0b5a-111">Retrieve the status of a **workbookOperation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c0b5a-112">属性</span><span class="sxs-lookup"><span data-stu-id="c0b5a-112">Properties</span></span>

| <span data-ttu-id="c0b5a-113">属性</span><span class="sxs-lookup"><span data-stu-id="c0b5a-113">Property</span></span>     | <span data-ttu-id="c0b5a-114">类型</span><span class="sxs-lookup"><span data-stu-id="c0b5a-114">Type</span></span>        | <span data-ttu-id="c0b5a-115">说明</span><span class="sxs-lookup"><span data-stu-id="c0b5a-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c0b5a-116">id</span><span class="sxs-lookup"><span data-stu-id="c0b5a-116">id</span></span>|<span data-ttu-id="c0b5a-117">String</span><span class="sxs-lookup"><span data-stu-id="c0b5a-117">String</span></span>| <span data-ttu-id="c0b5a-118">操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="c0b5a-118">The operation id. Read-only.</span></span>|
|<span data-ttu-id="c0b5a-119">状态</span><span class="sxs-lookup"><span data-stu-id="c0b5a-119">status</span></span>|<span data-ttu-id="c0b5a-120">String</span><span class="sxs-lookup"><span data-stu-id="c0b5a-120">String</span></span>| <span data-ttu-id="c0b5a-121">操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="c0b5a-121">The current status of the operation.</span></span> <span data-ttu-id="c0b5a-122">可取值为：`notStarted`、`running`、`succeeded`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="c0b5a-122">Possible values are: `notStarted`, `running`, `succeeded`, `failed`.</span></span>|
|<span data-ttu-id="c0b5a-123">error</span><span class="sxs-lookup"><span data-stu-id="c0b5a-123">error</span></span>|[<span data-ttu-id="c0b5a-124">workbookOperationError</span><span class="sxs-lookup"><span data-stu-id="c0b5a-124">workbookOperationError</span></span>](workbookoperationerror.md)| <span data-ttu-id="c0b5a-125">操作返回的错误。</span><span class="sxs-lookup"><span data-stu-id="c0b5a-125">The error returned by the operation.</span></span>|
|<span data-ttu-id="c0b5a-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="c0b5a-126">resourceLocation</span></span>|<span data-ttu-id="c0b5a-127">String</span><span class="sxs-lookup"><span data-stu-id="c0b5a-127">String</span></span>| <span data-ttu-id="c0b5a-128">结果的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="c0b5a-128">The resource URI for the result.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0b5a-129">关系</span><span class="sxs-lookup"><span data-stu-id="c0b5a-129">Relationships</span></span>

<span data-ttu-id="c0b5a-130">无。</span><span class="sxs-lookup"><span data-stu-id="c0b5a-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0b5a-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0b5a-131">JSON representation</span></span>

<span data-ttu-id="c0b5a-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0b5a-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperation",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "status": {"@odata.type": "microsoft.graph.workbookOperationStatus"},
  "error": {"@odata.type": "microsoft.graph.workbookOperationError"},
  "resourceLocation": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


