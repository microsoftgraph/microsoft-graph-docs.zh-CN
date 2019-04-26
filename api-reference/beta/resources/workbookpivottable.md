---
title: workbookPivotTable 资源类型
description: 表示 Excel 数据透视表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 99ad62474ef0c8e56ec5a699edac742ee28ae446
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345780"
---
# <a name="workbookpivottable-resource-type"></a><span data-ttu-id="aac50-103">workbookPivotTable 资源类型</span><span class="sxs-lookup"><span data-stu-id="aac50-103">workbookPivotTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aac50-104">表示 Excel 数据透视表。</span><span class="sxs-lookup"><span data-stu-id="aac50-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="aac50-105">方法</span><span class="sxs-lookup"><span data-stu-id="aac50-105">Methods</span></span>

| <span data-ttu-id="aac50-106">方法</span><span class="sxs-lookup"><span data-stu-id="aac50-106">Method</span></span>           | <span data-ttu-id="aac50-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="aac50-107">Return Type</span></span>    |<span data-ttu-id="aac50-108">说明</span><span class="sxs-lookup"><span data-stu-id="aac50-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aac50-109">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="aac50-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="aac50-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="aac50-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="aac50-111">读取 workbookPivotTable 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aac50-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="aac50-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="aac50-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="aac50-113">无</span><span class="sxs-lookup"><span data-stu-id="aac50-113">None</span></span>|<span data-ttu-id="aac50-114">刷新数据透视表。</span><span class="sxs-lookup"><span data-stu-id="aac50-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="aac50-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="aac50-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="aac50-116">无</span><span class="sxs-lookup"><span data-stu-id="aac50-116">None</span></span>|<span data-ttu-id="aac50-p101">刷新给定工作表内的所有表。请注意，只能对数据透视表集合执行此操作。</span><span class="sxs-lookup"><span data-stu-id="aac50-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="aac50-119">属性</span><span class="sxs-lookup"><span data-stu-id="aac50-119">Properties</span></span>
| <span data-ttu-id="aac50-120">属性</span><span class="sxs-lookup"><span data-stu-id="aac50-120">Property</span></span>     | <span data-ttu-id="aac50-121">类型</span><span class="sxs-lookup"><span data-stu-id="aac50-121">Type</span></span>   |<span data-ttu-id="aac50-122">说明</span><span class="sxs-lookup"><span data-stu-id="aac50-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aac50-123">id</span><span class="sxs-lookup"><span data-stu-id="aac50-123">id</span></span>|<span data-ttu-id="aac50-124">String</span><span class="sxs-lookup"><span data-stu-id="aac50-124">String</span></span>| <span data-ttu-id="aac50-p102">数据透视表的 ID。 只读。</span><span class="sxs-lookup"><span data-stu-id="aac50-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="aac50-127">name</span><span class="sxs-lookup"><span data-stu-id="aac50-127">name</span></span>|<span data-ttu-id="aac50-128">String</span><span class="sxs-lookup"><span data-stu-id="aac50-128">String</span></span>|<span data-ttu-id="aac50-129">数据透视表对象的名称。</span><span class="sxs-lookup"><span data-stu-id="aac50-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="aac50-130">关系</span><span class="sxs-lookup"><span data-stu-id="aac50-130">Relationships</span></span>
| <span data-ttu-id="aac50-131">关系</span><span class="sxs-lookup"><span data-stu-id="aac50-131">Relationship</span></span> | <span data-ttu-id="aac50-132">类型</span><span class="sxs-lookup"><span data-stu-id="aac50-132">Type</span></span>   |<span data-ttu-id="aac50-133">说明</span><span class="sxs-lookup"><span data-stu-id="aac50-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aac50-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="aac50-134">worksheet</span></span>|[<span data-ttu-id="aac50-135">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="aac50-135">workbookWorksheet</span></span>](workbookworksheet.md)| <span data-ttu-id="aac50-136">包含当前 PivotTable 对象的工作表。</span><span class="sxs-lookup"><span data-stu-id="aac50-136">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="aac50-137">只读。</span><span class="sxs-lookup"><span data-stu-id="aac50-137">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="aac50-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aac50-138">JSON representation</span></span>
<span data-ttu-id="aac50-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aac50-139">Here is a JSON representation of the resource.</span></span>

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
