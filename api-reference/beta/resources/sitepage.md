---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
ms.openlocfilehash: 65cfe61dadd1708abffe2d01abbbb15f40d158ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047134"
---
# <a name="sitepage-resource"></a><span data-ttu-id="f0ae5-102">sitePage 资源</span><span class="sxs-lookup"><span data-stu-id="f0ae5-102">sitePage resource</span></span>

> <span data-ttu-id="f0ae5-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0ae5-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0ae5-105">此资源代表 SitePages[列表][]中的页面。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-105">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="f0ae5-106">它包含标题、 布局和[web 部件][]s 的集合。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-106">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="f0ae5-107">页面上的任务</span><span class="sxs-lookup"><span data-stu-id="f0ae5-107">Tasks on a page</span></span>

<span data-ttu-id="f0ae5-108">为**sitePage**资源提供了下列任务。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-108">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="f0ae5-109">下面的所有示例都是相对于[网站][]，如： `https://graph.microsoft.com/{api-version}/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-109">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="f0ae5-110">常见任务</span><span class="sxs-lookup"><span data-stu-id="f0ae5-110">Common task</span></span>                     | <span data-ttu-id="f0ae5-111">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="f0ae5-111">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="f0ae5-112">[List pages][]</span><span class="sxs-lookup"><span data-stu-id="f0ae5-112">[List pages][]</span></span>                  | <span data-ttu-id="f0ae5-113">获取 /pages</span><span class="sxs-lookup"><span data-stu-id="f0ae5-113">GET /pages</span></span>
| <span data-ttu-id="f0ae5-114">[Get page][]</span><span class="sxs-lookup"><span data-stu-id="f0ae5-114">[Get page][]</span></span>                    | <span data-ttu-id="f0ae5-115">获取 /pages/ {页-id}</span><span class="sxs-lookup"><span data-stu-id="f0ae5-115">GET /pages/{page-id}</span></span>
| <span data-ttu-id="f0ae5-116">[Create][]</span><span class="sxs-lookup"><span data-stu-id="f0ae5-116">[Create][]</span></span>                      | <span data-ttu-id="f0ae5-117">POST /pages</span><span class="sxs-lookup"><span data-stu-id="f0ae5-117">POST /pages</span></span>
| <span data-ttu-id="f0ae5-118">[删除][]</span><span class="sxs-lookup"><span data-stu-id="f0ae5-118">[Delete][]</span></span>                      | <span data-ttu-id="f0ae5-119">删除 /pages/ {页-id}</span><span class="sxs-lookup"><span data-stu-id="f0ae5-119">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="f0ae5-120">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="f0ae5-120">[Publish][]</span></span>                     | <span data-ttu-id="f0ae5-121">发布 /pages/ {页-id} / 发布</span><span class="sxs-lookup"><span data-stu-id="f0ae5-121">POST /pages/{page-id}/publish</span></span>

[List pages]: ../api/sitepage-list.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[删除]: ../api/sitepage-delete.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="f0ae5-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0ae5-127">JSON representation</span></span>

