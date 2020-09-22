---
title: WorksheetProtection 资源类型
description: 表示对工作表对象的保护。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8bb91dae367f9f9c95465aed0f8c71a26aaddd1a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014999"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="5ec42-103">WorksheetProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ec42-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="5ec42-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ec42-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ec42-105">表示对工作表对象的保护。</span><span class="sxs-lookup"><span data-stu-id="5ec42-105">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="5ec42-106">方法</span><span class="sxs-lookup"><span data-stu-id="5ec42-106">Methods</span></span>

| <span data-ttu-id="5ec42-107">方法</span><span class="sxs-lookup"><span data-stu-id="5ec42-107">Method</span></span>           | <span data-ttu-id="5ec42-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="5ec42-108">Return Type</span></span>    |<span data-ttu-id="5ec42-109">说明</span><span class="sxs-lookup"><span data-stu-id="5ec42-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5ec42-110">获取 WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="5ec42-110">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="5ec42-111">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="5ec42-111">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="5ec42-112">读取 worksheetProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5ec42-112">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="5ec42-113">保护</span><span class="sxs-lookup"><span data-stu-id="5ec42-113">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="5ec42-114">无</span><span class="sxs-lookup"><span data-stu-id="5ec42-114">None</span></span>|<span data-ttu-id="5ec42-p101">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="5ec42-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="5ec42-117">解除保护</span><span class="sxs-lookup"><span data-stu-id="5ec42-117">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="5ec42-118">无</span><span class="sxs-lookup"><span data-stu-id="5ec42-118">None</span></span>|<span data-ttu-id="5ec42-119">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="5ec42-119">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="5ec42-120">属性</span><span class="sxs-lookup"><span data-stu-id="5ec42-120">Properties</span></span>
| <span data-ttu-id="5ec42-121">属性</span><span class="sxs-lookup"><span data-stu-id="5ec42-121">Property</span></span>     | <span data-ttu-id="5ec42-122">类型</span><span class="sxs-lookup"><span data-stu-id="5ec42-122">Type</span></span>   |<span data-ttu-id="5ec42-123">说明</span><span class="sxs-lookup"><span data-stu-id="5ec42-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ec42-124">选项</span><span class="sxs-lookup"><span data-stu-id="5ec42-124">options</span></span>|[<span data-ttu-id="5ec42-125">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="5ec42-125">workbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="5ec42-126">工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="5ec42-126">Sheet protection options.</span></span> <span data-ttu-id="5ec42-127">只读。</span><span class="sxs-lookup"><span data-stu-id="5ec42-127">Read-only.</span></span>|
|<span data-ttu-id="5ec42-128">protected</span><span class="sxs-lookup"><span data-stu-id="5ec42-128">protected</span></span>|<span data-ttu-id="5ec42-129">boolean</span><span class="sxs-lookup"><span data-stu-id="5ec42-129">boolean</span></span>|<span data-ttu-id="5ec42-p103">表示该工作表是否受保护。只读。</span><span class="sxs-lookup"><span data-stu-id="5ec42-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ec42-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ec42-132">JSON representation</span></span>

<span data-ttu-id="5ec42-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ec42-133">Here is a JSON representation of the resource.</span></span>

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

