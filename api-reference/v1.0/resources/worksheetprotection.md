---
title: WorksheetProtection 资源类型
description: 表示对工作表对象的保护。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1c92c02b9c5e2409ad3036bbc34c41588161ae79
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345398"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="47771-103">WorksheetProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="47771-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="47771-104">表示对工作表对象的保护。</span><span class="sxs-lookup"><span data-stu-id="47771-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="47771-105">方法</span><span class="sxs-lookup"><span data-stu-id="47771-105">Methods</span></span>

| <span data-ttu-id="47771-106">方法</span><span class="sxs-lookup"><span data-stu-id="47771-106">Method</span></span>           | <span data-ttu-id="47771-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="47771-107">Return Type</span></span>    |<span data-ttu-id="47771-108">说明</span><span class="sxs-lookup"><span data-stu-id="47771-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="47771-109">获取 WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="47771-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="47771-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="47771-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="47771-111">读取 worksheetProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="47771-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="47771-112">保护</span><span class="sxs-lookup"><span data-stu-id="47771-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="47771-113">无</span><span class="sxs-lookup"><span data-stu-id="47771-113">None</span></span>|<span data-ttu-id="47771-p101">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="47771-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="47771-116">解除保护</span><span class="sxs-lookup"><span data-stu-id="47771-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="47771-117">无</span><span class="sxs-lookup"><span data-stu-id="47771-117">None</span></span>|<span data-ttu-id="47771-118">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="47771-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="47771-119">属性</span><span class="sxs-lookup"><span data-stu-id="47771-119">Properties</span></span>
| <span data-ttu-id="47771-120">属性</span><span class="sxs-lookup"><span data-stu-id="47771-120">Property</span></span>     | <span data-ttu-id="47771-121">类型</span><span class="sxs-lookup"><span data-stu-id="47771-121">Type</span></span>   |<span data-ttu-id="47771-122">说明</span><span class="sxs-lookup"><span data-stu-id="47771-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47771-123">选项</span><span class="sxs-lookup"><span data-stu-id="47771-123">options</span></span>|[<span data-ttu-id="47771-124">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="47771-124">workbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="47771-125">工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="47771-125">Sheet protection options.</span></span> <span data-ttu-id="47771-126">只读。</span><span class="sxs-lookup"><span data-stu-id="47771-126">Read-only.</span></span>|
|<span data-ttu-id="47771-127">protected</span><span class="sxs-lookup"><span data-stu-id="47771-127">protected</span></span>|<span data-ttu-id="47771-128">boolean</span><span class="sxs-lookup"><span data-stu-id="47771-128">boolean</span></span>|<span data-ttu-id="47771-p103">表示该工作表是否受保护。只读。</span><span class="sxs-lookup"><span data-stu-id="47771-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47771-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47771-131">JSON representation</span></span>

<span data-ttu-id="47771-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47771-132">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": true,
  "options": { "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
