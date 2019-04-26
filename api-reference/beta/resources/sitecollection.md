---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 6dc6b5198e85f43609bb0c878439a1d0d5a22a11
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343066"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="07dcd-102">SiteCollection 资源</span><span class="sxs-lookup"><span data-stu-id="07dcd-102">SiteCollection resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07dcd-103">**siteCollection** 资源提供有关网站集的详细信息。</span><span class="sxs-lookup"><span data-stu-id="07dcd-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="07dcd-104">如果[**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。</span><span class="sxs-lookup"><span data-stu-id="07dcd-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07dcd-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07dcd-105">JSON representation</span></span>

<span data-ttu-id="07dcd-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07dcd-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="07dcd-107">属性</span><span class="sxs-lookup"><span data-stu-id="07dcd-107">Properties</span></span>

| <span data-ttu-id="07dcd-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="07dcd-108">Property name</span></span>        | <span data-ttu-id="07dcd-109">类型</span><span class="sxs-lookup"><span data-stu-id="07dcd-109">Type</span></span>     | <span data-ttu-id="07dcd-110">说明</span><span class="sxs-lookup"><span data-stu-id="07dcd-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="07dcd-111">**主机名称**</span><span class="sxs-lookup"><span data-stu-id="07dcd-111">**hostname**</span></span>         | <span data-ttu-id="07dcd-112">string</span><span class="sxs-lookup"><span data-stu-id="07dcd-112">string</span></span>   | <span data-ttu-id="07dcd-p101">网站集的主机名称。只读。</span><span class="sxs-lookup"><span data-stu-id="07dcd-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="07dcd-115">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="07dcd-115">**dataLocationCode**</span></span> | <span data-ttu-id="07dcd-116">string</span><span class="sxs-lookup"><span data-stu-id="07dcd-116">string</span></span>   | <span data-ttu-id="07dcd-117">此网站集所在位置的地理区域代码。</span><span class="sxs-lookup"><span data-stu-id="07dcd-117">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="07dcd-118">只读。</span><span class="sxs-lookup"><span data-stu-id="07dcd-118">Read-only.</span></span>
| <span data-ttu-id="07dcd-119">**根**</span><span class="sxs-lookup"><span data-stu-id="07dcd-119">**root**</span></span>             | <span data-ttu-id="07dcd-120">[根][]</span><span class="sxs-lookup"><span data-stu-id="07dcd-120">[root][]</span></span> | <span data-ttu-id="07dcd-121">如果存在, 则表示这是 SharePoint 中的根网站集。</span><span class="sxs-lookup"><span data-stu-id="07dcd-121">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="07dcd-122">只读。</span><span class="sxs-lookup"><span data-stu-id="07dcd-122">Read-only.</span></span>

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
