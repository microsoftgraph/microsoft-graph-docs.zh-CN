---
title: workbookWorksheetProtection 资源类型
description: 表示对工作表对象的保护。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ed6f52074836368eade8851ea32f1e8ef64e493e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007037"
---
# <a name="workbookworksheetprotection-resource-type"></a><span data-ttu-id="5cc8f-103">workbookWorksheetProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="5cc8f-103">workbookWorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cc8f-104">表示对工作表对象的保护。</span><span class="sxs-lookup"><span data-stu-id="5cc8f-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="5cc8f-105">方法</span><span class="sxs-lookup"><span data-stu-id="5cc8f-105">Methods</span></span>

| <span data-ttu-id="5cc8f-106">方法</span><span class="sxs-lookup"><span data-stu-id="5cc8f-106">Method</span></span>           | <span data-ttu-id="5cc8f-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="5cc8f-107">Return Type</span></span>    |<span data-ttu-id="5cc8f-108">说明</span><span class="sxs-lookup"><span data-stu-id="5cc8f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5cc8f-109">获取 workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="5cc8f-109">Get workbookWorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="5cc8f-110">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="5cc8f-110">workbookWorksheetProtection</span></span>](workbookworksheetprotection.md) |<span data-ttu-id="5cc8f-111">读取 workbookWorksheetProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5cc8f-111">Read properties and relationships of workbookWorksheetProtection object.</span></span>|
|[<span data-ttu-id="5cc8f-112">保护</span><span class="sxs-lookup"><span data-stu-id="5cc8f-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="5cc8f-113">无</span><span class="sxs-lookup"><span data-stu-id="5cc8f-113">None</span></span>|<span data-ttu-id="5cc8f-p101">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="5cc8f-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="5cc8f-116">解除保护</span><span class="sxs-lookup"><span data-stu-id="5cc8f-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="5cc8f-117">无</span><span class="sxs-lookup"><span data-stu-id="5cc8f-117">None</span></span>|<span data-ttu-id="5cc8f-118">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="5cc8f-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="5cc8f-119">属性</span><span class="sxs-lookup"><span data-stu-id="5cc8f-119">Properties</span></span>
| <span data-ttu-id="5cc8f-120">属性</span><span class="sxs-lookup"><span data-stu-id="5cc8f-120">Property</span></span>     | <span data-ttu-id="5cc8f-121">类型</span><span class="sxs-lookup"><span data-stu-id="5cc8f-121">Type</span></span>   |<span data-ttu-id="5cc8f-122">说明</span><span class="sxs-lookup"><span data-stu-id="5cc8f-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cc8f-123">选项</span><span class="sxs-lookup"><span data-stu-id="5cc8f-123">options</span></span>|[<span data-ttu-id="5cc8f-124">workbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="5cc8f-124">workbookWorksheetProtectionOptions</span></span>](workbookworksheetprotectionoptions.md)|<span data-ttu-id="5cc8f-125">工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="5cc8f-125">Sheet protection options.</span></span> <span data-ttu-id="5cc8f-126">只读。</span><span class="sxs-lookup"><span data-stu-id="5cc8f-126">Read-only.</span></span>|
|<span data-ttu-id="5cc8f-127">protected</span><span class="sxs-lookup"><span data-stu-id="5cc8f-127">protected</span></span>|<span data-ttu-id="5cc8f-128">boolean</span><span class="sxs-lookup"><span data-stu-id="5cc8f-128">boolean</span></span>|<span data-ttu-id="5cc8f-p103">表示该工作表是否受保护。只读。</span><span class="sxs-lookup"><span data-stu-id="5cc8f-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cc8f-131">关系</span><span class="sxs-lookup"><span data-stu-id="5cc8f-131">Relationships</span></span>
<span data-ttu-id="5cc8f-132">无。</span><span class="sxs-lookup"><span data-stu-id="5cc8f-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cc8f-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5cc8f-133">JSON representation</span></span>

<span data-ttu-id="5cc8f-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cc8f-134">Here is a JSON representation of the resource.</span></span>

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
