---
title: WorksheetProtection 资源类型
description: 表示对工作表对象的保护。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c8a719d1be9f21edf1bef82d2aa058b45bbf2df8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463612"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="b5afb-103">WorksheetProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5afb-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="b5afb-104">表示对工作表对象的保护。</span><span class="sxs-lookup"><span data-stu-id="b5afb-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="b5afb-105">方法</span><span class="sxs-lookup"><span data-stu-id="b5afb-105">Methods</span></span>

| <span data-ttu-id="b5afb-106">方法</span><span class="sxs-lookup"><span data-stu-id="b5afb-106">Method</span></span>           | <span data-ttu-id="b5afb-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="b5afb-107">Return Type</span></span>    |<span data-ttu-id="b5afb-108">说明</span><span class="sxs-lookup"><span data-stu-id="b5afb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b5afb-109">获取 WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="b5afb-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="b5afb-110">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="b5afb-110">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="b5afb-111">读取 worksheetProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b5afb-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="b5afb-112">保护</span><span class="sxs-lookup"><span data-stu-id="b5afb-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="b5afb-113">无</span><span class="sxs-lookup"><span data-stu-id="b5afb-113">None</span></span>|<span data-ttu-id="b5afb-p101">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="b5afb-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="b5afb-116">解除保护</span><span class="sxs-lookup"><span data-stu-id="b5afb-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="b5afb-117">无</span><span class="sxs-lookup"><span data-stu-id="b5afb-117">None</span></span>|<span data-ttu-id="b5afb-118">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="b5afb-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="b5afb-119">属性</span><span class="sxs-lookup"><span data-stu-id="b5afb-119">Properties</span></span>
| <span data-ttu-id="b5afb-120">属性</span><span class="sxs-lookup"><span data-stu-id="b5afb-120">Property</span></span>     | <span data-ttu-id="b5afb-121">类型</span><span class="sxs-lookup"><span data-stu-id="b5afb-121">Type</span></span>   |<span data-ttu-id="b5afb-122">说明</span><span class="sxs-lookup"><span data-stu-id="b5afb-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5afb-123">选项</span><span class="sxs-lookup"><span data-stu-id="b5afb-123">options</span></span>|[<span data-ttu-id="b5afb-124">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="b5afb-124">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="b5afb-125">工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="b5afb-125">Sheet protection options.</span></span> <span data-ttu-id="b5afb-126">只读。</span><span class="sxs-lookup"><span data-stu-id="b5afb-126">Read-only.</span></span>|
|<span data-ttu-id="b5afb-127">protected</span><span class="sxs-lookup"><span data-stu-id="b5afb-127">protected</span></span>|<span data-ttu-id="b5afb-128">boolean</span><span class="sxs-lookup"><span data-stu-id="b5afb-128">boolean</span></span>|<span data-ttu-id="b5afb-p103">表示该工作表是否受保护。只读。</span><span class="sxs-lookup"><span data-stu-id="b5afb-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5afb-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5afb-131">JSON representation</span></span>

<span data-ttu-id="b5afb-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5afb-132">Here is a JSON representation of the resource.</span></span>

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
