---
author: rahmit
description: 此资源表示 "SitePages" 列表中的页面。
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 240ab50f31d500fad960768bb6c45cb9c6ff6511
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965045"
---
# <a name="sitepage-resource"></a><span data-ttu-id="24081-103">sitePage 资源</span><span class="sxs-lookup"><span data-stu-id="24081-103">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24081-104">此资源表示 "SitePages"[列表][]中的页面。</span><span class="sxs-lookup"><span data-stu-id="24081-104">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="24081-105">它包含[Web 部件][]s 的标题、布局和集合。</span><span class="sxs-lookup"><span data-stu-id="24081-105">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="24081-106">页面上的任务</span><span class="sxs-lookup"><span data-stu-id="24081-106">Tasks on a page</span></span>

<span data-ttu-id="24081-107">以下任务可用于**sitePage**资源。</span><span class="sxs-lookup"><span data-stu-id="24081-107">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="24081-108">下面的所有示例都是相对于[网站][]而言的`https://graph.microsoft.com/{api-version}/sites/{site-id}`, 例如:。</span><span class="sxs-lookup"><span data-stu-id="24081-108">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="24081-109">常见任务</span><span class="sxs-lookup"><span data-stu-id="24081-109">Common task</span></span>                     | <span data-ttu-id="24081-110">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="24081-110">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="24081-111">[列出页面][]</span><span class="sxs-lookup"><span data-stu-id="24081-111">[List pages][]</span></span>                  | <span data-ttu-id="24081-112">获取/pages</span><span class="sxs-lookup"><span data-stu-id="24081-112">GET /pages</span></span>
| <span data-ttu-id="24081-113">[获取页面][]</span><span class="sxs-lookup"><span data-stu-id="24081-113">[Get page][]</span></span>                    | <span data-ttu-id="24081-114">获取/pages/{page-id}</span><span class="sxs-lookup"><span data-stu-id="24081-114">GET /pages/{page-id}</span></span>
| <span data-ttu-id="24081-115">[创建][]</span><span class="sxs-lookup"><span data-stu-id="24081-115">[Create][]</span></span>                      | <span data-ttu-id="24081-116">POST/pages</span><span class="sxs-lookup"><span data-stu-id="24081-116">POST /pages</span></span>
| <span data-ttu-id="24081-117">[删除][]</span><span class="sxs-lookup"><span data-stu-id="24081-117">[Delete][]</span></span>                      | <span data-ttu-id="24081-118">删除/pages/{page-id}</span><span class="sxs-lookup"><span data-stu-id="24081-118">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="24081-119">[发布][]</span><span class="sxs-lookup"><span data-stu-id="24081-119">[Publish][]</span></span>                     | <span data-ttu-id="24081-120">POST/pages/{page-id}/publish</span><span class="sxs-lookup"><span data-stu-id="24081-120">POST /pages/{page-id}/publish</span></span>

[列出页面]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[获取页面]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[创建]: ../api/sitepage-create.md
[Create]: ../api/sitepage-create.md
[删除]: ../api/sitepage-delete.md
[Delete]: ../api/sitepage-delete.md
[发布]: ../api/sitepage-publish.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="24081-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24081-126">JSON representation</span></span>

