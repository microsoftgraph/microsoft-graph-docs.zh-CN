---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: 84de2a8aa6796051b3b11ebec0d0f8f5934ea1fc
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "19069341"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="154d1-102">SiteCollection 资源</span><span class="sxs-lookup"><span data-stu-id="154d1-102">SiteCollection resource</span></span>

<span data-ttu-id="154d1-103">**siteCollection** 资源提供有关网站集的详细信息。</span><span class="sxs-lookup"><span data-stu-id="154d1-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="154d1-104">如果[**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。</span><span class="sxs-lookup"><span data-stu-id="154d1-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="154d1-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="154d1-105">JSON representation</span></span>

<span data-ttu-id="154d1-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="154d1-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="154d1-107">属性</span><span class="sxs-lookup"><span data-stu-id="154d1-107">Properties</span></span>

| <span data-ttu-id="154d1-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="154d1-108">Property name</span></span>        | <span data-ttu-id="154d1-109">类型</span><span class="sxs-lookup"><span data-stu-id="154d1-109">Type</span></span>     | <span data-ttu-id="154d1-110">说明</span><span class="sxs-lookup"><span data-stu-id="154d1-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="154d1-111">**主机名称**</span><span class="sxs-lookup"><span data-stu-id="154d1-111">**hostname**</span></span>         | <span data-ttu-id="154d1-112">字符串</span><span class="sxs-lookup"><span data-stu-id="154d1-112">string</span></span>   | <span data-ttu-id="154d1-p101">网站集的主机名称。只读。</span><span class="sxs-lookup"><span data-stu-id="154d1-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="154d1-115">**root**</span><span class="sxs-lookup"><span data-stu-id="154d1-115">**root**</span></span>             | <span data-ttu-id="154d1-116">[root][]</span><span class="sxs-lookup"><span data-stu-id="154d1-116">[root][]</span></span> | <span data-ttu-id="154d1-117">如果存在此参数，指示这是 SharePoint 中的根网站集。</span><span class="sxs-lookup"><span data-stu-id="154d1-117">If present, indicates that this is the root site in the site collection. Read-only.</span></span> <span data-ttu-id="154d1-118">只读。</span><span class="sxs-lookup"><span data-stu-id="154d1-118">Read-only.</span></span>

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
