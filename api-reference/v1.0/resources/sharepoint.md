---
title: 使用 Microsoft Graph 中的 SharePoint 网站
description: Microsoft Graph 中的 SharePoint API 支持以下核心情形：
localization_priority: Priority
ms.openlocfilehash: 0beb3e5d7b56e072632c093613fee5534ec0e54b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860954"
---
# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a><span data-ttu-id="dab9e-103">使用 Microsoft Graph 中的 SharePoint 网站</span><span class="sxs-lookup"><span data-stu-id="dab9e-103">Working with SharePoint sites in Microsoft Graph</span></span>

<span data-ttu-id="dab9e-104">Microsoft Graph 中的 SharePoint API 支持以下核心情形：</span><span class="sxs-lookup"><span data-stu-id="dab9e-104">The SharePoint API in Microsoft Graph supports the following core scenarios:</span></span>

* <span data-ttu-id="dab9e-105">访问 SharePoint **网站**、**列表**和**驱动器**（文档库）</span><span class="sxs-lookup"><span data-stu-id="dab9e-105">Access to SharePoint **sites**, **lists**, and **drives** (document libraries)</span></span>
* <span data-ttu-id="dab9e-106">支持对 **site** 资源进行只读访问（无法创建新网站）</span><span class="sxs-lookup"><span data-stu-id="dab9e-106">Read-only support for **site** resources (no ability to create new sites)</span></span>
* <span data-ttu-id="dab9e-107">支持对 **lists**、**listItems** 和 **driveItems** 进行读写访问</span><span class="sxs-lookup"><span data-stu-id="dab9e-107">Read-write support for **lists**, **listItems**, and **driveItems**</span></span>
* <span data-ttu-id="dab9e-108">用 SharePoint ID、URL 或相对路径表示的 Address 资源</span><span class="sxs-lookup"><span data-stu-id="dab9e-108">Address resources by SharePoint ID, URL, or relative path</span></span>

<span data-ttu-id="dab9e-109">SharePoint API 公开了三种主要资源类型：</span><span class="sxs-lookup"><span data-stu-id="dab9e-109">The SharePoint API exposes three major resource types:</span></span>

* <span data-ttu-id="dab9e-110">[Site](site.md) _（顶层的对象）_</span><span class="sxs-lookup"><span data-stu-id="dab9e-110">[Site](site.md) _(top-level object)_</span></span>
* [<span data-ttu-id="dab9e-111">List</span><span class="sxs-lookup"><span data-stu-id="dab9e-111">List</span></span>](list.md)
* [<span data-ttu-id="dab9e-112">ListItem</span><span class="sxs-lookup"><span data-stu-id="dab9e-112">ListItem</span></span>](listitem.md)

<span data-ttu-id="dab9e-113">下面的示例展示了 listItem 资源。</span><span class="sxs-lookup"><span data-stu-id="dab9e-113">The following is an example of a listItem resource.</span></span>

```json
{
  "fields": {
    "Title": "Access card",
    "Employee": "Ryan Gregg",
    "EmployeeId": "10",
    "CardSerial": "01235492",
    "Alias": "RGregg",
    "ID": 1,
    "ContentType": "Item",
    "Modified": "2016-09-19T23:15:25-07:00",
    "Created": "2016-09-19T23:15:25-07:00"
  },
  "createdBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "createdDateTime": "2016-09-20T06:15:25Z",
  "eTag": "48e941c3-9515-4c48-9760-c07c90c79d48,1",
  "id": "4",
  "lastModifiedBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "lastModifiedDateTime": "2016-09-20T06:15:25Z",
}
```

<span data-ttu-id="dab9e-114">资源通过三种不同的方式公开数据：</span><span class="sxs-lookup"><span data-stu-id="dab9e-114">Resources expose data in three different ways:</span></span>

* <span data-ttu-id="dab9e-115">_属性_（如 **id** 和 **name**）公开简单值。</span><span class="sxs-lookup"><span data-stu-id="dab9e-115">_Properties_ (like **id** and **name**) expose simple values.</span></span>
* <span data-ttu-id="dab9e-116">_Facet_（如 **fields** 和 **createdBy**）公开复杂值。</span><span class="sxs-lookup"><span data-stu-id="dab9e-116">_Facets_ (like **fields** and **createdBy**) expose complex values.</span></span>
* <span data-ttu-id="dab9e-117">_引用_（如 **items**）指向其他资源的集合。</span><span class="sxs-lookup"><span data-stu-id="dab9e-117">_References_ (like **items**) point to collections of other resources.</span></span>

