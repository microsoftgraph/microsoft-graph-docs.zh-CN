---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: 98f7b9d930ccf7f1f0e1a6a0e1ad0353d49cf2bf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009835"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="313b8-102">SiteCollection 资源</span><span class="sxs-lookup"><span data-stu-id="313b8-102">SiteCollection resource</span></span>

<span data-ttu-id="313b8-103">**siteCollection** 资源提供有关网站集的详细信息。</span><span class="sxs-lookup"><span data-stu-id="313b8-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="313b8-104">如果[**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。</span><span class="sxs-lookup"><span data-stu-id="313b8-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="313b8-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="313b8-105">JSON representation</span></span>

<span data-ttu-id="313b8-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="313b8-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="313b8-107">属性</span><span class="sxs-lookup"><span data-stu-id="313b8-107">Properties</span></span>

| <span data-ttu-id="313b8-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="313b8-108">Property name</span></span>        | <span data-ttu-id="313b8-109">类型</span><span class="sxs-lookup"><span data-stu-id="313b8-109">Type</span></span>     | <span data-ttu-id="313b8-110">说明</span><span class="sxs-lookup"><span data-stu-id="313b8-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="313b8-111">**主机名称**</span><span class="sxs-lookup"><span data-stu-id="313b8-111">**hostname**</span></span>         | <span data-ttu-id="313b8-112">string</span><span class="sxs-lookup"><span data-stu-id="313b8-112">string</span></span>   | <span data-ttu-id="313b8-p101">网站集的主机名称。只读。</span><span class="sxs-lookup"><span data-stu-id="313b8-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="313b8-115">**根**</span><span class="sxs-lookup"><span data-stu-id="313b8-115">**root**</span></span>             | <span data-ttu-id="313b8-116">[根][]</span><span class="sxs-lookup"><span data-stu-id="313b8-116">[root][]</span></span> | <span data-ttu-id="313b8-117">如果存在此参数，指示这是 SharePoint 中的根网站集。</span><span class="sxs-lookup"><span data-stu-id="313b8-117">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="313b8-118">只读。</span><span class="sxs-lookup"><span data-stu-id="313b8-118">Read-only.</span></span>

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
