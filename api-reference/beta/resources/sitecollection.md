---
author: JeremyKelley
description: siteCollection 资源提供有关网站集的详细信息。
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0989306be8fa8e456d2718079aec069097cab035
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008290"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="e4098-103">SiteCollection 资源</span><span class="sxs-lookup"><span data-stu-id="e4098-103">SiteCollection resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4098-104">**siteCollection** 资源提供有关网站集的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e4098-104">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="e4098-105">如果[**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。</span><span class="sxs-lookup"><span data-stu-id="e4098-105">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4098-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4098-106">JSON representation</span></span>

<span data-ttu-id="e4098-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4098-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="e4098-108">属性</span><span class="sxs-lookup"><span data-stu-id="e4098-108">Properties</span></span>

| <span data-ttu-id="e4098-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="e4098-109">Property name</span></span>        | <span data-ttu-id="e4098-110">类型</span><span class="sxs-lookup"><span data-stu-id="e4098-110">Type</span></span>     | <span data-ttu-id="e4098-111">说明</span><span class="sxs-lookup"><span data-stu-id="e4098-111">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="e4098-112">**主机名称**</span><span class="sxs-lookup"><span data-stu-id="e4098-112">**hostname**</span></span>         | <span data-ttu-id="e4098-113">string</span><span class="sxs-lookup"><span data-stu-id="e4098-113">string</span></span>   | <span data-ttu-id="e4098-p101">网站集的主机名称。只读。</span><span class="sxs-lookup"><span data-stu-id="e4098-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="e4098-116">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="e4098-116">**dataLocationCode**</span></span> | <span data-ttu-id="e4098-117">string</span><span class="sxs-lookup"><span data-stu-id="e4098-117">string</span></span>   | <span data-ttu-id="e4098-118">此网站集所在位置的地理区域代码。</span><span class="sxs-lookup"><span data-stu-id="e4098-118">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="e4098-119">只读。</span><span class="sxs-lookup"><span data-stu-id="e4098-119">Read-only.</span></span>
| <span data-ttu-id="e4098-120">**根**</span><span class="sxs-lookup"><span data-stu-id="e4098-120">**root**</span></span>             | <span data-ttu-id="e4098-121">[根][]</span><span class="sxs-lookup"><span data-stu-id="e4098-121">[root][]</span></span> | <span data-ttu-id="e4098-122">如果存在, 则表示这是 SharePoint 中的根网站集。</span><span class="sxs-lookup"><span data-stu-id="e4098-122">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="e4098-123">只读。</span><span class="sxs-lookup"><span data-stu-id="e4098-123">Read-only.</span></span>

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
  "suppressions": []
}
-->
