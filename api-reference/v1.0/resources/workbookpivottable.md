---
title: pivotTable 资源类型
description: 表示 Excel 数据透视表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5f6360ce1eacc313f1bcc8a9f59b44b216a87b84
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958738"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="5d820-103">pivotTable 资源类型</span><span class="sxs-lookup"><span data-stu-id="5d820-103">pivotTable resource type</span></span>

<span data-ttu-id="5d820-104">表示 Excel 数据透视表。</span><span class="sxs-lookup"><span data-stu-id="5d820-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="5d820-105">方法</span><span class="sxs-lookup"><span data-stu-id="5d820-105">Methods</span></span>

| <span data-ttu-id="5d820-106">方法</span><span class="sxs-lookup"><span data-stu-id="5d820-106">Method</span></span>           | <span data-ttu-id="5d820-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="5d820-107">Return Type</span></span>    |<span data-ttu-id="5d820-108">说明</span><span class="sxs-lookup"><span data-stu-id="5d820-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5d820-109">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="5d820-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="5d820-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="5d820-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="5d820-111">读取 workbookPivotTable 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5d820-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="5d820-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="5d820-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="5d820-113">无</span><span class="sxs-lookup"><span data-stu-id="5d820-113">None</span></span>|<span data-ttu-id="5d820-114">刷新数据透视表。</span><span class="sxs-lookup"><span data-stu-id="5d820-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="5d820-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="5d820-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="5d820-116">无</span><span class="sxs-lookup"><span data-stu-id="5d820-116">None</span></span>|<span data-ttu-id="5d820-p101">刷新给定工作表内的所有表。请注意，只能对数据透视表集合执行此操作。</span><span class="sxs-lookup"><span data-stu-id="5d820-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="5d820-119">属性</span><span class="sxs-lookup"><span data-stu-id="5d820-119">Properties</span></span>
| <span data-ttu-id="5d820-120">属性</span><span class="sxs-lookup"><span data-stu-id="5d820-120">Property</span></span>     | <span data-ttu-id="5d820-121">类型</span><span class="sxs-lookup"><span data-stu-id="5d820-121">Type</span></span>   |<span data-ttu-id="5d820-122">说明</span><span class="sxs-lookup"><span data-stu-id="5d820-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d820-123">id</span><span class="sxs-lookup"><span data-stu-id="5d820-123">id</span></span>|<span data-ttu-id="5d820-124">String</span><span class="sxs-lookup"><span data-stu-id="5d820-124">String</span></span>| <span data-ttu-id="5d820-p102">数据透视表的 ID。 只读。</span><span class="sxs-lookup"><span data-stu-id="5d820-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="5d820-127">name</span><span class="sxs-lookup"><span data-stu-id="5d820-127">name</span></span>|<span data-ttu-id="5d820-128">String</span><span class="sxs-lookup"><span data-stu-id="5d820-128">String</span></span>|<span data-ttu-id="5d820-129">数据透视表对象的名称。</span><span class="sxs-lookup"><span data-stu-id="5d820-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="5d820-130">关系</span><span class="sxs-lookup"><span data-stu-id="5d820-130">Relationships</span></span>
| <span data-ttu-id="5d820-131">关系</span><span class="sxs-lookup"><span data-stu-id="5d820-131">Relationship</span></span> | <span data-ttu-id="5d820-132">类型</span><span class="sxs-lookup"><span data-stu-id="5d820-132">Type</span></span>   |<span data-ttu-id="5d820-133">说明</span><span class="sxs-lookup"><span data-stu-id="5d820-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d820-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="5d820-134">worksheet</span></span>|[<span data-ttu-id="5d820-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="5d820-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="5d820-p103">包含当前 PivotTable 对象的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="5d820-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="5d820-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5d820-138">JSON representation</span></span>
<span data-ttu-id="5d820-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d820-139">Here is a JSON representation of the resource.</span></span>

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
