---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 006f239acdecb2fb93ecf1d70e25a42b056b9283
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480192"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="c3ac9-102">SiteCollection 资源</span><span class="sxs-lookup"><span data-stu-id="c3ac9-102">SiteCollection resource</span></span>

<span data-ttu-id="c3ac9-103">**siteCollection** 资源提供有关网站集的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c3ac9-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="c3ac9-104">如果[**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。</span><span class="sxs-lookup"><span data-stu-id="c3ac9-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3ac9-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3ac9-105">JSON representation</span></span>

<span data-ttu-id="c3ac9-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3ac9-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c3ac9-107">属性</span><span class="sxs-lookup"><span data-stu-id="c3ac9-107">Properties</span></span>

| <span data-ttu-id="c3ac9-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="c3ac9-108">Property name</span></span>        | <span data-ttu-id="c3ac9-109">类型</span><span class="sxs-lookup"><span data-stu-id="c3ac9-109">Type</span></span>     | <span data-ttu-id="c3ac9-110">说明</span><span class="sxs-lookup"><span data-stu-id="c3ac9-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="c3ac9-111">**主机名称**</span><span class="sxs-lookup"><span data-stu-id="c3ac9-111">**hostname**</span></span>         | <span data-ttu-id="c3ac9-112">string</span><span class="sxs-lookup"><span data-stu-id="c3ac9-112">string</span></span>   | <span data-ttu-id="c3ac9-p101">网站集的主机名称。只读。</span><span class="sxs-lookup"><span data-stu-id="c3ac9-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="c3ac9-115">**根**</span><span class="sxs-lookup"><span data-stu-id="c3ac9-115">**root**</span></span>             | <span data-ttu-id="c3ac9-116">[root][]</span><span class="sxs-lookup"><span data-stu-id="c3ac9-116">[root][]</span></span> | <span data-ttu-id="c3ac9-117">如果存在, 则表示这是 SharePoint 中的根网站集。</span><span class="sxs-lookup"><span data-stu-id="c3ac9-117">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="c3ac9-118">只读。</span><span class="sxs-lookup"><span data-stu-id="c3ac9-118">Read-only.</span></span>

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
