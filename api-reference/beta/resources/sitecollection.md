---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 865fc21691eb37811300caaf675b123d1a544ac0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528128"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="64e52-102">SiteCollection 资源</span><span class="sxs-lookup"><span data-stu-id="64e52-102">SiteCollection resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64e52-103">**siteCollection** 资源提供有关网站集的详细信息。</span><span class="sxs-lookup"><span data-stu-id="64e52-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="64e52-104">如果[**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。</span><span class="sxs-lookup"><span data-stu-id="64e52-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="64e52-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64e52-105">JSON representation</span></span>

<span data-ttu-id="64e52-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64e52-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="64e52-107">属性</span><span class="sxs-lookup"><span data-stu-id="64e52-107">Properties</span></span>

| <span data-ttu-id="64e52-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="64e52-108">Property name</span></span>        | <span data-ttu-id="64e52-109">类型</span><span class="sxs-lookup"><span data-stu-id="64e52-109">Type</span></span>     | <span data-ttu-id="64e52-110">说明</span><span class="sxs-lookup"><span data-stu-id="64e52-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="64e52-111">**主机名称**</span><span class="sxs-lookup"><span data-stu-id="64e52-111">**hostname**</span></span>         | <span data-ttu-id="64e52-112">string</span><span class="sxs-lookup"><span data-stu-id="64e52-112">string</span></span>   | <span data-ttu-id="64e52-p101">网站集的主机名称。只读。</span><span class="sxs-lookup"><span data-stu-id="64e52-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="64e52-115">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="64e52-115">**dataLocationCode**</span></span> | <span data-ttu-id="64e52-116">string</span><span class="sxs-lookup"><span data-stu-id="64e52-116">string</span></span>   | <span data-ttu-id="64e52-117">地理区域代码为此网站集所在的位置。</span><span class="sxs-lookup"><span data-stu-id="64e52-117">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="64e52-118">只读。</span><span class="sxs-lookup"><span data-stu-id="64e52-118">Read-only.</span></span>
| <span data-ttu-id="64e52-119">**根**</span><span class="sxs-lookup"><span data-stu-id="64e52-119">**root**</span></span>             | <span data-ttu-id="64e52-120">[root][]</span><span class="sxs-lookup"><span data-stu-id="64e52-120">[root][]</span></span> | <span data-ttu-id="64e52-121">如果存在此参数，指示这是 SharePoint 中的根网站集。</span><span class="sxs-lookup"><span data-stu-id="64e52-121">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="64e52-122">只读。</span><span class="sxs-lookup"><span data-stu-id="64e52-122">Read-only.</span></span>

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
