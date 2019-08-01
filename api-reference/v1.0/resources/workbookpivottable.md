---
title: pivotTable 资源类型
description: 表示 Excel 数据透视表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c5b841495b19a81967ba056f702a88c4cbe74efc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033360"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="77d6c-103">pivotTable 资源类型</span><span class="sxs-lookup"><span data-stu-id="77d6c-103">pivotTable resource type</span></span>

<span data-ttu-id="77d6c-104">表示 Excel 数据透视表。</span><span class="sxs-lookup"><span data-stu-id="77d6c-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="77d6c-105">方法</span><span class="sxs-lookup"><span data-stu-id="77d6c-105">Methods</span></span>

| <span data-ttu-id="77d6c-106">方法</span><span class="sxs-lookup"><span data-stu-id="77d6c-106">Method</span></span>           | <span data-ttu-id="77d6c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="77d6c-107">Return Type</span></span>    |<span data-ttu-id="77d6c-108">说明</span><span class="sxs-lookup"><span data-stu-id="77d6c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77d6c-109">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="77d6c-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="77d6c-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="77d6c-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="77d6c-111">读取 workbookPivotTable 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77d6c-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="77d6c-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="77d6c-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="77d6c-113">无</span><span class="sxs-lookup"><span data-stu-id="77d6c-113">None</span></span>|<span data-ttu-id="77d6c-114">刷新数据透视表。</span><span class="sxs-lookup"><span data-stu-id="77d6c-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="77d6c-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="77d6c-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="77d6c-116">无</span><span class="sxs-lookup"><span data-stu-id="77d6c-116">None</span></span>|<span data-ttu-id="77d6c-p101">刷新给定工作表内的所有表。请注意，只能对数据透视表集合执行此操作。</span><span class="sxs-lookup"><span data-stu-id="77d6c-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="77d6c-119">属性</span><span class="sxs-lookup"><span data-stu-id="77d6c-119">Properties</span></span>
| <span data-ttu-id="77d6c-120">属性</span><span class="sxs-lookup"><span data-stu-id="77d6c-120">Property</span></span>     | <span data-ttu-id="77d6c-121">类型</span><span class="sxs-lookup"><span data-stu-id="77d6c-121">Type</span></span>   |<span data-ttu-id="77d6c-122">说明</span><span class="sxs-lookup"><span data-stu-id="77d6c-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77d6c-123">id</span><span class="sxs-lookup"><span data-stu-id="77d6c-123">id</span></span>|<span data-ttu-id="77d6c-124">String</span><span class="sxs-lookup"><span data-stu-id="77d6c-124">String</span></span>| <span data-ttu-id="77d6c-p102">数据透视表的 ID。 只读。</span><span class="sxs-lookup"><span data-stu-id="77d6c-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="77d6c-127">name</span><span class="sxs-lookup"><span data-stu-id="77d6c-127">name</span></span>|<span data-ttu-id="77d6c-128">String</span><span class="sxs-lookup"><span data-stu-id="77d6c-128">String</span></span>|<span data-ttu-id="77d6c-129">数据透视表对象的名称。</span><span class="sxs-lookup"><span data-stu-id="77d6c-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="77d6c-130">关系</span><span class="sxs-lookup"><span data-stu-id="77d6c-130">Relationships</span></span>
| <span data-ttu-id="77d6c-131">关系</span><span class="sxs-lookup"><span data-stu-id="77d6c-131">Relationship</span></span> | <span data-ttu-id="77d6c-132">类型</span><span class="sxs-lookup"><span data-stu-id="77d6c-132">Type</span></span>   |<span data-ttu-id="77d6c-133">说明</span><span class="sxs-lookup"><span data-stu-id="77d6c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77d6c-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="77d6c-134">worksheet</span></span>|[<span data-ttu-id="77d6c-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="77d6c-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="77d6c-136">包含当前 PivotTable 对象的工作表。</span><span class="sxs-lookup"><span data-stu-id="77d6c-136">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="77d6c-137">只读。</span><span class="sxs-lookup"><span data-stu-id="77d6c-137">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="77d6c-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77d6c-138">JSON representation</span></span>
<span data-ttu-id="77d6c-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77d6c-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
