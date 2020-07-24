---
title: workbookOperation 资源类型
description: 表示长时间运行的工作簿操作的状态。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4fa98cdfdfc013386f7d615c54c832d27c5f826e
ms.sourcegitcommit: 233ac43db0eb5edd46fe944a5515d7dd9abb1298
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2020
ms.locfileid: "45408140"
---
# <a name="workbookoperation-resource-type"></a><span data-ttu-id="5af7f-103">workbookOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="5af7f-103">workbookOperation resource type</span></span>

<span data-ttu-id="5af7f-104">表示长时间运行的工作簿操作的状态。</span><span class="sxs-lookup"><span data-stu-id="5af7f-104">Represents the status of a long-running workbook operation.</span></span>


## <a name="methods"></a><span data-ttu-id="5af7f-105">方法</span><span class="sxs-lookup"><span data-stu-id="5af7f-105">Methods</span></span>

| <span data-ttu-id="5af7f-106">方法</span><span class="sxs-lookup"><span data-stu-id="5af7f-106">Method</span></span>       | <span data-ttu-id="5af7f-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="5af7f-107">Return Type</span></span> | <span data-ttu-id="5af7f-108">说明</span><span class="sxs-lookup"><span data-stu-id="5af7f-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5af7f-109">获取 workbookOperation</span><span class="sxs-lookup"><span data-stu-id="5af7f-109">Get workbookOperation</span></span>](../api/workbookoperation-get.md) | [<span data-ttu-id="5af7f-110">workbookOperation</span><span class="sxs-lookup"><span data-stu-id="5af7f-110">workbookOperation</span></span>](workbookoperation.md) | <span data-ttu-id="5af7f-111">使用获取的操作 `{operation-id}` 。</span><span class="sxs-lookup"><span data-stu-id="5af7f-111">Get the operation with `{operation-id}`.</span></span> |


## <a name="properties"></a><span data-ttu-id="5af7f-112">属性</span><span class="sxs-lookup"><span data-stu-id="5af7f-112">Properties</span></span>

| <span data-ttu-id="5af7f-113">属性</span><span class="sxs-lookup"><span data-stu-id="5af7f-113">Property</span></span>     | <span data-ttu-id="5af7f-114">类型</span><span class="sxs-lookup"><span data-stu-id="5af7f-114">Type</span></span>        | <span data-ttu-id="5af7f-115">说明</span><span class="sxs-lookup"><span data-stu-id="5af7f-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5af7f-116">状态</span><span class="sxs-lookup"><span data-stu-id="5af7f-116">status</span></span>|<span data-ttu-id="5af7f-117">字符串</span><span class="sxs-lookup"><span data-stu-id="5af7f-117">String</span></span>| <span data-ttu-id="5af7f-118">操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="5af7f-118">The current status of the operation.</span></span> <span data-ttu-id="5af7f-119">可取值为：`NotStarted`、`Running`、`Completed`、`Failed`。</span><span class="sxs-lookup"><span data-stu-id="5af7f-119">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="5af7f-120">id</span><span class="sxs-lookup"><span data-stu-id="5af7f-120">id</span></span>|<span data-ttu-id="5af7f-121">String</span><span class="sxs-lookup"><span data-stu-id="5af7f-121">String</span></span>| <span data-ttu-id="5af7f-122">操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="5af7f-122">The operation id. Read-only.</span></span>|
|<span data-ttu-id="5af7f-123">error</span><span class="sxs-lookup"><span data-stu-id="5af7f-123">error</span></span>|[<span data-ttu-id="5af7f-124">workbookOperationError</span><span class="sxs-lookup"><span data-stu-id="5af7f-124">workbookOperationError</span></span>](workbookoperationerror.md)| <span data-ttu-id="5af7f-125">操作返回的错误。</span><span class="sxs-lookup"><span data-stu-id="5af7f-125">The error returned by the operation.</span></span>|
|<span data-ttu-id="5af7f-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="5af7f-126">resourceLocation</span></span>|<span data-ttu-id="5af7f-127">字符串</span><span class="sxs-lookup"><span data-stu-id="5af7f-127">String</span></span>| <span data-ttu-id="5af7f-128">结果的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="5af7f-128">The resource URI for the result.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5af7f-129">关系</span><span class="sxs-lookup"><span data-stu-id="5af7f-129">Relationships</span></span>

<span data-ttu-id="5af7f-130">无</span><span class="sxs-lookup"><span data-stu-id="5af7f-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5af7f-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5af7f-131">JSON representation</span></span>

<span data-ttu-id="5af7f-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5af7f-132">The following is a JSON representation of the resource.</span></span>

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
  "resourceLocation": "String",
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