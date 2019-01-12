---
title: WorksheetProtection 资源类型
description: 表示对 sheet 对象的保护。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5b9faed56e545698cb731728b2c95fd31682b252
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916990"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="39499-103">WorksheetProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="39499-103">WorksheetProtection resource type</span></span>

> <span data-ttu-id="39499-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="39499-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39499-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="39499-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="39499-106">表示对 sheet 对象的保护。</span><span class="sxs-lookup"><span data-stu-id="39499-106">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="39499-107">方法</span><span class="sxs-lookup"><span data-stu-id="39499-107">Methods</span></span>

| <span data-ttu-id="39499-108">方法</span><span class="sxs-lookup"><span data-stu-id="39499-108">Method</span></span>           | <span data-ttu-id="39499-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="39499-109">Return Type</span></span>    |<span data-ttu-id="39499-110">说明</span><span class="sxs-lookup"><span data-stu-id="39499-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="39499-111">获取 WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="39499-111">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="39499-112">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="39499-112">WorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="39499-113">读取 worksheetProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="39499-113">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="39499-114">Protect</span><span class="sxs-lookup"><span data-stu-id="39499-114">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="39499-115">无</span><span class="sxs-lookup"><span data-stu-id="39499-115">None</span></span>|<span data-ttu-id="39499-p102">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="39499-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="39499-118">Unprotect</span><span class="sxs-lookup"><span data-stu-id="39499-118">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="39499-119">无</span><span class="sxs-lookup"><span data-stu-id="39499-119">None</span></span>|<span data-ttu-id="39499-120">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="39499-120">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="39499-121">属性</span><span class="sxs-lookup"><span data-stu-id="39499-121">Properties</span></span>
| <span data-ttu-id="39499-122">属性</span><span class="sxs-lookup"><span data-stu-id="39499-122">Property</span></span>     | <span data-ttu-id="39499-123">类型</span><span class="sxs-lookup"><span data-stu-id="39499-123">Type</span></span>   |<span data-ttu-id="39499-124">说明</span><span class="sxs-lookup"><span data-stu-id="39499-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39499-125">protected</span><span class="sxs-lookup"><span data-stu-id="39499-125">protected</span></span>|<span data-ttu-id="39499-126">boolean</span><span class="sxs-lookup"><span data-stu-id="39499-126">boolean</span></span>|<span data-ttu-id="39499-p103">表示该工作表是否受保护。只读。</span><span class="sxs-lookup"><span data-stu-id="39499-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39499-129">Relationships</span><span class="sxs-lookup"><span data-stu-id="39499-129">Relationships</span></span>
| <span data-ttu-id="39499-130">关系</span><span class="sxs-lookup"><span data-stu-id="39499-130">Relationship</span></span> | <span data-ttu-id="39499-131">类型</span><span class="sxs-lookup"><span data-stu-id="39499-131">Type</span></span>   |<span data-ttu-id="39499-132">说明</span><span class="sxs-lookup"><span data-stu-id="39499-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39499-133">选项</span><span class="sxs-lookup"><span data-stu-id="39499-133">options</span></span>|[<span data-ttu-id="39499-134">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="39499-134">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="39499-p104">工作表保护选项。只读。</span><span class="sxs-lookup"><span data-stu-id="39499-p104">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39499-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39499-137">JSON representation</span></span>

<span data-ttu-id="39499-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39499-138">Here is a JSON representation of the resource.</span></span>

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
