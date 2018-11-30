---
title: WorksheetProtectionOptions 资源类型
description: 代表工作表保护中的选项。
ms.openlocfilehash: 2944663c62edd6533a12afe8e24cdd4f84f038fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042712"
---
# <a name="worksheetprotectionoptions-resource-type"></a><span data-ttu-id="a1b24-103">WorksheetProtectionOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="a1b24-103">WorksheetProtectionOptions resource type</span></span>

> <span data-ttu-id="a1b24-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a1b24-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1b24-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a1b24-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1b24-106">表示工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="a1b24-106">Represents the options in sheet protection.</span></span>

## <a name="properties"></a><span data-ttu-id="a1b24-107">属性</span><span class="sxs-lookup"><span data-stu-id="a1b24-107">Properties</span></span>
| <span data-ttu-id="a1b24-108">属性</span><span class="sxs-lookup"><span data-stu-id="a1b24-108">Property</span></span>     | <span data-ttu-id="a1b24-109">类型</span><span class="sxs-lookup"><span data-stu-id="a1b24-109">Type</span></span>   |<span data-ttu-id="a1b24-110">说明</span><span class="sxs-lookup"><span data-stu-id="a1b24-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1b24-111">allowAutoFilter</span><span class="sxs-lookup"><span data-stu-id="a1b24-111">allowAutoFilter</span></span>|<span data-ttu-id="a1b24-112">boolean</span><span class="sxs-lookup"><span data-stu-id="a1b24-112">boolean</span></span>|<span data-ttu-id="a1b24-113">表示允许使用自动筛选功能的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="a1b24-113">Represents the worksheet protection option of allowing using auto filter feature.</span></span>|
|<span data-ttu-id="a1b24-114">allowDeleteColumns</span><span class="sxs-lookup"><span data-stu-id="a1b24-114">allowDeleteColumns</span></span>|<span data-ttu-id="a1b24-115">boolean</span><span class="sxs-lookup"><span data-stu-id="a1b24-115">boolean</span></span>|<span data-ttu-id="a1b24-116">表示允许删除列的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="a1b24-116">Represents the worksheet protection option of allowing deleting columns.</span></span>|
|<span data-ttu-id="a1b24-117">allowDeleteRows</span><span class="sxs-lookup"><span data-stu-id="a1b24-117">allowDeleteRows</span></span>|<span data-ttu-id="a1b24-118">boolean</span><span class="sxs-lookup"><span data-stu-id="a1b24-118">boolean</span></span>|<span data-ttu-id="a1b24-119">表示允许删除行的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="a1b24-119">Represents the worksheet protection option of allowing deleting rows.</span></span>|
|<span data-ttu-id="a1b24-120">allowFormatCells</span><span class="sxs-lookup"><span data-stu-id="a1b24-120">allowFormatCells</span></span>|<span data-ttu-id="a1b24-121">boolean</span><span class="sxs-lookup"><span data-stu-id="a1b24-121">boolean</span></span>|<span data-ttu-id="a1b24-122">表示允许格式化单元格的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="a1b24-122">Represents the worksheet protection option of allowing formatting cells.</span></span>|
|<span data-ttu-id="a1b24-123">allowFormatColumns</span><span class="sxs-lookup"><span data-stu-id="a1b24-123">allowFormatColumns</span></span>|<span data-ttu-id="a1b24-124">boolean</span><span class="sxs-lookup"><span data-stu-id="a1b24-124">boolean</span></span>|<span data-ttu-id="a1b24-125">表示允许格式化列的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="a1b24-125">Represents the worksheet protection option of allowing formatting columns.</span></span>|
|<span data-ttu-id="a1b24-126">allowFormatRows</span><span class="sxs-lookup"><span data-stu-id="a1b24-126">allowFormatRows</span></span>|<span data-ttu-id="a1b24-127">boolean</span><span class="sxs-lookup"><span data-stu-id="a1b24-127">boolean</span></span>|<span data-ttu-id="a1b24-128">表示允许格式化行的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="a1b24-128">Represents the worksheet protection option of allowing formatting rows.</span></span>|
|<span data-ttu-id="a1b24-129">allowInsertColumns</span><span class="sxs-lookup"><span data-stu-id="a1b24-129">allowInsertColumns</span></span>|<span data-ttu-id="a1b24-130">boolean</span><span class="sxs-lookup"><span data-stu-id="a1b24-130">boolean</span></span>|<span data-ttu-id="a1b24-131">表示允许插入列的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="a1b24-131">Represents the worksheet protection option of allowing inserting columns.</span></span>|
|<span data-ttu-id="a1b24-132">allowInsertHyperlinks</span><span class="sxs-lookup"><span data-stu-id="a1b24-132">allowInsertHyperlinks</span></span>|<span data-ttu-id="a1b24-133">boolean</span><span class="sxs-lookup"><span data-stu-id="a1b24-133">boolean</span></span>|<span data-ttu-id="a1b24-134">表示允许插入超链接的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="a1b24-134">Represents the worksheet protection option of allowing inserting hyperlinks.</span></span>|
|<span data-ttu-id="a1b24-135">allowInsertRows</span><span class="sxs-lookup"><span data-stu-id="a1b24-135">allowInsertRows</span></span>|<span data-ttu-id="a1b24-136">boolean</span><span class="sxs-lookup"><span data-stu-id="a1b24-136">boolean</span></span>|<span data-ttu-id="a1b24-137">表示允许插入行的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="a1b24-137">Represents the worksheet protection option of allowing inserting rows.</span></span>|
|<span data-ttu-id="a1b24-138">allowPivotTables</span><span class="sxs-lookup"><span data-stu-id="a1b24-138">allowPivotTables</span></span>|<span data-ttu-id="a1b24-139">boolean</span><span class="sxs-lookup"><span data-stu-id="a1b24-139">boolean</span></span>|<span data-ttu-id="a1b24-140">表示允许使用数据透视表功能的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="a1b24-140">Represents the worksheet protection option of allowing using pivot table feature.</span></span>|
|<span data-ttu-id="a1b24-141">allowSort</span><span class="sxs-lookup"><span data-stu-id="a1b24-141">allowSort</span></span>|<span data-ttu-id="a1b24-142">boolean</span><span class="sxs-lookup"><span data-stu-id="a1b24-142">boolean</span></span>|<span data-ttu-id="a1b24-143">表示允许使用排序功能的工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="a1b24-143">Represents the worksheet protection option of allowing using sort feature.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1b24-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1b24-144">JSON representation</span></span>

<span data-ttu-id="a1b24-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1b24-145">Here is a JSON representation of the resource.</span></span>

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