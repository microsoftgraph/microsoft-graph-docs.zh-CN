---
title: pivotTable 资源类型
description: 表示 Excel 数据透视表。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: d500d4bc88608b032262cfae505385bf7ed3f072
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889206"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="7984c-103">pivotTable 资源类型</span><span class="sxs-lookup"><span data-stu-id="7984c-103">pivotTable resource type</span></span>

<span data-ttu-id="7984c-104">表示 Excel 数据透视表。</span><span class="sxs-lookup"><span data-stu-id="7984c-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="7984c-105">方法</span><span class="sxs-lookup"><span data-stu-id="7984c-105">Methods</span></span>

| <span data-ttu-id="7984c-106">方法</span><span class="sxs-lookup"><span data-stu-id="7984c-106">Method</span></span>           | <span data-ttu-id="7984c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="7984c-107">Return Type</span></span>    |<span data-ttu-id="7984c-108">说明</span><span class="sxs-lookup"><span data-stu-id="7984c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7984c-109">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="7984c-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="7984c-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="7984c-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="7984c-111">读取 workbookPivotTable 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7984c-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="7984c-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="7984c-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="7984c-113">无</span><span class="sxs-lookup"><span data-stu-id="7984c-113">None</span></span>|<span data-ttu-id="7984c-114">刷新数据透视表。</span><span class="sxs-lookup"><span data-stu-id="7984c-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="7984c-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="7984c-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="7984c-116">无</span><span class="sxs-lookup"><span data-stu-id="7984c-116">None</span></span>|<span data-ttu-id="7984c-p101">刷新给定工作表内的所有表。请注意，只能对数据透视表集合执行此操作。</span><span class="sxs-lookup"><span data-stu-id="7984c-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="7984c-119">属性</span><span class="sxs-lookup"><span data-stu-id="7984c-119">Properties</span></span>
| <span data-ttu-id="7984c-120">属性</span><span class="sxs-lookup"><span data-stu-id="7984c-120">Property</span></span>     | <span data-ttu-id="7984c-121">类型</span><span class="sxs-lookup"><span data-stu-id="7984c-121">Type</span></span>   |<span data-ttu-id="7984c-122">说明</span><span class="sxs-lookup"><span data-stu-id="7984c-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7984c-123">id</span><span class="sxs-lookup"><span data-stu-id="7984c-123">id</span></span>|<span data-ttu-id="7984c-124">String</span><span class="sxs-lookup"><span data-stu-id="7984c-124">String</span></span>| <span data-ttu-id="7984c-p102">数据透视表的 ID。 只读。</span><span class="sxs-lookup"><span data-stu-id="7984c-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="7984c-127">name</span><span class="sxs-lookup"><span data-stu-id="7984c-127">name</span></span>|<span data-ttu-id="7984c-128">String</span><span class="sxs-lookup"><span data-stu-id="7984c-128">String</span></span>|<span data-ttu-id="7984c-129">数据透视表对象的名称。</span><span class="sxs-lookup"><span data-stu-id="7984c-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="7984c-130">关系</span><span class="sxs-lookup"><span data-stu-id="7984c-130">Relationships</span></span>
| <span data-ttu-id="7984c-131">关系</span><span class="sxs-lookup"><span data-stu-id="7984c-131">Relationship</span></span> | <span data-ttu-id="7984c-132">类型</span><span class="sxs-lookup"><span data-stu-id="7984c-132">Type</span></span>   |<span data-ttu-id="7984c-133">说明</span><span class="sxs-lookup"><span data-stu-id="7984c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7984c-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="7984c-134">worksheet</span></span>|[<span data-ttu-id="7984c-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="7984c-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="7984c-p103">包含当前 PivotTable 对象的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="7984c-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="7984c-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7984c-138">JSON representation</span></span>
<span data-ttu-id="7984c-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7984c-139">Here is a JSON representation of the resource.</span></span>

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
