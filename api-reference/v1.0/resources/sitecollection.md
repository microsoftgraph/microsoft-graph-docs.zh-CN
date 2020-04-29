---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
description: siteCollection 资源提供有关网站集的详细信息。
doc_type: resourcePageType
ms.openlocfilehash: f73505ead4ad060f81bdfe7e77099783a8ff0242
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2020
ms.locfileid: "43934820"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="68761-103">SiteCollection 资源</span><span class="sxs-lookup"><span data-stu-id="68761-103">SiteCollection resource</span></span>

<span data-ttu-id="68761-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68761-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68761-105">**siteCollection** 资源提供有关网站集的详细信息。</span><span class="sxs-lookup"><span data-stu-id="68761-105">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="68761-106">如果[**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。</span><span class="sxs-lookup"><span data-stu-id="68761-106">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="68761-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68761-107">JSON representation</span></span>

<span data-ttu-id="68761-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68761-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
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

## <a name="properties"></a><span data-ttu-id="68761-109">属性</span><span class="sxs-lookup"><span data-stu-id="68761-109">Properties</span></span>

| <span data-ttu-id="68761-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="68761-110">Property name</span></span>        | <span data-ttu-id="68761-111">类型</span><span class="sxs-lookup"><span data-stu-id="68761-111">Type</span></span>     | <span data-ttu-id="68761-112">说明</span><span class="sxs-lookup"><span data-stu-id="68761-112">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="68761-113">**主机名称**</span><span class="sxs-lookup"><span data-stu-id="68761-113">**hostname**</span></span>         | <span data-ttu-id="68761-114">string</span><span class="sxs-lookup"><span data-stu-id="68761-114">string</span></span>   | <span data-ttu-id="68761-p101">网站集的主机名称。只读。</span><span class="sxs-lookup"><span data-stu-id="68761-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="68761-117">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="68761-117">**dataLocationCode**</span></span> | <span data-ttu-id="68761-118">string</span><span class="sxs-lookup"><span data-stu-id="68761-118">string</span></span>   | <span data-ttu-id="68761-119">此网站集所在位置的地理区域代码。</span><span class="sxs-lookup"><span data-stu-id="68761-119">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="68761-120">只读。</span><span class="sxs-lookup"><span data-stu-id="68761-120">Read-only.</span></span>
| <span data-ttu-id="68761-121">**根**</span><span class="sxs-lookup"><span data-stu-id="68761-121">**root**</span></span>             | <span data-ttu-id="68761-122">[根][]</span><span class="sxs-lookup"><span data-stu-id="68761-122">[root][]</span></span> | <span data-ttu-id="68761-123">如果存在，则表示这是 SharePoint 中的根网站集。</span><span class="sxs-lookup"><span data-stu-id="68761-123">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="68761-124">只读。</span><span class="sxs-lookup"><span data-stu-id="68761-124">Read-only.</span></span>

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
