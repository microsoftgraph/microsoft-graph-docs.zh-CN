---
title: workbookPivotTable 资源类型
description: 表示 Excel 数据透视表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d8df88699fde1e4d5562db6299cd12665512c03b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963988"
---
# <a name="workbookpivottable-resource-type"></a><span data-ttu-id="efe53-103">workbookPivotTable 资源类型</span><span class="sxs-lookup"><span data-stu-id="efe53-103">workbookPivotTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efe53-104">表示 Excel 数据透视表。</span><span class="sxs-lookup"><span data-stu-id="efe53-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="efe53-105">方法</span><span class="sxs-lookup"><span data-stu-id="efe53-105">Methods</span></span>

| <span data-ttu-id="efe53-106">方法</span><span class="sxs-lookup"><span data-stu-id="efe53-106">Method</span></span>           | <span data-ttu-id="efe53-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="efe53-107">Return Type</span></span>    |<span data-ttu-id="efe53-108">说明</span><span class="sxs-lookup"><span data-stu-id="efe53-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="efe53-109">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="efe53-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="efe53-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="efe53-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="efe53-111">读取 workbookPivotTable 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="efe53-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="efe53-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="efe53-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="efe53-113">无</span><span class="sxs-lookup"><span data-stu-id="efe53-113">None</span></span>|<span data-ttu-id="efe53-114">刷新数据透视表。</span><span class="sxs-lookup"><span data-stu-id="efe53-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="efe53-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="efe53-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="efe53-116">无</span><span class="sxs-lookup"><span data-stu-id="efe53-116">None</span></span>|<span data-ttu-id="efe53-p101">刷新给定工作表内的所有表。请注意，只能对数据透视表集合执行此操作。</span><span class="sxs-lookup"><span data-stu-id="efe53-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="efe53-119">属性</span><span class="sxs-lookup"><span data-stu-id="efe53-119">Properties</span></span>
| <span data-ttu-id="efe53-120">属性</span><span class="sxs-lookup"><span data-stu-id="efe53-120">Property</span></span>     | <span data-ttu-id="efe53-121">类型</span><span class="sxs-lookup"><span data-stu-id="efe53-121">Type</span></span>   |<span data-ttu-id="efe53-122">说明</span><span class="sxs-lookup"><span data-stu-id="efe53-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efe53-123">id</span><span class="sxs-lookup"><span data-stu-id="efe53-123">id</span></span>|<span data-ttu-id="efe53-124">String</span><span class="sxs-lookup"><span data-stu-id="efe53-124">String</span></span>| <span data-ttu-id="efe53-p102">数据透视表的 ID。 只读。</span><span class="sxs-lookup"><span data-stu-id="efe53-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="efe53-127">name</span><span class="sxs-lookup"><span data-stu-id="efe53-127">name</span></span>|<span data-ttu-id="efe53-128">String</span><span class="sxs-lookup"><span data-stu-id="efe53-128">String</span></span>|<span data-ttu-id="efe53-129">数据透视表对象的名称。</span><span class="sxs-lookup"><span data-stu-id="efe53-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="efe53-130">关系</span><span class="sxs-lookup"><span data-stu-id="efe53-130">Relationships</span></span>
| <span data-ttu-id="efe53-131">关系</span><span class="sxs-lookup"><span data-stu-id="efe53-131">Relationship</span></span> | <span data-ttu-id="efe53-132">类型</span><span class="sxs-lookup"><span data-stu-id="efe53-132">Type</span></span>   |<span data-ttu-id="efe53-133">说明</span><span class="sxs-lookup"><span data-stu-id="efe53-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efe53-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="efe53-134">worksheet</span></span>|[<span data-ttu-id="efe53-135">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="efe53-135">workbookWorksheet</span></span>](workbookworksheet.md)| <span data-ttu-id="efe53-136">包含当前 PivotTable 对象的工作表。</span><span class="sxs-lookup"><span data-stu-id="efe53-136">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="efe53-137">只读。</span><span class="sxs-lookup"><span data-stu-id="efe53-137">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="efe53-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="efe53-138">JSON representation</span></span>
<span data-ttu-id="efe53-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efe53-139">Here is a JSON representation of the resource.</span></span>

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