<span data-ttu-id="dab9e-118">可以使用 _expand_ 查询参数展开 URL 中的引用；例如 `?expand=fields`。</span><span class="sxs-lookup"><span data-stu-id="dab9e-118">You can expand references in your URL with the _expand_ query parameter; for example, `?expand=fields`.</span></span>
<span data-ttu-id="dab9e-119">可以使用 _select_ 查询参数请求特定属性和 facet；例如 `?select=id,name`。</span><span class="sxs-lookup"><span data-stu-id="dab9e-119">You can request specific properties and facets with the _select_ query parameter; for example, `?select=id,name`.</span></span>
<span data-ttu-id="dab9e-120">默认情况下，虽然大部分属性和 Facet 都会返回，但所有引用都会被隐藏。</span><span class="sxs-lookup"><span data-stu-id="dab9e-120">By default, most properties and facets are returned while all references are hidden.</span></span>
<span data-ttu-id="dab9e-121">为了提高效率，建议将 _select_ 和 _expand_ 指定为仅返回你关注的数据。</span><span class="sxs-lookup"><span data-stu-id="dab9e-121">For efficiency, we recommend that you specify _select_ and _expand_ to only return the data you care about.</span></span>

## <a name="sharepoint-api-root-resources"></a><span data-ttu-id="dab9e-122">SharePoint API 根资源</span><span class="sxs-lookup"><span data-stu-id="dab9e-122">SharePoint API root resources</span></span>

<span data-ttu-id="dab9e-123">以下示例与 `https://graph.microsoft.com/v1.0` 有关。</span><span class="sxs-lookup"><span data-stu-id="dab9e-123">The following examples are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="dab9e-124">路径</span><span class="sxs-lookup"><span data-stu-id="dab9e-124">Path</span></span>                                   | <span data-ttu-id="dab9e-125">说明</span><span class="sxs-lookup"><span data-stu-id="dab9e-125">Description</span></span>
|:---------------------------------------|:------------------------------------
| <span data-ttu-id="dab9e-126">/sites/root</span><span class="sxs-lookup"><span data-stu-id="dab9e-126">/sites/root</span></span>                            | <span data-ttu-id="dab9e-127">组织的默认[网站][]。</span><span class="sxs-lookup"><span data-stu-id="dab9e-127">Organization's default [site][].</span></span>
| <span data-ttu-id="dab9e-128">/sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="dab9e-128">/sites/{site-id}</span></span>                       | <span data-ttu-id="dab9e-129">通过其 ID 访问特定[网站][]。</span><span class="sxs-lookup"><span data-stu-id="dab9e-129">Access a specific [site][] by its ID.</span></span>
| <span data-ttu-id="dab9e-130">/sites/{site-id}/drive</span><span class="sxs-lookup"><span data-stu-id="dab9e-130">/sites/{site-id}/drive</span></span>                 | <span data-ttu-id="dab9e-131">访问给定[网站][]的默认[驱动器](drive.md)（文档库）。</span><span class="sxs-lookup"><span data-stu-id="dab9e-131">Access the default [drive](drive.md) (document library) for the given [site][].</span></span>
| <span data-ttu-id="dab9e-132">/sites/{site-id}/drives</span><span class="sxs-lookup"><span data-stu-id="dab9e-132">/sites/{site-id}/drives</span></span>                | <span data-ttu-id="dab9e-133">枚举[网站][]下的[驱动器](drive.md)（文档库）。</span><span class="sxs-lookup"><span data-stu-id="dab9e-133">Enumerate the [drives](drive.md) (document libraries) under the [site][].</span></span>
| <span data-ttu-id="dab9e-134">/sites/{site-id}/sites</span><span class="sxs-lookup"><span data-stu-id="dab9e-134">/sites/{site-id}/sites</span></span>                 | <span data-ttu-id="dab9e-135">枚举[网站][]下的子网站。</span><span class="sxs-lookup"><span data-stu-id="dab9e-135">Enumerate the sub-sites under the [site][].</span></span>
| <span data-ttu-id="dab9e-136">/sites/{site-id}/lists</span><span class="sxs-lookup"><span data-stu-id="dab9e-136">/sites/{site-id}/lists</span></span>                 | <span data-ttu-id="dab9e-137">枚举[网站](site.md)下的[列表](list.md)。</span><span class="sxs-lookup"><span data-stu-id="dab9e-137">Enumerate the [lists](list.md) under the [site](site.md).</span></span>
| <span data-ttu-id="dab9e-138">/sites/{site-id}/lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="dab9e-138">/sites/{site-id}/lists/{list-id}/items</span></span> | <span data-ttu-id="dab9e-139">枚举[列表](list.md)下的 [listItem](listitem.md)。</span><span class="sxs-lookup"><span data-stu-id="dab9e-139">Enumerate the [listItems](listitem.md) under the [list](list.md).</span></span>
| <span data-ttu-id="dab9e-140">/groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="dab9e-140">/groups/{group-id}/sites/root</span></span>          | <span data-ttu-id="dab9e-141">访问组的团队[网站][]。</span><span class="sxs-lookup"><span data-stu-id="dab9e-141">Access a group's team [site][].</span></span>

