---
title: WorksheetProtection 资源类型
description: 表示对工作表对象的保护。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 805c3b53a60495ebd50a230a83e3ce1272cacf4d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446665"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="79f23-103">WorksheetProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="79f23-103">WorksheetProtection resource type</span></span>

<span data-ttu-id="79f23-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="79f23-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79f23-105">表示对工作表对象的保护。</span><span class="sxs-lookup"><span data-stu-id="79f23-105">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="79f23-106">方法</span><span class="sxs-lookup"><span data-stu-id="79f23-106">Methods</span></span>

| <span data-ttu-id="79f23-107">方法</span><span class="sxs-lookup"><span data-stu-id="79f23-107">Method</span></span>           | <span data-ttu-id="79f23-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="79f23-108">Return Type</span></span>    |<span data-ttu-id="79f23-109">说明</span><span class="sxs-lookup"><span data-stu-id="79f23-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="79f23-110">获取 WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="79f23-110">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="79f23-111">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="79f23-111">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="79f23-112">读取 worksheetProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="79f23-112">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="79f23-113">保护</span><span class="sxs-lookup"><span data-stu-id="79f23-113">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="79f23-114">无</span><span class="sxs-lookup"><span data-stu-id="79f23-114">None</span></span>|<span data-ttu-id="79f23-p101">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="79f23-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="79f23-117">解除保护</span><span class="sxs-lookup"><span data-stu-id="79f23-117">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="79f23-118">无</span><span class="sxs-lookup"><span data-stu-id="79f23-118">None</span></span>|<span data-ttu-id="79f23-119">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="79f23-119">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="79f23-120">属性</span><span class="sxs-lookup"><span data-stu-id="79f23-120">Properties</span></span>
| <span data-ttu-id="79f23-121">属性</span><span class="sxs-lookup"><span data-stu-id="79f23-121">Property</span></span>     | <span data-ttu-id="79f23-122">类型</span><span class="sxs-lookup"><span data-stu-id="79f23-122">Type</span></span>   |<span data-ttu-id="79f23-123">说明</span><span class="sxs-lookup"><span data-stu-id="79f23-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79f23-124">选项</span><span class="sxs-lookup"><span data-stu-id="79f23-124">options</span></span>|[<span data-ttu-id="79f23-125">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="79f23-125">workbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="79f23-126">工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="79f23-126">Sheet protection options.</span></span> <span data-ttu-id="79f23-127">只读。</span><span class="sxs-lookup"><span data-stu-id="79f23-127">Read-only.</span></span>|
|<span data-ttu-id="79f23-128">protected</span><span class="sxs-lookup"><span data-stu-id="79f23-128">protected</span></span>|<span data-ttu-id="79f23-129">boolean</span><span class="sxs-lookup"><span data-stu-id="79f23-129">boolean</span></span>|<span data-ttu-id="79f23-p103">表示该工作表是否受保护。只读。</span><span class="sxs-lookup"><span data-stu-id="79f23-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79f23-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79f23-132">JSON representation</span></span>

<span data-ttu-id="79f23-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79f23-133">Here is a JSON representation of the resource.</span></span>

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
