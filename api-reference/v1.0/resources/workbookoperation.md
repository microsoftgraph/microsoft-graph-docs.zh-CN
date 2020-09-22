---
title: workbookOperation 资源类型
description: 表示长时间运行的工作簿操作的状态。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9f186fe1c6c5e7ac917508ed75f6fb8488cbdc94
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015146"
---
# <a name="workbookoperation-resource-type"></a><span data-ttu-id="34326-103">workbookOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="34326-103">workbookOperation resource type</span></span>

<span data-ttu-id="34326-104">表示长时间运行的工作簿操作的状态。</span><span class="sxs-lookup"><span data-stu-id="34326-104">Represents the status of a long-running workbook operation.</span></span>


## <a name="methods"></a><span data-ttu-id="34326-105">方法</span><span class="sxs-lookup"><span data-stu-id="34326-105">Methods</span></span>

| <span data-ttu-id="34326-106">方法</span><span class="sxs-lookup"><span data-stu-id="34326-106">Method</span></span>       | <span data-ttu-id="34326-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="34326-107">Return Type</span></span> | <span data-ttu-id="34326-108">说明</span><span class="sxs-lookup"><span data-stu-id="34326-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="34326-109">获取 workbookOperation</span><span class="sxs-lookup"><span data-stu-id="34326-109">Get workbookOperation</span></span>](../api/workbookoperation-get.md) | [<span data-ttu-id="34326-110">workbookOperation</span><span class="sxs-lookup"><span data-stu-id="34326-110">workbookOperation</span></span>](workbookoperation.md) | <span data-ttu-id="34326-111">使用获取的操作 `{operation-id}` 。</span><span class="sxs-lookup"><span data-stu-id="34326-111">Get the operation with `{operation-id}`.</span></span> |


## <a name="properties"></a><span data-ttu-id="34326-112">属性</span><span class="sxs-lookup"><span data-stu-id="34326-112">Properties</span></span>

| <span data-ttu-id="34326-113">属性</span><span class="sxs-lookup"><span data-stu-id="34326-113">Property</span></span>     | <span data-ttu-id="34326-114">类型</span><span class="sxs-lookup"><span data-stu-id="34326-114">Type</span></span>        | <span data-ttu-id="34326-115">说明</span><span class="sxs-lookup"><span data-stu-id="34326-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="34326-116">状态</span><span class="sxs-lookup"><span data-stu-id="34326-116">status</span></span>|<span data-ttu-id="34326-117">String</span><span class="sxs-lookup"><span data-stu-id="34326-117">String</span></span>| <span data-ttu-id="34326-118">操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="34326-118">The current status of the operation.</span></span> <span data-ttu-id="34326-119">可取值为：`NotStarted`、`Running`、`Completed`、`Failed`。</span><span class="sxs-lookup"><span data-stu-id="34326-119">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="34326-120">id</span><span class="sxs-lookup"><span data-stu-id="34326-120">id</span></span>|<span data-ttu-id="34326-121">String</span><span class="sxs-lookup"><span data-stu-id="34326-121">String</span></span>| <span data-ttu-id="34326-122">操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="34326-122">The operation id. Read-only.</span></span>|
|<span data-ttu-id="34326-123">error</span><span class="sxs-lookup"><span data-stu-id="34326-123">error</span></span>|[<span data-ttu-id="34326-124">workbookOperationError</span><span class="sxs-lookup"><span data-stu-id="34326-124">workbookOperationError</span></span>](workbookoperationerror.md)| <span data-ttu-id="34326-125">操作返回的错误。</span><span class="sxs-lookup"><span data-stu-id="34326-125">The error returned by the operation.</span></span>|
|<span data-ttu-id="34326-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="34326-126">resourceLocation</span></span>|<span data-ttu-id="34326-127">String</span><span class="sxs-lookup"><span data-stu-id="34326-127">String</span></span>| <span data-ttu-id="34326-128">结果的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="34326-128">The resource URI for the result.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34326-129">关系</span><span class="sxs-lookup"><span data-stu-id="34326-129">Relationships</span></span>

<span data-ttu-id="34326-130">无</span><span class="sxs-lookup"><span data-stu-id="34326-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34326-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34326-131">JSON representation</span></span>

<span data-ttu-id="34326-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34326-132">The following is a JSON representation of the resource.</span></span>

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
