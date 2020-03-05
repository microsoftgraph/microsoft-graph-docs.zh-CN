---
title: workbookWorksheetProtection 资源类型
description: 表示对工作表对象的保护。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ab5d3101b1b9cabf8843d3726f036de74bf3a258
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519097"
---
# <a name="workbookworksheetprotection-resource-type"></a><span data-ttu-id="4ca95-103">workbookWorksheetProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ca95-103">workbookWorksheetProtection resource type</span></span>

<span data-ttu-id="4ca95-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4ca95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ca95-105">表示对工作表对象的保护。</span><span class="sxs-lookup"><span data-stu-id="4ca95-105">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="4ca95-106">方法</span><span class="sxs-lookup"><span data-stu-id="4ca95-106">Methods</span></span>

| <span data-ttu-id="4ca95-107">方法</span><span class="sxs-lookup"><span data-stu-id="4ca95-107">Method</span></span>           | <span data-ttu-id="4ca95-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4ca95-108">Return Type</span></span>    |<span data-ttu-id="4ca95-109">说明</span><span class="sxs-lookup"><span data-stu-id="4ca95-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4ca95-110">获取 workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="4ca95-110">Get workbookWorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="4ca95-111">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="4ca95-111">workbookWorksheetProtection</span></span>](workbookworksheetprotection.md) |<span data-ttu-id="4ca95-112">读取 workbookWorksheetProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4ca95-112">Read properties and relationships of workbookWorksheetProtection object.</span></span>|
|[<span data-ttu-id="4ca95-113">保护</span><span class="sxs-lookup"><span data-stu-id="4ca95-113">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="4ca95-114">无</span><span class="sxs-lookup"><span data-stu-id="4ca95-114">None</span></span>|<span data-ttu-id="4ca95-p101">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="4ca95-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="4ca95-117">解除保护</span><span class="sxs-lookup"><span data-stu-id="4ca95-117">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="4ca95-118">无</span><span class="sxs-lookup"><span data-stu-id="4ca95-118">None</span></span>|<span data-ttu-id="4ca95-119">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="4ca95-119">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="4ca95-120">属性</span><span class="sxs-lookup"><span data-stu-id="4ca95-120">Properties</span></span>
| <span data-ttu-id="4ca95-121">属性</span><span class="sxs-lookup"><span data-stu-id="4ca95-121">Property</span></span>     | <span data-ttu-id="4ca95-122">类型</span><span class="sxs-lookup"><span data-stu-id="4ca95-122">Type</span></span>   |<span data-ttu-id="4ca95-123">说明</span><span class="sxs-lookup"><span data-stu-id="4ca95-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ca95-124">选项</span><span class="sxs-lookup"><span data-stu-id="4ca95-124">options</span></span>|[<span data-ttu-id="4ca95-125">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="4ca95-125">workbookWorksheetProtectionOptions</span></span>](workbookworksheetprotectionoptions.md)|<span data-ttu-id="4ca95-126">工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="4ca95-126">Sheet protection options.</span></span> <span data-ttu-id="4ca95-127">只读。</span><span class="sxs-lookup"><span data-stu-id="4ca95-127">Read-only.</span></span>|
|<span data-ttu-id="4ca95-128">protected</span><span class="sxs-lookup"><span data-stu-id="4ca95-128">protected</span></span>|<span data-ttu-id="4ca95-129">boolean</span><span class="sxs-lookup"><span data-stu-id="4ca95-129">boolean</span></span>|<span data-ttu-id="4ca95-p103">表示该工作表是否受保护。只读。</span><span class="sxs-lookup"><span data-stu-id="4ca95-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ca95-132">关系</span><span class="sxs-lookup"><span data-stu-id="4ca95-132">Relationships</span></span>
<span data-ttu-id="4ca95-133">无。</span><span class="sxs-lookup"><span data-stu-id="4ca95-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ca95-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ca95-134">JSON representation</span></span>

<span data-ttu-id="4ca95-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ca95-135">Here is a JSON representation of the resource.</span></span>

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
