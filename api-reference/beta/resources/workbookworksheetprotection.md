---
title: workbookWorksheetProtection 资源类型
description: 表示对工作表对象的保护。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7e4a2f3130c71df35b1106d1a342004cfc6fdf25
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348574"
---
# <a name="workbookworksheetprotection-resource-type"></a><span data-ttu-id="aaee0-103">workbookWorksheetProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="aaee0-103">workbookWorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aaee0-104">表示对工作表对象的保护。</span><span class="sxs-lookup"><span data-stu-id="aaee0-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="aaee0-105">方法</span><span class="sxs-lookup"><span data-stu-id="aaee0-105">Methods</span></span>

| <span data-ttu-id="aaee0-106">方法</span><span class="sxs-lookup"><span data-stu-id="aaee0-106">Method</span></span>           | <span data-ttu-id="aaee0-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="aaee0-107">Return Type</span></span>    |<span data-ttu-id="aaee0-108">说明</span><span class="sxs-lookup"><span data-stu-id="aaee0-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aaee0-109">获取 workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="aaee0-109">Get workbookWorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="aaee0-110">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="aaee0-110">workbookWorksheetProtection</span></span>](workbookworksheetprotection.md) |<span data-ttu-id="aaee0-111">读取 workbookWorksheetProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aaee0-111">Read properties and relationships of workbookWorksheetProtection object.</span></span>|
|[<span data-ttu-id="aaee0-112">保护</span><span class="sxs-lookup"><span data-stu-id="aaee0-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="aaee0-113">无</span><span class="sxs-lookup"><span data-stu-id="aaee0-113">None</span></span>|<span data-ttu-id="aaee0-p101">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="aaee0-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="aaee0-116">解除保护</span><span class="sxs-lookup"><span data-stu-id="aaee0-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="aaee0-117">无</span><span class="sxs-lookup"><span data-stu-id="aaee0-117">None</span></span>|<span data-ttu-id="aaee0-118">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="aaee0-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="aaee0-119">属性</span><span class="sxs-lookup"><span data-stu-id="aaee0-119">Properties</span></span>
| <span data-ttu-id="aaee0-120">属性</span><span class="sxs-lookup"><span data-stu-id="aaee0-120">Property</span></span>     | <span data-ttu-id="aaee0-121">类型</span><span class="sxs-lookup"><span data-stu-id="aaee0-121">Type</span></span>   |<span data-ttu-id="aaee0-122">说明</span><span class="sxs-lookup"><span data-stu-id="aaee0-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aaee0-123">选项</span><span class="sxs-lookup"><span data-stu-id="aaee0-123">options</span></span>|[<span data-ttu-id="aaee0-124">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="aaee0-124">workbookWorksheetProtectionOptions</span></span>](workbookworksheetprotectionoptions.md)|<span data-ttu-id="aaee0-125">工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="aaee0-125">Sheet protection options.</span></span> <span data-ttu-id="aaee0-126">只读。</span><span class="sxs-lookup"><span data-stu-id="aaee0-126">Read-only.</span></span>|
|<span data-ttu-id="aaee0-127">protected</span><span class="sxs-lookup"><span data-stu-id="aaee0-127">protected</span></span>|<span data-ttu-id="aaee0-128">boolean</span><span class="sxs-lookup"><span data-stu-id="aaee0-128">boolean</span></span>|<span data-ttu-id="aaee0-p103">表示该工作表是否受保护。只读。</span><span class="sxs-lookup"><span data-stu-id="aaee0-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aaee0-131">Relationships</span><span class="sxs-lookup"><span data-stu-id="aaee0-131">Relationships</span></span>
<span data-ttu-id="aaee0-132">无。</span><span class="sxs-lookup"><span data-stu-id="aaee0-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aaee0-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aaee0-133">JSON representation</span></span>

<span data-ttu-id="aaee0-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aaee0-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "options"
  ],
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": "boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookWorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
