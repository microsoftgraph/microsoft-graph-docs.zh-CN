---
title: pivotTable 资源类型
description: 表示 Excel 数据透视表。
author: lumine2008
ms.openlocfilehash: 68075aebeac9c0846e48739daf65e5bf97e4d6f5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334109"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="dea0e-103">pivotTable 资源类型</span><span class="sxs-lookup"><span data-stu-id="dea0e-103">pivotTable resource type</span></span>

<span data-ttu-id="dea0e-104">表示 Excel 数据透视表。</span><span class="sxs-lookup"><span data-stu-id="dea0e-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="dea0e-105">方法</span><span class="sxs-lookup"><span data-stu-id="dea0e-105">Methods</span></span>

| <span data-ttu-id="dea0e-106">方法</span><span class="sxs-lookup"><span data-stu-id="dea0e-106">Method</span></span>           | <span data-ttu-id="dea0e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="dea0e-107">Return Type</span></span>    |<span data-ttu-id="dea0e-108">说明</span><span class="sxs-lookup"><span data-stu-id="dea0e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dea0e-109">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="dea0e-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="dea0e-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="dea0e-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="dea0e-111">读取 workbookPivotTable 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dea0e-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="dea0e-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="dea0e-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="dea0e-113">无</span><span class="sxs-lookup"><span data-stu-id="dea0e-113">None</span></span>|<span data-ttu-id="dea0e-114">刷新数据透视表。</span><span class="sxs-lookup"><span data-stu-id="dea0e-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="dea0e-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="dea0e-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="dea0e-116">无</span><span class="sxs-lookup"><span data-stu-id="dea0e-116">None</span></span>|<span data-ttu-id="dea0e-p101">刷新给定工作表内的所有表。请注意，只能对数据透视表集合执行此操作。</span><span class="sxs-lookup"><span data-stu-id="dea0e-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="dea0e-119">属性</span><span class="sxs-lookup"><span data-stu-id="dea0e-119">Properties</span></span>
| <span data-ttu-id="dea0e-120">属性</span><span class="sxs-lookup"><span data-stu-id="dea0e-120">Property</span></span>     | <span data-ttu-id="dea0e-121">类型</span><span class="sxs-lookup"><span data-stu-id="dea0e-121">Type</span></span>   |<span data-ttu-id="dea0e-122">说明</span><span class="sxs-lookup"><span data-stu-id="dea0e-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dea0e-123">id</span><span class="sxs-lookup"><span data-stu-id="dea0e-123">id</span></span>|<span data-ttu-id="dea0e-124">String</span><span class="sxs-lookup"><span data-stu-id="dea0e-124">String</span></span>| <span data-ttu-id="dea0e-p102">数据透视表的 ID。 只读。</span><span class="sxs-lookup"><span data-stu-id="dea0e-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="dea0e-127">name</span><span class="sxs-lookup"><span data-stu-id="dea0e-127">name</span></span>|<span data-ttu-id="dea0e-128">String</span><span class="sxs-lookup"><span data-stu-id="dea0e-128">String</span></span>|<span data-ttu-id="dea0e-129">数据透视表对象的名称。</span><span class="sxs-lookup"><span data-stu-id="dea0e-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="dea0e-130">关系</span><span class="sxs-lookup"><span data-stu-id="dea0e-130">Relationships</span></span>
| <span data-ttu-id="dea0e-131">关系</span><span class="sxs-lookup"><span data-stu-id="dea0e-131">Relationship</span></span> | <span data-ttu-id="dea0e-132">类型</span><span class="sxs-lookup"><span data-stu-id="dea0e-132">Type</span></span>   |<span data-ttu-id="dea0e-133">说明</span><span class="sxs-lookup"><span data-stu-id="dea0e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dea0e-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="dea0e-134">worksheet</span></span>|[<span data-ttu-id="dea0e-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="dea0e-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="dea0e-p103">包含当前 PivotTable 对象的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="dea0e-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="dea0e-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dea0e-138">JSON representation</span></span>
<span data-ttu-id="dea0e-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dea0e-139">Here is a JSON representation of the resource.</span></span>

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
