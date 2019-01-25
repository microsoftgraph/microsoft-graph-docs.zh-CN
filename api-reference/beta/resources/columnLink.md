---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: d5b1d068202057bc6a07982d04ff77b6bf07f028
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511861"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="dc3f9-102">ColumnLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc3f9-102">ColumnLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc3f9-103">[contentType][] 上的 **columnLink** 将网站 **columnDefinition** 附加到该内容类型。</span><span class="sxs-lookup"><span data-stu-id="dc3f9-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="dc3f9-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc3f9-105">JSON representation</span></span>

<span data-ttu-id="dc3f9-106">下面是 **columnLink** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc3f9-106">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="dc3f9-107">属性</span><span class="sxs-lookup"><span data-stu-id="dc3f9-107">Properties</span></span>

| <span data-ttu-id="dc3f9-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="dc3f9-108">Property name</span></span> | <span data-ttu-id="dc3f9-109">类型</span><span class="sxs-lookup"><span data-stu-id="dc3f9-109">Type</span></span>   | <span data-ttu-id="dc3f9-110">说明</span><span class="sxs-lookup"><span data-stu-id="dc3f9-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="dc3f9-111">**id**</span><span class="sxs-lookup"><span data-stu-id="dc3f9-111">**id**</span></span>        | <span data-ttu-id="dc3f9-112">string</span><span class="sxs-lookup"><span data-stu-id="dc3f9-112">string</span></span> | <span data-ttu-id="dc3f9-113">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dc3f9-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="dc3f9-114">**name**</span><span class="sxs-lookup"><span data-stu-id="dc3f9-114">**name**</span></span>      | <span data-ttu-id="dc3f9-115">string</span><span class="sxs-lookup"><span data-stu-id="dc3f9-115">string</span></span> | <span data-ttu-id="dc3f9-116">此内容类型中的列的名称。</span><span class="sxs-lookup"><span data-stu-id="dc3f9-116">The name of the column  in this content type.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink",
  "suppressions": [
    "Error: /api-reference/beta/resources/columnLink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
