---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 6fb5f05a1dbdf7485957bb4bf04db06432f17da4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916983"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="3352a-102">SiteCollection 资源</span><span class="sxs-lookup"><span data-stu-id="3352a-102">SiteCollection resource</span></span>

<span data-ttu-id="3352a-103">**siteCollection** 资源提供有关网站集的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3352a-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="3352a-104">如果[**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。</span><span class="sxs-lookup"><span data-stu-id="3352a-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3352a-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3352a-105">JSON representation</span></span>

<span data-ttu-id="3352a-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3352a-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3352a-107">属性</span><span class="sxs-lookup"><span data-stu-id="3352a-107">Properties</span></span>

| <span data-ttu-id="3352a-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="3352a-108">Property name</span></span>        | <span data-ttu-id="3352a-109">类型</span><span class="sxs-lookup"><span data-stu-id="3352a-109">Type</span></span>     | <span data-ttu-id="3352a-110">说明</span><span class="sxs-lookup"><span data-stu-id="3352a-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="3352a-111">**主机名称**</span><span class="sxs-lookup"><span data-stu-id="3352a-111">**hostname**</span></span>         | <span data-ttu-id="3352a-112">string</span><span class="sxs-lookup"><span data-stu-id="3352a-112">string</span></span>   | <span data-ttu-id="3352a-p101">网站集的主机名称。只读。</span><span class="sxs-lookup"><span data-stu-id="3352a-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="3352a-115">**根**</span><span class="sxs-lookup"><span data-stu-id="3352a-115">**root**</span></span>             | <span data-ttu-id="3352a-116">[根][]</span><span class="sxs-lookup"><span data-stu-id="3352a-116">[root][]</span></span> | <span data-ttu-id="3352a-117">如果存在此参数，指示这是 SharePoint 中的根网站集。</span><span class="sxs-lookup"><span data-stu-id="3352a-117">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="3352a-118">只读。</span><span class="sxs-lookup"><span data-stu-id="3352a-118">Read-only.</span></span>

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
