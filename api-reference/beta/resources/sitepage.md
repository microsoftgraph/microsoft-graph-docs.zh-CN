---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7b1634e79214f1cece85a78af29db6422ac03a81
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583401"
---
# <a name="sitepage-resource"></a><span data-ttu-id="bb6d3-102">sitePage 资源</span><span class="sxs-lookup"><span data-stu-id="bb6d3-102">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb6d3-103">此资源表示 "SitePages"[列表][]中的页面。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-103">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="bb6d3-104">它包含[web 部件][]s 的标题、布局和集合。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-104">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="bb6d3-105">页面上的任务</span><span class="sxs-lookup"><span data-stu-id="bb6d3-105">Tasks on a page</span></span>

<span data-ttu-id="bb6d3-106">以下任务可用于**sitePage**资源。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-106">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="bb6d3-107">下面的所有示例都是相对于[网站][]而言的`https://graph.microsoft.com/{api-version}/sites/{site-id}`, 例如:。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-107">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="bb6d3-108">常见任务</span><span class="sxs-lookup"><span data-stu-id="bb6d3-108">Common task</span></span>                     | <span data-ttu-id="bb6d3-109">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="bb6d3-109">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="bb6d3-110">[列出页面][]</span><span class="sxs-lookup"><span data-stu-id="bb6d3-110">[List pages][]</span></span>                  | <span data-ttu-id="bb6d3-111">获取/pages</span><span class="sxs-lookup"><span data-stu-id="bb6d3-111">GET /pages</span></span>
| <span data-ttu-id="bb6d3-112">[获取页面][]</span><span class="sxs-lookup"><span data-stu-id="bb6d3-112">[Get page][]</span></span>                    | <span data-ttu-id="bb6d3-113">获取/pages/{page-id}</span><span class="sxs-lookup"><span data-stu-id="bb6d3-113">GET /pages/{page-id}</span></span>
| <span data-ttu-id="bb6d3-114">[创建][]</span><span class="sxs-lookup"><span data-stu-id="bb6d3-114">[Create][]</span></span>                      | <span data-ttu-id="bb6d3-115">POST/pages</span><span class="sxs-lookup"><span data-stu-id="bb6d3-115">POST /pages</span></span>
| <span data-ttu-id="bb6d3-116">[删除][]</span><span class="sxs-lookup"><span data-stu-id="bb6d3-116">[Delete][]</span></span>                      | <span data-ttu-id="bb6d3-117">删除/pages/{page-id}</span><span class="sxs-lookup"><span data-stu-id="bb6d3-117">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="bb6d3-118">[发布][]</span><span class="sxs-lookup"><span data-stu-id="bb6d3-118">[Publish][]</span></span>                     | <span data-ttu-id="bb6d3-119">POST/pages/{page-id}/publish</span><span class="sxs-lookup"><span data-stu-id="bb6d3-119">POST /pages/{page-id}/publish</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="bb6d3-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb6d3-125">JSON representation</span></span>

<span data-ttu-id="bb6d3-126">下面是**sitePage**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-126">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="bb6d3-127">属性</span><span class="sxs-lookup"><span data-stu-id="bb6d3-127">Properties</span></span>

<span data-ttu-id="bb6d3-128">**sitePage**资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-128">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="bb6d3-129">属性名称</span><span class="sxs-lookup"><span data-stu-id="bb6d3-129">Property name</span></span>    | <span data-ttu-id="bb6d3-130">类型</span><span class="sxs-lookup"><span data-stu-id="bb6d3-130">Type</span></span>                         | <span data-ttu-id="bb6d3-131">说明</span><span class="sxs-lookup"><span data-stu-id="bb6d3-131">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="bb6d3-132">contentType</span><span class="sxs-lookup"><span data-stu-id="bb6d3-132">contentType</span></span>      | <span data-ttu-id="bb6d3-133">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="bb6d3-133">[contentTypeInfo][]</span></span>          | <span data-ttu-id="bb6d3-134">页面的内容类型。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-134">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="bb6d3-135">页面内容</span><span class="sxs-lookup"><span data-stu-id="bb6d3-135">Page Content</span></span>

<span data-ttu-id="bb6d3-136">**sitePage**资源具有以下内容字段。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-136">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="bb6d3-137">属性名称</span><span class="sxs-lookup"><span data-stu-id="bb6d3-137">Property name</span></span>      | <span data-ttu-id="bb6d3-138">类型</span><span class="sxs-lookup"><span data-stu-id="bb6d3-138">Type</span></span>                       | <span data-ttu-id="bb6d3-139">说明</span><span class="sxs-lookup"><span data-stu-id="bb6d3-139">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="bb6d3-140">title</span><span class="sxs-lookup"><span data-stu-id="bb6d3-140">title</span></span>              | <span data-ttu-id="bb6d3-141">字符串</span><span class="sxs-lookup"><span data-stu-id="bb6d3-141">string</span></span>                     | <span data-ttu-id="bb6d3-142">页面的标题。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-142">The title of the page.</span></span>
| <span data-ttu-id="bb6d3-143">pageLayout</span><span class="sxs-lookup"><span data-stu-id="bb6d3-143">pageLayout</span></span>         | <span data-ttu-id="bb6d3-144">string</span><span class="sxs-lookup"><span data-stu-id="bb6d3-144">string</span></span>                     | <span data-ttu-id="bb6d3-145">页面的页面布局的名称。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-145">The name of the page layout of the page.</span></span>
| <span data-ttu-id="bb6d3-146">部件</span><span class="sxs-lookup"><span data-stu-id="bb6d3-146">webParts</span></span>           | <span data-ttu-id="bb6d3-147">[.webpart][]</span><span class="sxs-lookup"><span data-stu-id="bb6d3-147">[webPart][]</span></span>                | <span data-ttu-id="bb6d3-148">页面上的 web 部件。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-148">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="bb6d3-149">创作元数据</span><span class="sxs-lookup"><span data-stu-id="bb6d3-149">Authoring Metadata</span></span>