<span data-ttu-id="24081-127">下面是**sitePage**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24081-127">Here is a JSON representation of a **sitePage** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage",
  "openType": true
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayoutType": "String",
  "webParts": [{ "@odata.type": "microsoft.graph.webPart" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

   /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="24081-128">属性</span><span class="sxs-lookup"><span data-stu-id="24081-128">Properties</span></span>

<span data-ttu-id="24081-129">**SitePage**资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="24081-129">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="24081-130">属性名</span><span class="sxs-lookup"><span data-stu-id="24081-130">Property name</span></span>    | <span data-ttu-id="24081-131">类型</span><span class="sxs-lookup"><span data-stu-id="24081-131">Type</span></span>                         | <span data-ttu-id="24081-132">说明</span><span class="sxs-lookup"><span data-stu-id="24081-132">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="24081-133">contentType</span><span class="sxs-lookup"><span data-stu-id="24081-133">contentType</span></span>      | <span data-ttu-id="24081-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="24081-134">[contentTypeInfo][]</span></span>          | <span data-ttu-id="24081-135">页面的内容类型。</span><span class="sxs-lookup"><span data-stu-id="24081-135">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="24081-136">页面内容</span><span class="sxs-lookup"><span data-stu-id="24081-136">Page Content</span></span>

<span data-ttu-id="24081-137">**SitePage**资源具有以下内容字段。</span><span class="sxs-lookup"><span data-stu-id="24081-137">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="24081-138">属性名</span><span class="sxs-lookup"><span data-stu-id="24081-138">Property name</span></span>      | <span data-ttu-id="24081-139">类型</span><span class="sxs-lookup"><span data-stu-id="24081-139">Type</span></span>                       | <span data-ttu-id="24081-140">说明</span><span class="sxs-lookup"><span data-stu-id="24081-140">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="24081-141">title</span><span class="sxs-lookup"><span data-stu-id="24081-141">title</span></span>              | <span data-ttu-id="24081-142">字符串</span><span class="sxs-lookup"><span data-stu-id="24081-142">string</span></span>                     | <span data-ttu-id="24081-143">页面的标题。</span><span class="sxs-lookup"><span data-stu-id="24081-143">The title of the page.</span></span>
| <span data-ttu-id="24081-144">pageLayout</span><span class="sxs-lookup"><span data-stu-id="24081-144">pageLayout</span></span>         | <span data-ttu-id="24081-145">string</span><span class="sxs-lookup"><span data-stu-id="24081-145">string</span></span>                     | <span data-ttu-id="24081-146">页面的页面布局的名称。</span><span class="sxs-lookup"><span data-stu-id="24081-146">The name of the page layout of the page.</span></span>
| <span data-ttu-id="24081-147">部件</span><span class="sxs-lookup"><span data-stu-id="24081-147">webParts</span></span>           | <span data-ttu-id="24081-148">[.Webpart][]</span><span class="sxs-lookup"><span data-stu-id="24081-148">[webPart][]</span></span>                | <span data-ttu-id="24081-149">页面上的 web 部件。</span><span class="sxs-lookup"><span data-stu-id="24081-149">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="24081-150">创作元数据</span><span class="sxs-lookup"><span data-stu-id="24081-150">Authoring Metadata</span></span>

<span data-ttu-id="24081-151">**SitePage**资源具有以下与创作相关的元数据。</span><span class="sxs-lookup"><span data-stu-id="24081-151">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="24081-152">PublishingState 属性将反映页面创作状态 (如 "已签出" 或 "已发布")。</span><span class="sxs-lookup"><span data-stu-id="24081-152">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="24081-153">属性名</span><span class="sxs-lookup"><span data-stu-id="24081-153">Property name</span></span>          | <span data-ttu-id="24081-154">类型</span><span class="sxs-lookup"><span data-stu-id="24081-154">Type</span></span>                   | <span data-ttu-id="24081-155">说明</span><span class="sxs-lookup"><span data-stu-id="24081-155">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="24081-156">publishingState</span><span class="sxs-lookup"><span data-stu-id="24081-156">publishingState</span></span>        | <span data-ttu-id="24081-157">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="24081-157">[publicationFacet][]</span></span>   | <span data-ttu-id="24081-158">页面的发布状态和 MM.mm 版本。</span><span class="sxs-lookup"><span data-stu-id="24081-158">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="24081-159">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="24081-159">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="24081-160">属性名称</span><span class="sxs-lookup"><span data-stu-id="24081-160">Property name</span></span>        | <span data-ttu-id="24081-161">类型</span><span class="sxs-lookup"><span data-stu-id="24081-161">Type</span></span>              | <span data-ttu-id="24081-162">说明</span><span class="sxs-lookup"><span data-stu-id="24081-162">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="24081-163">id</span><span class="sxs-lookup"><span data-stu-id="24081-163">id</span></span>                   | <span data-ttu-id="24081-164">string</span><span class="sxs-lookup"><span data-stu-id="24081-164">string</span></span>            | <span data-ttu-id="24081-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="24081-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="24081-167">name</span><span class="sxs-lookup"><span data-stu-id="24081-167">name</span></span>                 | <span data-ttu-id="24081-168">string</span><span class="sxs-lookup"><span data-stu-id="24081-168">string</span></span>            | <span data-ttu-id="24081-169">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="24081-169">The name / title of the item.</span></span>
| <span data-ttu-id="24081-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="24081-170">createdBy</span></span>            | <span data-ttu-id="24081-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="24081-171">[identitySet][]</span></span>   | <span data-ttu-id="24081-172">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="24081-172">Identity of the creator of this item.</span></span> <span data-ttu-id="24081-173">只读。</span><span class="sxs-lookup"><span data-stu-id="24081-173">Read-only.</span></span>
| <span data-ttu-id="24081-174">eTag</span><span class="sxs-lookup"><span data-stu-id="24081-174">eTag</span></span>                 | <span data-ttu-id="24081-175">字符串</span><span class="sxs-lookup"><span data-stu-id="24081-175">string</span></span>            | <span data-ttu-id="24081-p106">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="24081-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="24081-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="24081-178">lastModifiedBy</span></span>       | <span data-ttu-id="24081-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="24081-179">[identitySet][]</span></span>   | <span data-ttu-id="24081-180">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="24081-180">Identity of the last modifier of this item.</span></span> <span data-ttu-id="24081-181">只读。</span><span class="sxs-lookup"><span data-stu-id="24081-181">Read-only.</span></span>
| <span data-ttu-id="24081-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24081-182">lastModifiedDateTime</span></span> | <span data-ttu-id="24081-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24081-183">DateTimeOffset</span></span>    | <span data-ttu-id="24081-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="24081-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="24081-186">parentReference</span><span class="sxs-lookup"><span data-stu-id="24081-186">parentReference</span></span>      | <span data-ttu-id="24081-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="24081-187">[itemReference][]</span></span> | <span data-ttu-id="24081-p109">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="24081-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="24081-190">WebUrl</span><span class="sxs-lookup"><span data-stu-id="24081-190">webUrl</span></span>               | <span data-ttu-id="24081-191">string (url)</span><span class="sxs-lookup"><span data-stu-id="24081-191">string (url)</span></span>      | <span data-ttu-id="24081-p110">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="24081-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="24081-194">关系</span><span class="sxs-lookup"><span data-stu-id="24081-194">Relationships</span></span>

<span data-ttu-id="24081-195">**SitePage**资源不具有与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="24081-195">The **sitePage** resource does not have relationships to other resources.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md
[网站]: site.md
[site]: site.md
[.Webpart]: webpart.md
[webPart]: webpart.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  },
  "suppressions": []
}
-->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
