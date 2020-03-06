---
title: pivotTable 资源类型
description: 表示 Excel 数据透视表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b3ec3c9237e246b2af10a867155bc7b6d360a67f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533376"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="e05e3-103">pivotTable 资源类型</span><span class="sxs-lookup"><span data-stu-id="e05e3-103">pivotTable resource type</span></span>

<span data-ttu-id="e05e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e05e3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e05e3-105">表示 Excel 数据透视表。</span><span class="sxs-lookup"><span data-stu-id="e05e3-105">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="e05e3-106">Methods</span><span class="sxs-lookup"><span data-stu-id="e05e3-106">Methods</span></span>

| <span data-ttu-id="e05e3-107">方法</span><span class="sxs-lookup"><span data-stu-id="e05e3-107">Method</span></span>           | <span data-ttu-id="e05e3-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e05e3-108">Return Type</span></span>    |<span data-ttu-id="e05e3-109">说明</span><span class="sxs-lookup"><span data-stu-id="e05e3-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e05e3-110">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="e05e3-110">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="e05e3-111">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="e05e3-111">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="e05e3-112">读取 workbookPivotTable 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e05e3-112">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="e05e3-113">Refresh</span><span class="sxs-lookup"><span data-stu-id="e05e3-113">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="e05e3-114">无</span><span class="sxs-lookup"><span data-stu-id="e05e3-114">None</span></span>|<span data-ttu-id="e05e3-115">刷新数据透视表。</span><span class="sxs-lookup"><span data-stu-id="e05e3-115">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="e05e3-116">Refreshall</span><span class="sxs-lookup"><span data-stu-id="e05e3-116">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="e05e3-117">无</span><span class="sxs-lookup"><span data-stu-id="e05e3-117">None</span></span>|<span data-ttu-id="e05e3-p101">刷新给定工作表内的所有表。请注意，只能对数据透视表集合执行此操作。</span><span class="sxs-lookup"><span data-stu-id="e05e3-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="e05e3-120">属性</span><span class="sxs-lookup"><span data-stu-id="e05e3-120">Properties</span></span>
| <span data-ttu-id="e05e3-121">属性</span><span class="sxs-lookup"><span data-stu-id="e05e3-121">Property</span></span>     | <span data-ttu-id="e05e3-122">类型</span><span class="sxs-lookup"><span data-stu-id="e05e3-122">Type</span></span>   |<span data-ttu-id="e05e3-123">说明</span><span class="sxs-lookup"><span data-stu-id="e05e3-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e05e3-124">id</span><span class="sxs-lookup"><span data-stu-id="e05e3-124">id</span></span>|<span data-ttu-id="e05e3-125">String</span><span class="sxs-lookup"><span data-stu-id="e05e3-125">String</span></span>| <span data-ttu-id="e05e3-p102">数据透视表的 ID。 只读。</span><span class="sxs-lookup"><span data-stu-id="e05e3-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="e05e3-128">name</span><span class="sxs-lookup"><span data-stu-id="e05e3-128">name</span></span>|<span data-ttu-id="e05e3-129">字符串</span><span class="sxs-lookup"><span data-stu-id="e05e3-129">String</span></span>|<span data-ttu-id="e05e3-130">数据透视表对象的名称。</span><span class="sxs-lookup"><span data-stu-id="e05e3-130">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="e05e3-131">关系</span><span class="sxs-lookup"><span data-stu-id="e05e3-131">Relationships</span></span>
| <span data-ttu-id="e05e3-132">关系</span><span class="sxs-lookup"><span data-stu-id="e05e3-132">Relationship</span></span> | <span data-ttu-id="e05e3-133">类型</span><span class="sxs-lookup"><span data-stu-id="e05e3-133">Type</span></span>   |<span data-ttu-id="e05e3-134">说明</span><span class="sxs-lookup"><span data-stu-id="e05e3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e05e3-135">worksheet</span><span class="sxs-lookup"><span data-stu-id="e05e3-135">worksheet</span></span>|[<span data-ttu-id="e05e3-136">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="e05e3-136">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="e05e3-137">包含当前 PivotTable 对象的工作表。</span><span class="sxs-lookup"><span data-stu-id="e05e3-137">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="e05e3-138">只读。</span><span class="sxs-lookup"><span data-stu-id="e05e3-138">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="e05e3-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e05e3-139">JSON representation</span></span>
<span data-ttu-id="e05e3-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e05e3-140">Here is a JSON representation of the resource.</span></span>

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
