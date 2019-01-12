---
title: pivotTable 资源类型
description: 表示 Excel 数据透视表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 91035b607d8c44f2d1515e9c004abd4c2235c0ec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950856"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="0cce6-103">pivotTable 资源类型</span><span class="sxs-lookup"><span data-stu-id="0cce6-103">pivotTable resource type</span></span>

> <span data-ttu-id="0cce6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0cce6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0cce6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0cce6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0cce6-106">表示 Excel 数据透视表。</span><span class="sxs-lookup"><span data-stu-id="0cce6-106">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="0cce6-107">方法</span><span class="sxs-lookup"><span data-stu-id="0cce6-107">Methods</span></span>

| <span data-ttu-id="0cce6-108">方法</span><span class="sxs-lookup"><span data-stu-id="0cce6-108">Method</span></span>           | <span data-ttu-id="0cce6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0cce6-109">Return Type</span></span>    |<span data-ttu-id="0cce6-110">说明</span><span class="sxs-lookup"><span data-stu-id="0cce6-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0cce6-111">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="0cce6-111">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="0cce6-112">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="0cce6-112">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="0cce6-113">读取 workbookPivotTable 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0cce6-113">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="0cce6-114">Refresh</span><span class="sxs-lookup"><span data-stu-id="0cce6-114">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="0cce6-115">无</span><span class="sxs-lookup"><span data-stu-id="0cce6-115">None</span></span>|<span data-ttu-id="0cce6-116">刷新数据透视表。</span><span class="sxs-lookup"><span data-stu-id="0cce6-116">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="0cce6-117">Refreshall</span><span class="sxs-lookup"><span data-stu-id="0cce6-117">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="0cce6-118">无</span><span class="sxs-lookup"><span data-stu-id="0cce6-118">None</span></span>|<span data-ttu-id="0cce6-p102">刷新给定工作表内的所有表。请注意，只能对数据透视表集合执行此操作。</span><span class="sxs-lookup"><span data-stu-id="0cce6-p102">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="0cce6-121">属性</span><span class="sxs-lookup"><span data-stu-id="0cce6-121">Properties</span></span>
| <span data-ttu-id="0cce6-122">属性</span><span class="sxs-lookup"><span data-stu-id="0cce6-122">Property</span></span>     | <span data-ttu-id="0cce6-123">类型</span><span class="sxs-lookup"><span data-stu-id="0cce6-123">Type</span></span>   |<span data-ttu-id="0cce6-124">说明</span><span class="sxs-lookup"><span data-stu-id="0cce6-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cce6-125">id</span><span class="sxs-lookup"><span data-stu-id="0cce6-125">id</span></span>|<span data-ttu-id="0cce6-126">String</span><span class="sxs-lookup"><span data-stu-id="0cce6-126">String</span></span>| <span data-ttu-id="0cce6-p103">数据透视表的 ID。 只读。</span><span class="sxs-lookup"><span data-stu-id="0cce6-p103">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="0cce6-129">name</span><span class="sxs-lookup"><span data-stu-id="0cce6-129">name</span></span>|<span data-ttu-id="0cce6-130">String</span><span class="sxs-lookup"><span data-stu-id="0cce6-130">String</span></span>|<span data-ttu-id="0cce6-131">数据透视表对象的名称。</span><span class="sxs-lookup"><span data-stu-id="0cce6-131">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="0cce6-132">关系</span><span class="sxs-lookup"><span data-stu-id="0cce6-132">Relationships</span></span>
| <span data-ttu-id="0cce6-133">关系</span><span class="sxs-lookup"><span data-stu-id="0cce6-133">Relationship</span></span> | <span data-ttu-id="0cce6-134">类型</span><span class="sxs-lookup"><span data-stu-id="0cce6-134">Type</span></span>   |<span data-ttu-id="0cce6-135">说明</span><span class="sxs-lookup"><span data-stu-id="0cce6-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cce6-136">worksheet</span><span class="sxs-lookup"><span data-stu-id="0cce6-136">worksheet</span></span>|[<span data-ttu-id="0cce6-137">worksheet</span><span class="sxs-lookup"><span data-stu-id="0cce6-137">worksheet</span></span>](worksheet.md)| <span data-ttu-id="0cce6-p104">包含当前数据透视表对象的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="0cce6-p104">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="0cce6-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0cce6-140">JSON representation</span></span>
<span data-ttu-id="0cce6-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0cce6-141">Here is a JSON representation of the resource.</span></span>

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
