---
title: pivotTable 资源类型
description: 表示 Excel 数据透视表。
ms.openlocfilehash: b4ddd0c1bb9e4ee13aaf3d1b4472c4e750e3a755
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008288"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="37186-103">pivotTable 资源类型</span><span class="sxs-lookup"><span data-stu-id="37186-103">pivotTable resource type</span></span>

<span data-ttu-id="37186-104">表示 Excel 数据透视表。</span><span class="sxs-lookup"><span data-stu-id="37186-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="37186-105">方法</span><span class="sxs-lookup"><span data-stu-id="37186-105">Methods</span></span>

| <span data-ttu-id="37186-106">方法</span><span class="sxs-lookup"><span data-stu-id="37186-106">Method</span></span>           | <span data-ttu-id="37186-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="37186-107">Return Type</span></span>    |<span data-ttu-id="37186-108">说明</span><span class="sxs-lookup"><span data-stu-id="37186-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="37186-109">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="37186-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="37186-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="37186-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="37186-111">读取 workbookPivotTable 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="37186-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="37186-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="37186-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="37186-113">无</span><span class="sxs-lookup"><span data-stu-id="37186-113">None</span></span>|<span data-ttu-id="37186-114">刷新数据透视表。</span><span class="sxs-lookup"><span data-stu-id="37186-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="37186-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="37186-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="37186-116">无</span><span class="sxs-lookup"><span data-stu-id="37186-116">None</span></span>|<span data-ttu-id="37186-p101">刷新给定工作表内的所有表。请注意，只能对数据透视表集合执行此操作。</span><span class="sxs-lookup"><span data-stu-id="37186-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="37186-119">属性</span><span class="sxs-lookup"><span data-stu-id="37186-119">Properties</span></span>
| <span data-ttu-id="37186-120">属性</span><span class="sxs-lookup"><span data-stu-id="37186-120">Property</span></span>     | <span data-ttu-id="37186-121">类型</span><span class="sxs-lookup"><span data-stu-id="37186-121">Type</span></span>   |<span data-ttu-id="37186-122">说明</span><span class="sxs-lookup"><span data-stu-id="37186-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37186-123">id</span><span class="sxs-lookup"><span data-stu-id="37186-123">id</span></span>|<span data-ttu-id="37186-124">String</span><span class="sxs-lookup"><span data-stu-id="37186-124">String</span></span>| <span data-ttu-id="37186-p102">数据透视表的 ID。 只读。</span><span class="sxs-lookup"><span data-stu-id="37186-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="37186-127">name</span><span class="sxs-lookup"><span data-stu-id="37186-127">name</span></span>|<span data-ttu-id="37186-128">String</span><span class="sxs-lookup"><span data-stu-id="37186-128">String</span></span>|<span data-ttu-id="37186-129">数据透视表对象的名称。</span><span class="sxs-lookup"><span data-stu-id="37186-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="37186-130">关系</span><span class="sxs-lookup"><span data-stu-id="37186-130">Relationships</span></span>
| <span data-ttu-id="37186-131">关系</span><span class="sxs-lookup"><span data-stu-id="37186-131">Relationship</span></span> | <span data-ttu-id="37186-132">类型</span><span class="sxs-lookup"><span data-stu-id="37186-132">Type</span></span>   |<span data-ttu-id="37186-133">说明</span><span class="sxs-lookup"><span data-stu-id="37186-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37186-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="37186-134">worksheet</span></span>|[<span data-ttu-id="37186-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="37186-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="37186-p103">包含当前 PivotTable 对象的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="37186-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="37186-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37186-138">JSON representation</span></span>
<span data-ttu-id="37186-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37186-139">Here is a JSON representation of the resource.</span></span>

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
