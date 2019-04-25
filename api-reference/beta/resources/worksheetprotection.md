---
title: WorksheetProtection 资源类型
description: 表示对工作表对象的保护。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7e87edcebae95f32ce0bccaf849a7d21140f4878
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523800"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="42d0e-103">WorksheetProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="42d0e-103">WorksheetProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42d0e-104">表示对工作表对象的保护。</span><span class="sxs-lookup"><span data-stu-id="42d0e-104">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="42d0e-105">方法</span><span class="sxs-lookup"><span data-stu-id="42d0e-105">Methods</span></span>

| <span data-ttu-id="42d0e-106">方法</span><span class="sxs-lookup"><span data-stu-id="42d0e-106">Method</span></span>           | <span data-ttu-id="42d0e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="42d0e-107">Return Type</span></span>    |<span data-ttu-id="42d0e-108">说明</span><span class="sxs-lookup"><span data-stu-id="42d0e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="42d0e-109">获取 WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="42d0e-109">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="42d0e-110">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="42d0e-110">WorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="42d0e-111">读取 worksheetProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="42d0e-111">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="42d0e-112">保护</span><span class="sxs-lookup"><span data-stu-id="42d0e-112">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="42d0e-113">无</span><span class="sxs-lookup"><span data-stu-id="42d0e-113">None</span></span>|<span data-ttu-id="42d0e-p101">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="42d0e-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="42d0e-116">解除保护</span><span class="sxs-lookup"><span data-stu-id="42d0e-116">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="42d0e-117">无</span><span class="sxs-lookup"><span data-stu-id="42d0e-117">None</span></span>|<span data-ttu-id="42d0e-118">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="42d0e-118">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="42d0e-119">属性</span><span class="sxs-lookup"><span data-stu-id="42d0e-119">Properties</span></span>
| <span data-ttu-id="42d0e-120">属性</span><span class="sxs-lookup"><span data-stu-id="42d0e-120">Property</span></span>     | <span data-ttu-id="42d0e-121">类型</span><span class="sxs-lookup"><span data-stu-id="42d0e-121">Type</span></span>   |<span data-ttu-id="42d0e-122">说明</span><span class="sxs-lookup"><span data-stu-id="42d0e-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42d0e-123">protected</span><span class="sxs-lookup"><span data-stu-id="42d0e-123">protected</span></span>|<span data-ttu-id="42d0e-124">boolean</span><span class="sxs-lookup"><span data-stu-id="42d0e-124">boolean</span></span>|<span data-ttu-id="42d0e-p102">表示该工作表是否受保护。只读。</span><span class="sxs-lookup"><span data-stu-id="42d0e-p102">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42d0e-127">关系</span><span class="sxs-lookup"><span data-stu-id="42d0e-127">Relationships</span></span>
| <span data-ttu-id="42d0e-128">关系</span><span class="sxs-lookup"><span data-stu-id="42d0e-128">Relationship</span></span> | <span data-ttu-id="42d0e-129">类型</span><span class="sxs-lookup"><span data-stu-id="42d0e-129">Type</span></span>   |<span data-ttu-id="42d0e-130">说明</span><span class="sxs-lookup"><span data-stu-id="42d0e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42d0e-131">选项</span><span class="sxs-lookup"><span data-stu-id="42d0e-131">options</span></span>|[<span data-ttu-id="42d0e-132">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="42d0e-132">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="42d0e-p103">工作表保护选项。只读。</span><span class="sxs-lookup"><span data-stu-id="42d0e-p103">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42d0e-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42d0e-135">JSON representation</span></span>

<span data-ttu-id="42d0e-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42d0e-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtection"
}-->

```json
{
  "protected": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheetprotection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