<span data-ttu-id="f0ae5-128">下面是**sitePage**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-128">Here is a JSON representation of a **sitePage** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayout": "Article",
  "webParts": [{ "@odata.type": "microsoft.graph.sitePageWebParts" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

  /* inherited from baseItem */
  "id": "string",
  "name": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="f0ae5-129">属性</span><span class="sxs-lookup"><span data-stu-id="f0ae5-129">Properties</span></span>

<span data-ttu-id="f0ae5-130">**SitePage**资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-130">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="f0ae5-131">属性名</span><span class="sxs-lookup"><span data-stu-id="f0ae5-131">Property name</span></span>    | <span data-ttu-id="f0ae5-132">类型</span><span class="sxs-lookup"><span data-stu-id="f0ae5-132">Type</span></span>                         | <span data-ttu-id="f0ae5-133">说明</span><span class="sxs-lookup"><span data-stu-id="f0ae5-133">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="f0ae5-134">contentType</span><span class="sxs-lookup"><span data-stu-id="f0ae5-134">contentType</span></span>      | <span data-ttu-id="f0ae5-135">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="f0ae5-135">[contentTypeInfo][]</span></span>          | <span data-ttu-id="f0ae5-136">页面内容类型。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-136">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="f0ae5-137">页面内容</span><span class="sxs-lookup"><span data-stu-id="f0ae5-137">Page Content</span></span>

<span data-ttu-id="f0ae5-138">**SitePage**资源具有以下内容的字段。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-138">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="f0ae5-139">属性名</span><span class="sxs-lookup"><span data-stu-id="f0ae5-139">Property name</span></span>      | <span data-ttu-id="f0ae5-140">类型</span><span class="sxs-lookup"><span data-stu-id="f0ae5-140">Type</span></span>                       | <span data-ttu-id="f0ae5-141">说明</span><span class="sxs-lookup"><span data-stu-id="f0ae5-141">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="f0ae5-142">title</span><span class="sxs-lookup"><span data-stu-id="f0ae5-142">title</span></span>              | <span data-ttu-id="f0ae5-143">字符串</span><span class="sxs-lookup"><span data-stu-id="f0ae5-143">string</span></span>                     | <span data-ttu-id="f0ae5-144">页面的标题。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-144">The title of the page.</span></span>
| <span data-ttu-id="f0ae5-145">pageLayout</span><span class="sxs-lookup"><span data-stu-id="f0ae5-145">pageLayout</span></span>         | <span data-ttu-id="f0ae5-146">string</span><span class="sxs-lookup"><span data-stu-id="f0ae5-146">string</span></span>                     | <span data-ttu-id="f0ae5-147">页的页面布局的名称。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-147">The name of the page layout of the page.</span></span>
| <span data-ttu-id="f0ae5-148">web 部件</span><span class="sxs-lookup"><span data-stu-id="f0ae5-148">webParts</span></span>           | <span data-ttu-id="f0ae5-149">[web 部件][]</span><span class="sxs-lookup"><span data-stu-id="f0ae5-149">[webPart][]</span></span>                | <span data-ttu-id="f0ae5-150">Web 部件页上。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-150">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="f0ae5-151">创作元数据</span><span class="sxs-lookup"><span data-stu-id="f0ae5-151">Authoring Metadata</span></span>

<span data-ttu-id="f0ae5-152">**SitePage**资源具有创作相关的以下元数据。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-152">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="f0ae5-153">PublishingState 属性将反映创作 like 签出或发布的状态页。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-153">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="f0ae5-154">属性名</span><span class="sxs-lookup"><span data-stu-id="f0ae5-154">Property name</span></span>          | <span data-ttu-id="f0ae5-155">类型</span><span class="sxs-lookup"><span data-stu-id="f0ae5-155">Type</span></span>                   | <span data-ttu-id="f0ae5-156">说明</span><span class="sxs-lookup"><span data-stu-id="f0ae5-156">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="f0ae5-157">publishingState</span><span class="sxs-lookup"><span data-stu-id="f0ae5-157">publishingState</span></span>        | <span data-ttu-id="f0ae5-158">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="f0ae5-158">[publicationFacet][]</span></span>   | <span data-ttu-id="f0ae5-159">发布状态和页的 MM.mm 版本。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-159">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="f0ae5-160">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-160">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="f0ae5-161">属性名称</span><span class="sxs-lookup"><span data-stu-id="f0ae5-161">Property name</span></span>        | <span data-ttu-id="f0ae5-162">类型</span><span class="sxs-lookup"><span data-stu-id="f0ae5-162">Type</span></span>              | <span data-ttu-id="f0ae5-163">说明</span><span class="sxs-lookup"><span data-stu-id="f0ae5-163">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="f0ae5-164">ID</span><span class="sxs-lookup"><span data-stu-id="f0ae5-164">id</span></span>                   | <span data-ttu-id="f0ae5-165">string</span><span class="sxs-lookup"><span data-stu-id="f0ae5-165">string</span></span>            | <span data-ttu-id="f0ae5-p105">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-p105">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="f0ae5-168">name</span><span class="sxs-lookup"><span data-stu-id="f0ae5-168">name</span></span>                 | <span data-ttu-id="f0ae5-169">string</span><span class="sxs-lookup"><span data-stu-id="f0ae5-169">string</span></span>            | <span data-ttu-id="f0ae5-170">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-170">The name / title of the item.</span></span>
| <span data-ttu-id="f0ae5-171">createdBy</span><span class="sxs-lookup"><span data-stu-id="f0ae5-171">createdBy</span></span>            | <span data-ttu-id="f0ae5-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f0ae5-172">[identitySet][]</span></span>   | <span data-ttu-id="f0ae5-173">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-173">Identity of the creator of this item.</span></span> <span data-ttu-id="f0ae5-174">只读。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-174">Read-only.</span></span>
| <span data-ttu-id="f0ae5-175">eTag</span><span class="sxs-lookup"><span data-stu-id="f0ae5-175">eTag</span></span>                 | <span data-ttu-id="f0ae5-176">string</span><span class="sxs-lookup"><span data-stu-id="f0ae5-176">string</span></span>            | <span data-ttu-id="f0ae5-p107">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-p107">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="f0ae5-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f0ae5-179">lastModifiedBy</span></span>       | <span data-ttu-id="f0ae5-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f0ae5-180">[identitySet][]</span></span>   | <span data-ttu-id="f0ae5-181">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="f0ae5-182">只读。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-182">Read-only.</span></span>
| <span data-ttu-id="f0ae5-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0ae5-183">lastModifiedDateTime</span></span> | <span data-ttu-id="f0ae5-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0ae5-184">DateTimeOffset</span></span>    | <span data-ttu-id="f0ae5-p109">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="f0ae5-187">parentReference</span><span class="sxs-lookup"><span data-stu-id="f0ae5-187">parentReference</span></span>      | <span data-ttu-id="f0ae5-188">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="f0ae5-188">[itemReference][]</span></span> | <span data-ttu-id="f0ae5-p110">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-p110">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="f0ae5-191">WebUrl</span><span class="sxs-lookup"><span data-stu-id="f0ae5-191">webUrl</span></span>               | <span data-ttu-id="f0ae5-192">string (url)</span><span class="sxs-lookup"><span data-stu-id="f0ae5-192">string (url)</span></span>      | <span data-ttu-id="f0ae5-p111">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="f0ae5-195">关系</span><span class="sxs-lookup"><span data-stu-id="f0ae5-195">Relationships</span></span>

<span data-ttu-id="f0ae5-196">**SitePage**资源没有与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="f0ae5-196">The **sitePage** resource does not have relationships to other resources.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md
[site]: site.md
[web 部件]: webpart.md
[webPart]: webpart.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  }
} -->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
