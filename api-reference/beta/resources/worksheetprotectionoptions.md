---
title: WorksheetProtectionOptions 资源类型
description: 代表工作表保护中的选项。
author: lumine2008
ms.openlocfilehash: 772c8b5eca7e9754a6bbc00e43cac102680974a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348571"
---
# <a name="worksheetprotectionoptions-resource-type"></a><span data-ttu-id="d4279-103">WorksheetProtectionOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4279-103">WorksheetProtectionOptions resource type</span></span>

> <span data-ttu-id="d4279-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d4279-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4279-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d4279-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4279-106">表示工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="d4279-106">Represents the options in sheet protection.</span></span>

## <a name="properties"></a><span data-ttu-id="d4279-107">属性</span><span class="sxs-lookup"><span data-stu-id="d4279-107">Properties</span></span>
| <span data-ttu-id="d4279-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4279-108">Property</span></span>     | <span data-ttu-id="d4279-109">类型</span><span class="sxs-lookup"><span data-stu-id="d4279-109">Type</span></span>   |<span data-ttu-id="d4279-110">说明</span><span class="sxs-lookup"><span data-stu-id="d4279-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4279-111">allowAutoFilter</span><span class="sxs-lookup"><span data-stu-id="d4279-111">allowAutoFilter</span></span>|<span data-ttu-id="d4279-112">boolean</span><span class="sxs-lookup"><span data-stu-id="d4279-112">boolean</span></span>|<span data-ttu-id="d4279-113">表示允许使用自动筛选功能的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="d4279-113">Represents the worksheet protection option of allowing using auto filter feature.</span></span>|
|<span data-ttu-id="d4279-114">allowDeleteColumns</span><span class="sxs-lookup"><span data-stu-id="d4279-114">allowDeleteColumns</span></span>|<span data-ttu-id="d4279-115">boolean</span><span class="sxs-lookup"><span data-stu-id="d4279-115">boolean</span></span>|<span data-ttu-id="d4279-116">表示允许删除列的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="d4279-116">Represents the worksheet protection option of allowing deleting columns.</span></span>|
|<span data-ttu-id="d4279-117">allowDeleteRows</span><span class="sxs-lookup"><span data-stu-id="d4279-117">allowDeleteRows</span></span>|<span data-ttu-id="d4279-118">boolean</span><span class="sxs-lookup"><span data-stu-id="d4279-118">boolean</span></span>|<span data-ttu-id="d4279-119">表示允许删除行的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="d4279-119">Represents the worksheet protection option of allowing deleting rows.</span></span>|
|<span data-ttu-id="d4279-120">allowFormatCells</span><span class="sxs-lookup"><span data-stu-id="d4279-120">allowFormatCells</span></span>|<span data-ttu-id="d4279-121">boolean</span><span class="sxs-lookup"><span data-stu-id="d4279-121">boolean</span></span>|<span data-ttu-id="d4279-122">表示允许格式化单元格的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="d4279-122">Represents the worksheet protection option of allowing formatting cells.</span></span>|
|<span data-ttu-id="d4279-123">allowFormatColumns</span><span class="sxs-lookup"><span data-stu-id="d4279-123">allowFormatColumns</span></span>|<span data-ttu-id="d4279-124">boolean</span><span class="sxs-lookup"><span data-stu-id="d4279-124">boolean</span></span>|<span data-ttu-id="d4279-125">表示允许格式化列的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="d4279-125">Represents the worksheet protection option of allowing formatting columns.</span></span>|
|<span data-ttu-id="d4279-126">allowFormatRows</span><span class="sxs-lookup"><span data-stu-id="d4279-126">allowFormatRows</span></span>|<span data-ttu-id="d4279-127">boolean</span><span class="sxs-lookup"><span data-stu-id="d4279-127">boolean</span></span>|<span data-ttu-id="d4279-128">表示允许格式化行的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="d4279-128">Represents the worksheet protection option of allowing formatting rows.</span></span>|
|<span data-ttu-id="d4279-129">allowInsertColumns</span><span class="sxs-lookup"><span data-stu-id="d4279-129">allowInsertColumns</span></span>|<span data-ttu-id="d4279-130">boolean</span><span class="sxs-lookup"><span data-stu-id="d4279-130">boolean</span></span>|<span data-ttu-id="d4279-131">表示允许插入列的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="d4279-131">Represents the worksheet protection option of allowing inserting columns.</span></span>|
|<span data-ttu-id="d4279-132">allowInsertHyperlinks</span><span class="sxs-lookup"><span data-stu-id="d4279-132">allowInsertHyperlinks</span></span>|<span data-ttu-id="d4279-133">boolean</span><span class="sxs-lookup"><span data-stu-id="d4279-133">boolean</span></span>|<span data-ttu-id="d4279-134">表示允许插入超链接的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="d4279-134">Represents the worksheet protection option of allowing inserting hyperlinks.</span></span>|
|<span data-ttu-id="d4279-135">allowInsertRows</span><span class="sxs-lookup"><span data-stu-id="d4279-135">allowInsertRows</span></span>|<span data-ttu-id="d4279-136">boolean</span><span class="sxs-lookup"><span data-stu-id="d4279-136">boolean</span></span>|<span data-ttu-id="d4279-137">表示允许插入行的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="d4279-137">Represents the worksheet protection option of allowing inserting rows.</span></span>|
|<span data-ttu-id="d4279-138">allowPivotTables</span><span class="sxs-lookup"><span data-stu-id="d4279-138">allowPivotTables</span></span>|<span data-ttu-id="d4279-139">boolean</span><span class="sxs-lookup"><span data-stu-id="d4279-139">boolean</span></span>|<span data-ttu-id="d4279-140">表示允许使用数据透视表功能的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="d4279-140">Represents the worksheet protection option of allowing using pivot table feature.</span></span>|
|<span data-ttu-id="d4279-141">allowSort</span><span class="sxs-lookup"><span data-stu-id="d4279-141">allowSort</span></span>|<span data-ttu-id="d4279-142">boolean</span><span class="sxs-lookup"><span data-stu-id="d4279-142">boolean</span></span>|<span data-ttu-id="d4279-143">表示允许使用排序功能的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="d4279-143">Represents the worksheet protection option of allowing using sort feature.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4279-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4279-144">JSON representation</span></span>

<span data-ttu-id="d4279-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4279-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtectionOptions"
}-->

```json
{
  "allowAutoFilter": true,
  "allowDeleteColumns": true,
  "allowDeleteRows": true,
  "allowFormatCells": true,
  "allowFormatColumns": true,
  "allowFormatRows": true,
  "allowInsertColumns": true,
  "allowInsertHyperlinks": true,
  "allowInsertRows": true,
  "allowPivotTables": true,
  "allowSort": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtectionOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->