---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
description: siteCollection 资源提供有关网站集的详细信息。
doc_type: resourcePageType
ms.openlocfilehash: 27a534f2f9afe99a1a5abb1aee91b1b53b29566d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034158"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="31ff8-103">SiteCollection 资源</span><span class="sxs-lookup"><span data-stu-id="31ff8-103">SiteCollection resource</span></span>

<span data-ttu-id="31ff8-104">**siteCollection** 资源提供有关网站集的详细信息。</span><span class="sxs-lookup"><span data-stu-id="31ff8-104">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="31ff8-105">如果[**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。</span><span class="sxs-lookup"><span data-stu-id="31ff8-105">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31ff8-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31ff8-106">JSON representation</span></span>

<span data-ttu-id="31ff8-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31ff8-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="31ff8-108">属性</span><span class="sxs-lookup"><span data-stu-id="31ff8-108">Properties</span></span>

| <span data-ttu-id="31ff8-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="31ff8-109">Property name</span></span>        | <span data-ttu-id="31ff8-110">类型</span><span class="sxs-lookup"><span data-stu-id="31ff8-110">Type</span></span>     | <span data-ttu-id="31ff8-111">说明</span><span class="sxs-lookup"><span data-stu-id="31ff8-111">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="31ff8-112">**主机名称**</span><span class="sxs-lookup"><span data-stu-id="31ff8-112">**hostname**</span></span>         | <span data-ttu-id="31ff8-113">string</span><span class="sxs-lookup"><span data-stu-id="31ff8-113">string</span></span>   | <span data-ttu-id="31ff8-p101">网站集的主机名称。只读。</span><span class="sxs-lookup"><span data-stu-id="31ff8-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="31ff8-116">**根**</span><span class="sxs-lookup"><span data-stu-id="31ff8-116">**root**</span></span>             | <span data-ttu-id="31ff8-117">[根][]</span><span class="sxs-lookup"><span data-stu-id="31ff8-117">[root][]</span></span> | <span data-ttu-id="31ff8-118">如果存在, 则表示这是 SharePoint 中的根网站集。</span><span class="sxs-lookup"><span data-stu-id="31ff8-118">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="31ff8-119">只读。</span><span class="sxs-lookup"><span data-stu-id="31ff8-119">Read-only.</span></span>

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
