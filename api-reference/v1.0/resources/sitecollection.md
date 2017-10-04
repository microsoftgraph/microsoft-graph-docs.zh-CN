---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: 6b36f3a0c2d958081f1b5663231a541f2e8a000f
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="sitecollection-resource"></a><span data-ttu-id="6c6ff-102">SiteCollection 资源</span><span class="sxs-lookup"><span data-stu-id="6c6ff-102">SiteCollection resource</span></span>

<span data-ttu-id="6c6ff-103">**siteCollection** 资源提供有关网站集的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6c6ff-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="6c6ff-104">如果[**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。</span><span class="sxs-lookup"><span data-stu-id="6c6ff-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c6ff-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c6ff-105">JSON representation</span></span>

<span data-ttu-id="6c6ff-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c6ff-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com"
}
```

## <a name="properties"></a><span data-ttu-id="6c6ff-107">属性</span><span class="sxs-lookup"><span data-stu-id="6c6ff-107">Properties</span></span>

| <span data-ttu-id="6c6ff-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="6c6ff-108">Property name</span></span> | <span data-ttu-id="6c6ff-109">类型</span><span class="sxs-lookup"><span data-stu-id="6c6ff-109">Type</span></span>    | <span data-ttu-id="6c6ff-110">说明</span><span class="sxs-lookup"><span data-stu-id="6c6ff-110">Description</span></span>                                                                                                                  |
|:--------------|:--------|:---------------------------------------------------
| <span data-ttu-id="6c6ff-111">**主机名称**</span><span class="sxs-lookup"><span data-stu-id="6c6ff-111">**hostname**</span></span>  | <span data-ttu-id="6c6ff-112">string</span><span class="sxs-lookup"><span data-stu-id="6c6ff-112">string</span></span>  | <span data-ttu-id="6c6ff-p101">网站集的主机名称。只读。</span><span class="sxs-lookup"><span data-stu-id="6c6ff-p101">The hostname for the site collection. Read-only.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Facets/SiteCollection"
}-->
