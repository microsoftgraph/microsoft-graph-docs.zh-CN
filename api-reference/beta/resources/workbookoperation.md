---
title: workbookOperation 资源类型
description: 表示长时间运行的工作簿操作的状态。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: bd015045b01d0a7f886ecf0f5165a347d76dc061
ms.sourcegitcommit: b469176f49aacbd02cd06838cc7c8d36cf5bc768
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2020
ms.locfileid: "45165125"
---
# <a name="workbookoperation-resource-type"></a><span data-ttu-id="f4de5-103">workbookOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4de5-103">workbookOperation resource type</span></span>

<span data-ttu-id="f4de5-104">表示长时间运行的工作簿操作的状态。</span><span class="sxs-lookup"><span data-stu-id="f4de5-104">Represents the status of a long-running workbook operation.</span></span>

## <a name="methods"></a><span data-ttu-id="f4de5-105">方法</span><span class="sxs-lookup"><span data-stu-id="f4de5-105">Methods</span></span>

| <span data-ttu-id="f4de5-106">方法</span><span class="sxs-lookup"><span data-stu-id="f4de5-106">Method</span></span>       | <span data-ttu-id="f4de5-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="f4de5-107">Return Type</span></span> | <span data-ttu-id="f4de5-108">说明</span><span class="sxs-lookup"><span data-stu-id="f4de5-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f4de5-109">获取 workbookOperation</span><span class="sxs-lookup"><span data-stu-id="f4de5-109">Get workbookOperation</span></span>](../api/workbookoperation-get.md) | [<span data-ttu-id="f4de5-110">workbookOperation</span><span class="sxs-lookup"><span data-stu-id="f4de5-110">workbookOperation</span></span>](workbookoperation.md) | <span data-ttu-id="f4de5-111">检索**workbookOperation**对象的状态。</span><span class="sxs-lookup"><span data-stu-id="f4de5-111">Retrieve the status of a **workbookOperation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f4de5-112">属性</span><span class="sxs-lookup"><span data-stu-id="f4de5-112">Properties</span></span>

| <span data-ttu-id="f4de5-113">属性</span><span class="sxs-lookup"><span data-stu-id="f4de5-113">Property</span></span>     | <span data-ttu-id="f4de5-114">类型</span><span class="sxs-lookup"><span data-stu-id="f4de5-114">Type</span></span>        | <span data-ttu-id="f4de5-115">说明</span><span class="sxs-lookup"><span data-stu-id="f4de5-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f4de5-116">id</span><span class="sxs-lookup"><span data-stu-id="f4de5-116">id</span></span>|<span data-ttu-id="f4de5-117">String</span><span class="sxs-lookup"><span data-stu-id="f4de5-117">String</span></span>| <span data-ttu-id="f4de5-118">操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="f4de5-118">The operation id. Read-only.</span></span>|
|<span data-ttu-id="f4de5-119">状态</span><span class="sxs-lookup"><span data-stu-id="f4de5-119">status</span></span>|<span data-ttu-id="f4de5-120">String</span><span class="sxs-lookup"><span data-stu-id="f4de5-120">String</span></span>| <span data-ttu-id="f4de5-121">操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="f4de5-121">The current status of the operation.</span></span> <span data-ttu-id="f4de5-122">可取值为：`notStarted`、`running`、`succeeded`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="f4de5-122">Possible values are: `notStarted`, `running`, `succeeded`, `failed`.</span></span>|
|<span data-ttu-id="f4de5-123">error</span><span class="sxs-lookup"><span data-stu-id="f4de5-123">error</span></span>|[<span data-ttu-id="f4de5-124">workbookOperationError</span><span class="sxs-lookup"><span data-stu-id="f4de5-124">workbookOperationError</span></span>](workbookoperationerror.md)| <span data-ttu-id="f4de5-125">操作返回的错误。</span><span class="sxs-lookup"><span data-stu-id="f4de5-125">The error returned by the operation.</span></span>|
|<span data-ttu-id="f4de5-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="f4de5-126">resourceLocation</span></span>|<span data-ttu-id="f4de5-127">String</span><span class="sxs-lookup"><span data-stu-id="f4de5-127">String</span></span>| <span data-ttu-id="f4de5-128">结果的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="f4de5-128">The resource URI for the result.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4de5-129">关系</span><span class="sxs-lookup"><span data-stu-id="f4de5-129">Relationships</span></span>

<span data-ttu-id="f4de5-130">无。</span><span class="sxs-lookup"><span data-stu-id="f4de5-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4de5-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4de5-131">JSON representation</span></span>

<span data-ttu-id="f4de5-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4de5-132">The following is a JSON representation of the resource.</span></span>

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
