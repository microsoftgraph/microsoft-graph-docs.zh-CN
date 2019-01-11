---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.openlocfilehash: a0c55967ed7f7a397e0c8c0a4ce607921dc8a9f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830546"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="a5495-102">SiteCollection 资源</span><span class="sxs-lookup"><span data-stu-id="a5495-102">SiteCollection resource</span></span>

> <span data-ttu-id="a5495-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a5495-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5495-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a5495-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5495-105">**siteCollection** 资源提供有关网站集的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a5495-105">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="a5495-106">如果[**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。</span><span class="sxs-lookup"><span data-stu-id="a5495-106">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5495-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5495-107">JSON representation</span></span>

<span data-ttu-id="a5495-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5495-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a5495-109">属性</span><span class="sxs-lookup"><span data-stu-id="a5495-109">Properties</span></span>

| <span data-ttu-id="a5495-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="a5495-110">Property name</span></span>        | <span data-ttu-id="a5495-111">类型</span><span class="sxs-lookup"><span data-stu-id="a5495-111">Type</span></span>     | <span data-ttu-id="a5495-112">说明</span><span class="sxs-lookup"><span data-stu-id="a5495-112">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="a5495-113">**主机名称**</span><span class="sxs-lookup"><span data-stu-id="a5495-113">**hostname**</span></span>         | <span data-ttu-id="a5495-114">string</span><span class="sxs-lookup"><span data-stu-id="a5495-114">string</span></span>   | <span data-ttu-id="a5495-p102">网站集的主机名称。只读。</span><span class="sxs-lookup"><span data-stu-id="a5495-p102">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="a5495-117">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="a5495-117">**dataLocationCode**</span></span> | <span data-ttu-id="a5495-118">string</span><span class="sxs-lookup"><span data-stu-id="a5495-118">string</span></span>   | <span data-ttu-id="a5495-119">地理区域代码为此网站集所在的位置。</span><span class="sxs-lookup"><span data-stu-id="a5495-119">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="a5495-120">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="a5495-120">Read-only.</span></span>
| <span data-ttu-id="a5495-121">**根**</span><span class="sxs-lookup"><span data-stu-id="a5495-121">**root**</span></span>             | <span data-ttu-id="a5495-122">[根][]</span><span class="sxs-lookup"><span data-stu-id="a5495-122">[root][]</span></span> | <span data-ttu-id="a5495-123">如果存在此参数，指示这是 SharePoint 中的根网站集。</span><span class="sxs-lookup"><span data-stu-id="a5495-123">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="a5495-124">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="a5495-124">Read-only.</span></span>

[根]: root.md
[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
