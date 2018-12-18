---
title: WorksheetProtection 资源类型
description: 表示对 sheet 对象的保护。
author: lumine2008
ms.openlocfilehash: 91415b067fbe54333e32d1a2ed84bce5025b7d3a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339205"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="e8c98-103">WorksheetProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8c98-103">WorksheetProtection resource type</span></span>

> <span data-ttu-id="e8c98-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e8c98-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8c98-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e8c98-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8c98-106">表示对 sheet 对象的保护。</span><span class="sxs-lookup"><span data-stu-id="e8c98-106">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="e8c98-107">方法</span><span class="sxs-lookup"><span data-stu-id="e8c98-107">Methods</span></span>

| <span data-ttu-id="e8c98-108">方法</span><span class="sxs-lookup"><span data-stu-id="e8c98-108">Method</span></span>           | <span data-ttu-id="e8c98-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e8c98-109">Return Type</span></span>    |<span data-ttu-id="e8c98-110">说明</span><span class="sxs-lookup"><span data-stu-id="e8c98-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e8c98-111">获取 WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="e8c98-111">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="e8c98-112">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="e8c98-112">WorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="e8c98-113">读取 worksheetProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e8c98-113">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="e8c98-114">Protect</span><span class="sxs-lookup"><span data-stu-id="e8c98-114">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="e8c98-115">无</span><span class="sxs-lookup"><span data-stu-id="e8c98-115">None</span></span>|<span data-ttu-id="e8c98-p102">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="e8c98-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="e8c98-118">Unprotect</span><span class="sxs-lookup"><span data-stu-id="e8c98-118">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="e8c98-119">无</span><span class="sxs-lookup"><span data-stu-id="e8c98-119">None</span></span>|<span data-ttu-id="e8c98-120">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="e8c98-120">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="e8c98-121">属性</span><span class="sxs-lookup"><span data-stu-id="e8c98-121">Properties</span></span>
| <span data-ttu-id="e8c98-122">属性</span><span class="sxs-lookup"><span data-stu-id="e8c98-122">Property</span></span>     | <span data-ttu-id="e8c98-123">类型</span><span class="sxs-lookup"><span data-stu-id="e8c98-123">Type</span></span>   |<span data-ttu-id="e8c98-124">说明</span><span class="sxs-lookup"><span data-stu-id="e8c98-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8c98-125">protected</span><span class="sxs-lookup"><span data-stu-id="e8c98-125">protected</span></span>|<span data-ttu-id="e8c98-126">boolean</span><span class="sxs-lookup"><span data-stu-id="e8c98-126">boolean</span></span>|<span data-ttu-id="e8c98-p103">表示该工作表是否受保护。只读。</span><span class="sxs-lookup"><span data-stu-id="e8c98-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8c98-129">Relationships</span><span class="sxs-lookup"><span data-stu-id="e8c98-129">Relationships</span></span>
| <span data-ttu-id="e8c98-130">关系</span><span class="sxs-lookup"><span data-stu-id="e8c98-130">Relationship</span></span> | <span data-ttu-id="e8c98-131">类型</span><span class="sxs-lookup"><span data-stu-id="e8c98-131">Type</span></span>   |<span data-ttu-id="e8c98-132">说明</span><span class="sxs-lookup"><span data-stu-id="e8c98-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8c98-133">选项</span><span class="sxs-lookup"><span data-stu-id="e8c98-133">options</span></span>|[<span data-ttu-id="e8c98-134">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="e8c98-134">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="e8c98-p104">工作表保护选项。只读。</span><span class="sxs-lookup"><span data-stu-id="e8c98-p104">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8c98-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8c98-137">JSON representation</span></span>

<span data-ttu-id="e8c98-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8c98-138">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->