<span data-ttu-id="bb6d3-150">**sitePage**资源具有以下与创作相关的元数据。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-150">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="bb6d3-151">publishingState 属性将反映页面创作状态 (如 "已签出" 或 "已发布")。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-151">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="bb6d3-152">属性名称</span><span class="sxs-lookup"><span data-stu-id="bb6d3-152">Property name</span></span>          | <span data-ttu-id="bb6d3-153">类型</span><span class="sxs-lookup"><span data-stu-id="bb6d3-153">Type</span></span>                   | <span data-ttu-id="bb6d3-154">说明</span><span class="sxs-lookup"><span data-stu-id="bb6d3-154">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="bb6d3-155">publishingState</span><span class="sxs-lookup"><span data-stu-id="bb6d3-155">publishingState</span></span>        | <span data-ttu-id="bb6d3-156">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="bb6d3-156">[publicationFacet][]</span></span>   | <span data-ttu-id="bb6d3-157">页面的发布状态和 MM.mm 版本。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-157">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="bb6d3-158">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-158">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="bb6d3-159">属性名称</span><span class="sxs-lookup"><span data-stu-id="bb6d3-159">Property name</span></span>        | <span data-ttu-id="bb6d3-160">类型</span><span class="sxs-lookup"><span data-stu-id="bb6d3-160">Type</span></span>              | <span data-ttu-id="bb6d3-161">说明</span><span class="sxs-lookup"><span data-stu-id="bb6d3-161">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="bb6d3-162">id</span><span class="sxs-lookup"><span data-stu-id="bb6d3-162">id</span></span>                   | <span data-ttu-id="bb6d3-163">string</span><span class="sxs-lookup"><span data-stu-id="bb6d3-163">string</span></span>            | <span data-ttu-id="bb6d3-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="bb6d3-166">name</span><span class="sxs-lookup"><span data-stu-id="bb6d3-166">name</span></span>                 | <span data-ttu-id="bb6d3-167">string</span><span class="sxs-lookup"><span data-stu-id="bb6d3-167">string</span></span>            | <span data-ttu-id="bb6d3-168">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-168">The name / title of the item.</span></span>
| <span data-ttu-id="bb6d3-169">createdBy</span><span class="sxs-lookup"><span data-stu-id="bb6d3-169">createdBy</span></span>            | <span data-ttu-id="bb6d3-170">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="bb6d3-170">[identitySet][]</span></span>   | <span data-ttu-id="bb6d3-171">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-171">Identity of the creator of this item.</span></span> <span data-ttu-id="bb6d3-172">只读。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-172">Read-only.</span></span>
| <span data-ttu-id="bb6d3-173">eTag</span><span class="sxs-lookup"><span data-stu-id="bb6d3-173">eTag</span></span>                 | <span data-ttu-id="bb6d3-174">字符串</span><span class="sxs-lookup"><span data-stu-id="bb6d3-174">string</span></span>            | <span data-ttu-id="bb6d3-p106">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="bb6d3-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="bb6d3-177">lastModifiedBy</span></span>       | <span data-ttu-id="bb6d3-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="bb6d3-178">[identitySet][]</span></span>   | <span data-ttu-id="bb6d3-179">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="bb6d3-180">只读。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-180">Read-only.</span></span>
| <span data-ttu-id="bb6d3-181">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb6d3-181">lastModifiedDateTime</span></span> | <span data-ttu-id="bb6d3-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb6d3-182">DateTimeOffset</span></span>    | <span data-ttu-id="bb6d3-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="bb6d3-185">parentReference</span><span class="sxs-lookup"><span data-stu-id="bb6d3-185">parentReference</span></span>      | <span data-ttu-id="bb6d3-186">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="bb6d3-186">[itemReference][]</span></span> | <span data-ttu-id="bb6d3-p109">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="bb6d3-189">webUrl</span><span class="sxs-lookup"><span data-stu-id="bb6d3-189">webUrl</span></span>               | <span data-ttu-id="bb6d3-190">string (url)</span><span class="sxs-lookup"><span data-stu-id="bb6d3-190">string (url)</span></span>      | <span data-ttu-id="bb6d3-p110">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="bb6d3-193">关系</span><span class="sxs-lookup"><span data-stu-id="bb6d3-193">Relationships</span></span>

<span data-ttu-id="bb6d3-194">**sitePage**资源不具有与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="bb6d3-194">The **sitePage** resource does not have relationships to other resources.</span></span>

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
[.webpart]: webpart.md
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
  "suppressions": [
    "Error: /api-reference/beta/resources/sitepage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
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