<span data-ttu-id="dab9e-p102">还可以使用 SharePoint 主机名，后面加上冒号和网站的相对路径，来为网站寻址。可以选择将另一个冒号置于末尾，转回为资源模型寻址。</span><span class="sxs-lookup"><span data-stu-id="dab9e-p102">Sites can also be addressed by path by using the SharePoint hostname, followed by a colon and the relative path to the site. You can optionally transition back to addressing the resource model by putting another colon at the end.</span></span>

| <span data-ttu-id="dab9e-144">Path</span><span class="sxs-lookup"><span data-stu-id="dab9e-144">Path</span></span>                                           | <span data-ttu-id="dab9e-145">说明</span><span class="sxs-lookup"><span data-stu-id="dab9e-145">Description</span></span>
|:-----------------------------------------------|:-----------------------------------
| <span data-ttu-id="dab9e-146">/sites/contoso.sharepoint.com:/teams/hr</span><span class="sxs-lookup"><span data-stu-id="dab9e-146">/sites/contoso.sharepoint.com:/teams/hr</span></span>        | <span data-ttu-id="dab9e-147">与关联的网站https://contoso.sharepoint.com/teams/hr</span><span class="sxs-lookup"><span data-stu-id="dab9e-147">The site associated with https://contoso.sharepoint.com/teams/hr</span></span>
| <span data-ttu-id="dab9e-148">/sites/contoso.sharepoint.com:/teams/hr:/drive</span><span class="sxs-lookup"><span data-stu-id="dab9e-148">/sites/contoso.sharepoint.com:/teams/hr:/drive</span></span> | <span data-ttu-id="dab9e-149">访问此网站的默认[驱动器](drive.md)。</span><span class="sxs-lookup"><span data-stu-id="dab9e-149">Access the default [drive](drive.md) for this site.</span></span>

## <a name="note-for-existing-sharepoint-developers"></a><span data-ttu-id="dab9e-150">现有 SharePoint 开发人员须知</span><span class="sxs-lookup"><span data-stu-id="dab9e-150">Note for existing SharePoint developers</span></span>

<span data-ttu-id="dab9e-p103">Microsoft Graph SharePoint API 与 CSOM API 有几个主要区别。[网站][]资源映射到 `SPWeb`。网站集中的根[网站][] (`SPWeb`) 具有 [siteCollection](sitecollection.md) 方面，其中包含有关 `SPSite` 的信息。由于网站 ID 只在其网站集中是唯一的，因此按 ID 为网站寻址需要提供网站集标识符和网站标识符。</span><span class="sxs-lookup"><span data-stu-id="dab9e-p103">The Microsoft Graph SharePoint API has a few key differences with the CSOM APIs. The [site][] resource maps to `SPWeb`. The root [site][] (`SPWeb`) in a site collection has a [siteCollection](sitecollection.md) facet, which contains information about the `SPSite`. Because IDs for sites are only unique within their site collection, addressing a site by ID requires providing both the site collection identifier and the site identifier.</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id},{spweb-id}/
```
<span data-ttu-id="dab9e-155">仅使用主机名构造的 URL 将指向默认网站集中的根网站 (`SPWeb`)。</span><span class="sxs-lookup"><span data-stu-id="dab9e-155">A URL constructed with only the hostname will point to the root site (`SPWeb`) in the default site collection.</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname}
```

<span data-ttu-id="dab9e-156">仅使用主机名和 siteCollection (`SPSite`) ID 构造的 URL 将指向给定网站集中的根网站 (`SPWeb`)。</span><span class="sxs-lookup"><span data-stu-id="dab9e-156">A URL constructed with only the hostname and siteCollection (`SPSite`) ID will point to the root site (`SPWeb`) in the given site collection.</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id}
```

[site]: site.md
[list]: list.md
[drive]: drive.md
[siteCollection]: sitecollection.md

<!-- {
  "type": "#page.annotation",
  "description": "Getting started programming with the SharePoint API",
  "keywords": "getting started sharepoint rest api programming C# ios android rest http",
  "section": "documentation",
  "tocPath": "Getting Started",
  "tocIndex": -100
} -->
