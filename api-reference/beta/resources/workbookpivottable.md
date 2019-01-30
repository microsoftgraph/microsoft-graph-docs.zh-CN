---
title: pivotTable 资源类型
description: 表示 Excel 数据透视表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fc43bf160e93e354ff58b2f960e8ec38d252287f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641104"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="812be-103">pivotTable 资源类型</span><span class="sxs-lookup"><span data-stu-id="812be-103">pivotTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="812be-104">表示 Excel 数据透视表。</span><span class="sxs-lookup"><span data-stu-id="812be-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="812be-105">方法</span><span class="sxs-lookup"><span data-stu-id="812be-105">Methods</span></span>

| <span data-ttu-id="812be-106">方法</span><span class="sxs-lookup"><span data-stu-id="812be-106">Method</span></span>           | <span data-ttu-id="812be-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="812be-107">Return Type</span></span>    |<span data-ttu-id="812be-108">说明</span><span class="sxs-lookup"><span data-stu-id="812be-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="812be-109">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="812be-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="812be-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="812be-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="812be-111">读取 workbookPivotTable 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="812be-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="812be-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="812be-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="812be-113">无</span><span class="sxs-lookup"><span data-stu-id="812be-113">None</span></span>|<span data-ttu-id="812be-114">刷新数据透视表。</span><span class="sxs-lookup"><span data-stu-id="812be-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="812be-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="812be-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="812be-116">无</span><span class="sxs-lookup"><span data-stu-id="812be-116">None</span></span>|<span data-ttu-id="812be-p101">刷新给定工作表内的所有表。请注意，只能对数据透视表集合执行此操作。</span><span class="sxs-lookup"><span data-stu-id="812be-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="812be-119">属性</span><span class="sxs-lookup"><span data-stu-id="812be-119">Properties</span></span>
| <span data-ttu-id="812be-120">属性</span><span class="sxs-lookup"><span data-stu-id="812be-120">Property</span></span>     | <span data-ttu-id="812be-121">类型</span><span class="sxs-lookup"><span data-stu-id="812be-121">Type</span></span>   |<span data-ttu-id="812be-122">说明</span><span class="sxs-lookup"><span data-stu-id="812be-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="812be-123">id</span><span class="sxs-lookup"><span data-stu-id="812be-123">id</span></span>|<span data-ttu-id="812be-124">String</span><span class="sxs-lookup"><span data-stu-id="812be-124">String</span></span>| <span data-ttu-id="812be-p102">数据透视表的 ID。 只读。</span><span class="sxs-lookup"><span data-stu-id="812be-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="812be-127">name</span><span class="sxs-lookup"><span data-stu-id="812be-127">name</span></span>|<span data-ttu-id="812be-128">String</span><span class="sxs-lookup"><span data-stu-id="812be-128">String</span></span>|<span data-ttu-id="812be-129">数据透视表对象的名称。</span><span class="sxs-lookup"><span data-stu-id="812be-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="812be-130">关系</span><span class="sxs-lookup"><span data-stu-id="812be-130">Relationships</span></span>
| <span data-ttu-id="812be-131">关系</span><span class="sxs-lookup"><span data-stu-id="812be-131">Relationship</span></span> | <span data-ttu-id="812be-132">类型</span><span class="sxs-lookup"><span data-stu-id="812be-132">Type</span></span>   |<span data-ttu-id="812be-133">说明</span><span class="sxs-lookup"><span data-stu-id="812be-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="812be-134">worksheet</span><span class="sxs-lookup"><span data-stu-id="812be-134">worksheet</span></span>|[<span data-ttu-id="812be-135">worksheet</span><span class="sxs-lookup"><span data-stu-id="812be-135">worksheet</span></span>](worksheet.md)| <span data-ttu-id="812be-p103">包含当前数据透视表对象的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="812be-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="812be-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="812be-138">JSON representation</span></span>
<span data-ttu-id="812be-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="812be-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookpivottable.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
