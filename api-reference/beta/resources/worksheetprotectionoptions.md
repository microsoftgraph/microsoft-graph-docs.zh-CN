---
title: WorksheetProtectionOptions 资源类型
description: 代表工作表保护中的选项。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 8753ae0b266c2bb3c44fdc3b10f843c58a522627
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845658"
---
# <a name="worksheetprotectionoptions-resource-type"></a><span data-ttu-id="ad01c-103">WorksheetProtectionOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad01c-103">WorksheetProtectionOptions resource type</span></span>

> <span data-ttu-id="ad01c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ad01c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad01c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ad01c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad01c-106">表示工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="ad01c-106">Represents the options in sheet protection.</span></span>

## <a name="properties"></a><span data-ttu-id="ad01c-107">属性</span><span class="sxs-lookup"><span data-stu-id="ad01c-107">Properties</span></span>
| <span data-ttu-id="ad01c-108">属性</span><span class="sxs-lookup"><span data-stu-id="ad01c-108">Property</span></span>     | <span data-ttu-id="ad01c-109">类型</span><span class="sxs-lookup"><span data-stu-id="ad01c-109">Type</span></span>   |<span data-ttu-id="ad01c-110">说明</span><span class="sxs-lookup"><span data-stu-id="ad01c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad01c-111">allowAutoFilter</span><span class="sxs-lookup"><span data-stu-id="ad01c-111">allowAutoFilter</span></span>|<span data-ttu-id="ad01c-112">boolean</span><span class="sxs-lookup"><span data-stu-id="ad01c-112">boolean</span></span>|<span data-ttu-id="ad01c-113">表示允许使用自动筛选功能的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="ad01c-113">Represents the worksheet protection option of allowing using auto filter feature.</span></span>|
|<span data-ttu-id="ad01c-114">allowDeleteColumns</span><span class="sxs-lookup"><span data-stu-id="ad01c-114">allowDeleteColumns</span></span>|<span data-ttu-id="ad01c-115">boolean</span><span class="sxs-lookup"><span data-stu-id="ad01c-115">boolean</span></span>|<span data-ttu-id="ad01c-116">表示允许删除列的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="ad01c-116">Represents the worksheet protection option of allowing deleting columns.</span></span>|
|<span data-ttu-id="ad01c-117">allowDeleteRows</span><span class="sxs-lookup"><span data-stu-id="ad01c-117">allowDeleteRows</span></span>|<span data-ttu-id="ad01c-118">boolean</span><span class="sxs-lookup"><span data-stu-id="ad01c-118">boolean</span></span>|<span data-ttu-id="ad01c-119">表示允许删除行的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="ad01c-119">Represents the worksheet protection option of allowing deleting rows.</span></span>|
|<span data-ttu-id="ad01c-120">allowFormatCells</span><span class="sxs-lookup"><span data-stu-id="ad01c-120">allowFormatCells</span></span>|<span data-ttu-id="ad01c-121">boolean</span><span class="sxs-lookup"><span data-stu-id="ad01c-121">boolean</span></span>|<span data-ttu-id="ad01c-122">表示允许格式化单元格的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="ad01c-122">Represents the worksheet protection option of allowing formatting cells.</span></span>|
|<span data-ttu-id="ad01c-123">allowFormatColumns</span><span class="sxs-lookup"><span data-stu-id="ad01c-123">allowFormatColumns</span></span>|<span data-ttu-id="ad01c-124">boolean</span><span class="sxs-lookup"><span data-stu-id="ad01c-124">boolean</span></span>|<span data-ttu-id="ad01c-125">表示允许格式化列的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="ad01c-125">Represents the worksheet protection option of allowing formatting columns.</span></span>|
|<span data-ttu-id="ad01c-126">allowFormatRows</span><span class="sxs-lookup"><span data-stu-id="ad01c-126">allowFormatRows</span></span>|<span data-ttu-id="ad01c-127">boolean</span><span class="sxs-lookup"><span data-stu-id="ad01c-127">boolean</span></span>|<span data-ttu-id="ad01c-128">表示允许格式化行的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="ad01c-128">Represents the worksheet protection option of allowing formatting rows.</span></span>|
|<span data-ttu-id="ad01c-129">allowInsertColumns</span><span class="sxs-lookup"><span data-stu-id="ad01c-129">allowInsertColumns</span></span>|<span data-ttu-id="ad01c-130">boolean</span><span class="sxs-lookup"><span data-stu-id="ad01c-130">boolean</span></span>|<span data-ttu-id="ad01c-131">表示允许插入列的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="ad01c-131">Represents the worksheet protection option of allowing inserting columns.</span></span>|
|<span data-ttu-id="ad01c-132">allowInsertHyperlinks</span><span class="sxs-lookup"><span data-stu-id="ad01c-132">allowInsertHyperlinks</span></span>|<span data-ttu-id="ad01c-133">boolean</span><span class="sxs-lookup"><span data-stu-id="ad01c-133">boolean</span></span>|<span data-ttu-id="ad01c-134">表示允许插入超链接的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="ad01c-134">Represents the worksheet protection option of allowing inserting hyperlinks.</span></span>|
|<span data-ttu-id="ad01c-135">allowInsertRows</span><span class="sxs-lookup"><span data-stu-id="ad01c-135">allowInsertRows</span></span>|<span data-ttu-id="ad01c-136">boolean</span><span class="sxs-lookup"><span data-stu-id="ad01c-136">boolean</span></span>|<span data-ttu-id="ad01c-137">表示允许插入行的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="ad01c-137">Represents the worksheet protection option of allowing inserting rows.</span></span>|
|<span data-ttu-id="ad01c-138">allowPivotTables</span><span class="sxs-lookup"><span data-stu-id="ad01c-138">allowPivotTables</span></span>|<span data-ttu-id="ad01c-139">boolean</span><span class="sxs-lookup"><span data-stu-id="ad01c-139">boolean</span></span>|<span data-ttu-id="ad01c-140">表示允许使用数据透视表功能的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="ad01c-140">Represents the worksheet protection option of allowing using pivot table feature.</span></span>|
|<span data-ttu-id="ad01c-141">allowSort</span><span class="sxs-lookup"><span data-stu-id="ad01c-141">allowSort</span></span>|<span data-ttu-id="ad01c-142">boolean</span><span class="sxs-lookup"><span data-stu-id="ad01c-142">boolean</span></span>|<span data-ttu-id="ad01c-143">表示允许使用排序功能的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="ad01c-143">Represents the worksheet protection option of allowing using sort feature.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad01c-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad01c-144">JSON representation</span></span>

<span data-ttu-id="ad01c-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad01c-145">Here is a JSON representation of the resource.</span></span>

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
