---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.openlocfilehash: c366c39a71e952521425d9eb08fab7c77a9a3415
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809980"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="a16f4-102">SiteCollection 资源</span><span class="sxs-lookup"><span data-stu-id="a16f4-102">SiteCollection resource</span></span>

<span data-ttu-id="a16f4-103">**siteCollection** 资源提供有关网站集的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a16f4-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="a16f4-104">如果[**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。</span><span class="sxs-lookup"><span data-stu-id="a16f4-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a16f4-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a16f4-105">JSON representation</span></span>

<span data-ttu-id="a16f4-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a16f4-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a><span data-ttu-id="a16f4-107">属性</span><span class="sxs-lookup"><span data-stu-id="a16f4-107">Properties</span></span>

| <span data-ttu-id="a16f4-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="a16f4-108">Property name</span></span>        | <span data-ttu-id="a16f4-109">类型</span><span class="sxs-lookup"><span data-stu-id="a16f4-109">Type</span></span>     | <span data-ttu-id="a16f4-110">说明</span><span class="sxs-lookup"><span data-stu-id="a16f4-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="a16f4-111">**主机名称**</span><span class="sxs-lookup"><span data-stu-id="a16f4-111">**hostname**</span></span>         | <span data-ttu-id="a16f4-112">string</span><span class="sxs-lookup"><span data-stu-id="a16f4-112">string</span></span>   | <span data-ttu-id="a16f4-p101">网站集的主机名称。只读。</span><span class="sxs-lookup"><span data-stu-id="a16f4-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="a16f4-115">**根**</span><span class="sxs-lookup"><span data-stu-id="a16f4-115">**root**</span></span>             | <span data-ttu-id="a16f4-116">[根][]</span><span class="sxs-lookup"><span data-stu-id="a16f4-116">[root][]</span></span> | <span data-ttu-id="a16f4-117">如果存在此参数，指示这是 SharePoint 中的根网站集。</span><span class="sxs-lookup"><span data-stu-id="a16f4-117">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="a16f4-118">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="a16f4-118">Read-only.</span></span>

[根]: root.md
[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Facets/SiteCollection"
}-->
