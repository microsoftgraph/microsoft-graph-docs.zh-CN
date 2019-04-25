---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e9525882b08aaae5500ce23a4b54e95d0b0e0d65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583695"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="5945b-102">SiteCollection 资源</span><span class="sxs-lookup"><span data-stu-id="5945b-102">SiteCollection resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5945b-103">**siteCollection** 资源提供有关网站集的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5945b-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="5945b-104">如果[**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。</span><span class="sxs-lookup"><span data-stu-id="5945b-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5945b-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5945b-105">JSON representation</span></span>

<span data-ttu-id="5945b-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5945b-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "dataLocationCode", "root"
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "dataLocationCode": "EUR",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a><span data-ttu-id="5945b-107">属性</span><span class="sxs-lookup"><span data-stu-id="5945b-107">Properties</span></span>

| <span data-ttu-id="5945b-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="5945b-108">Property name</span></span>        | <span data-ttu-id="5945b-109">类型</span><span class="sxs-lookup"><span data-stu-id="5945b-109">Type</span></span>     | <span data-ttu-id="5945b-110">说明</span><span class="sxs-lookup"><span data-stu-id="5945b-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="5945b-111">**主机名称**</span><span class="sxs-lookup"><span data-stu-id="5945b-111">**hostname**</span></span>         | <span data-ttu-id="5945b-112">string</span><span class="sxs-lookup"><span data-stu-id="5945b-112">string</span></span>   | <span data-ttu-id="5945b-p101">网站集的主机名称。只读。</span><span class="sxs-lookup"><span data-stu-id="5945b-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="5945b-115">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="5945b-115">**dataLocationCode**</span></span> | <span data-ttu-id="5945b-116">string</span><span class="sxs-lookup"><span data-stu-id="5945b-116">string</span></span>   | <span data-ttu-id="5945b-117">此网站集所在位置的地理区域代码。</span><span class="sxs-lookup"><span data-stu-id="5945b-117">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="5945b-118">只读。</span><span class="sxs-lookup"><span data-stu-id="5945b-118">Read-only.</span></span>
| <span data-ttu-id="5945b-119">**根**</span><span class="sxs-lookup"><span data-stu-id="5945b-119">**root**</span></span>             | <span data-ttu-id="5945b-120">[根][]</span><span class="sxs-lookup"><span data-stu-id="5945b-120">[root][]</span></span> | <span data-ttu-id="5945b-121">如果存在, 则表示这是 SharePoint 中的根网站集。</span><span class="sxs-lookup"><span data-stu-id="5945b-121">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="5945b-122">只读。</span><span class="sxs-lookup"><span data-stu-id="5945b-122">Read-only.</span></span>

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sitecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
