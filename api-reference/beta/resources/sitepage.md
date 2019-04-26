---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 6a9192423c4caf47913029e3671e975884533333
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343064"
---
# <a name="sitepage-resource"></a><span data-ttu-id="5953b-102">sitePage 资源</span><span class="sxs-lookup"><span data-stu-id="5953b-102">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5953b-103">此资源表示 "SitePages"[列表][]中的页面。</span><span class="sxs-lookup"><span data-stu-id="5953b-103">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="5953b-104">它包含[web 部件][]s 的标题、布局和集合。</span><span class="sxs-lookup"><span data-stu-id="5953b-104">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="5953b-105">页面上的任务</span><span class="sxs-lookup"><span data-stu-id="5953b-105">Tasks on a page</span></span>

<span data-ttu-id="5953b-106">以下任务可用于**sitePage**资源。</span><span class="sxs-lookup"><span data-stu-id="5953b-106">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="5953b-107">下面的所有示例都是相对于[网站][]而言的`https://graph.microsoft.com/{api-version}/sites/{site-id}`, 例如:。</span><span class="sxs-lookup"><span data-stu-id="5953b-107">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="5953b-108">常见任务</span><span class="sxs-lookup"><span data-stu-id="5953b-108">Common task</span></span>                     | <span data-ttu-id="5953b-109">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="5953b-109">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="5953b-110">[列出页面][]</span><span class="sxs-lookup"><span data-stu-id="5953b-110">[List pages][]</span></span>                  | <span data-ttu-id="5953b-111">获取/pages</span><span class="sxs-lookup"><span data-stu-id="5953b-111">GET /pages</span></span>
| <span data-ttu-id="5953b-112">[获取页面][]</span><span class="sxs-lookup"><span data-stu-id="5953b-112">[Get page][]</span></span>                    | <span data-ttu-id="5953b-113">获取/pages/{page-id}</span><span class="sxs-lookup"><span data-stu-id="5953b-113">GET /pages/{page-id}</span></span>
| <span data-ttu-id="5953b-114">[Create][]</span><span class="sxs-lookup"><span data-stu-id="5953b-114">[Create][]</span></span>                      | <span data-ttu-id="5953b-115">POST/pages</span><span class="sxs-lookup"><span data-stu-id="5953b-115">POST /pages</span></span>
| <span data-ttu-id="5953b-116">[删除][]</span><span class="sxs-lookup"><span data-stu-id="5953b-116">[Delete][]</span></span>                      | <span data-ttu-id="5953b-117">删除/pages/{page-id}</span><span class="sxs-lookup"><span data-stu-id="5953b-117">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="5953b-118">[发布][]</span><span class="sxs-lookup"><span data-stu-id="5953b-118">[Publish][]</span></span>                     | <span data-ttu-id="5953b-119">POST/pages/{page-id}/publish</span><span class="sxs-lookup"><span data-stu-id="5953b-119">POST /pages/{page-id}/publish</span></span>

[列出页面]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[获取页面]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[删除]: ../api/sitepage-delete.md
[Delete]: ../api/sitepage-delete.md
[发布]: ../api/sitepage-publish.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="5953b-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5953b-125">JSON representation</span></span>

<span data-ttu-id="5953b-126">下面是**sitePage**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5953b-126">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="5953b-127">属性</span><span class="sxs-lookup"><span data-stu-id="5953b-127">Properties</span></span>

<span data-ttu-id="5953b-128">**sitePage**资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="5953b-128">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="5953b-129">属性名称</span><span class="sxs-lookup"><span data-stu-id="5953b-129">Property name</span></span>    | <span data-ttu-id="5953b-130">类型</span><span class="sxs-lookup"><span data-stu-id="5953b-130">Type</span></span>                         | <span data-ttu-id="5953b-131">说明</span><span class="sxs-lookup"><span data-stu-id="5953b-131">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="5953b-132">contentType</span><span class="sxs-lookup"><span data-stu-id="5953b-132">contentType</span></span>      | <span data-ttu-id="5953b-133">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="5953b-133">[contentTypeInfo][]</span></span>          | <span data-ttu-id="5953b-134">页面的内容类型。</span><span class="sxs-lookup"><span data-stu-id="5953b-134">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="5953b-135">页面内容</span><span class="sxs-lookup"><span data-stu-id="5953b-135">Page Content</span></span>

<span data-ttu-id="5953b-136">**sitePage**资源具有以下内容字段。</span><span class="sxs-lookup"><span data-stu-id="5953b-136">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="5953b-137">属性名称</span><span class="sxs-lookup"><span data-stu-id="5953b-137">Property name</span></span>      | <span data-ttu-id="5953b-138">类型</span><span class="sxs-lookup"><span data-stu-id="5953b-138">Type</span></span>                       | <span data-ttu-id="5953b-139">说明</span><span class="sxs-lookup"><span data-stu-id="5953b-139">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="5953b-140">title</span><span class="sxs-lookup"><span data-stu-id="5953b-140">title</span></span>              | <span data-ttu-id="5953b-141">字符串</span><span class="sxs-lookup"><span data-stu-id="5953b-141">string</span></span>                     | <span data-ttu-id="5953b-142">页面的标题。</span><span class="sxs-lookup"><span data-stu-id="5953b-142">The title of the page.</span></span>
| <span data-ttu-id="5953b-143">pageLayout</span><span class="sxs-lookup"><span data-stu-id="5953b-143">pageLayout</span></span>         | <span data-ttu-id="5953b-144">string</span><span class="sxs-lookup"><span data-stu-id="5953b-144">string</span></span>                     | <span data-ttu-id="5953b-145">页面的页面布局的名称。</span><span class="sxs-lookup"><span data-stu-id="5953b-145">The name of the page layout of the page.</span></span>
| <span data-ttu-id="5953b-146">部件</span><span class="sxs-lookup"><span data-stu-id="5953b-146">webParts</span></span>           | <span data-ttu-id="5953b-147">[.webpart][]</span><span class="sxs-lookup"><span data-stu-id="5953b-147">[webPart][]</span></span>                | <span data-ttu-id="5953b-148">页面上的 web 部件。</span><span class="sxs-lookup"><span data-stu-id="5953b-148">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="5953b-149">创作元数据</span><span class="sxs-lookup"><span data-stu-id="5953b-149">Authoring Metadata</span></span>

<span data-ttu-id="5953b-150">**sitePage**资源具有以下与创作相关的元数据。</span><span class="sxs-lookup"><span data-stu-id="5953b-150">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="5953b-151">publishingState 属性将反映页面创作状态 (如 "已签出" 或 "已发布")。</span><span class="sxs-lookup"><span data-stu-id="5953b-151">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="5953b-152">属性名称</span><span class="sxs-lookup"><span data-stu-id="5953b-152">Property name</span></span>          | <span data-ttu-id="5953b-153">类型</span><span class="sxs-lookup"><span data-stu-id="5953b-153">Type</span></span>                   | <span data-ttu-id="5953b-154">说明</span><span class="sxs-lookup"><span data-stu-id="5953b-154">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="5953b-155">publishingState</span><span class="sxs-lookup"><span data-stu-id="5953b-155">publishingState</span></span>        | <span data-ttu-id="5953b-156">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="5953b-156">[publicationFacet][]</span></span>   | <span data-ttu-id="5953b-157">页面的发布状态和 MM.mm 版本。</span><span class="sxs-lookup"><span data-stu-id="5953b-157">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="5953b-158">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="5953b-158">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="5953b-159">属性名称</span><span class="sxs-lookup"><span data-stu-id="5953b-159">Property name</span></span>        | <span data-ttu-id="5953b-160">类型</span><span class="sxs-lookup"><span data-stu-id="5953b-160">Type</span></span>              | <span data-ttu-id="5953b-161">说明</span><span class="sxs-lookup"><span data-stu-id="5953b-161">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="5953b-162">id</span><span class="sxs-lookup"><span data-stu-id="5953b-162">id</span></span>                   | <span data-ttu-id="5953b-163">string</span><span class="sxs-lookup"><span data-stu-id="5953b-163">string</span></span>            | <span data-ttu-id="5953b-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="5953b-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="5953b-166">name</span><span class="sxs-lookup"><span data-stu-id="5953b-166">name</span></span>                 | <span data-ttu-id="5953b-167">string</span><span class="sxs-lookup"><span data-stu-id="5953b-167">string</span></span>            | <span data-ttu-id="5953b-168">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="5953b-168">The name / title of the item.</span></span>
| <span data-ttu-id="5953b-169">createdBy</span><span class="sxs-lookup"><span data-stu-id="5953b-169">createdBy</span></span>            | <span data-ttu-id="5953b-170">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5953b-170">[identitySet][]</span></span>   | <span data-ttu-id="5953b-171">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="5953b-171">Identity of the creator of this item.</span></span> <span data-ttu-id="5953b-172">只读。</span><span class="sxs-lookup"><span data-stu-id="5953b-172">Read-only.</span></span>
| <span data-ttu-id="5953b-173">eTag</span><span class="sxs-lookup"><span data-stu-id="5953b-173">eTag</span></span>                 | <span data-ttu-id="5953b-174">字符串</span><span class="sxs-lookup"><span data-stu-id="5953b-174">string</span></span>            | <span data-ttu-id="5953b-p106">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="5953b-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="5953b-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5953b-177">lastModifiedBy</span></span>       | <span data-ttu-id="5953b-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5953b-178">[identitySet][]</span></span>   | <span data-ttu-id="5953b-179">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="5953b-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="5953b-180">只读。</span><span class="sxs-lookup"><span data-stu-id="5953b-180">Read-only.</span></span>
| <span data-ttu-id="5953b-181">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5953b-181">lastModifiedDateTime</span></span> | <span data-ttu-id="5953b-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5953b-182">DateTimeOffset</span></span>    | <span data-ttu-id="5953b-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="5953b-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="5953b-185">parentReference</span><span class="sxs-lookup"><span data-stu-id="5953b-185">parentReference</span></span>      | <span data-ttu-id="5953b-186">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="5953b-186">[itemReference][]</span></span> | <span data-ttu-id="5953b-p109">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="5953b-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="5953b-189">WebUrl</span><span class="sxs-lookup"><span data-stu-id="5953b-189">webUrl</span></span>               | <span data-ttu-id="5953b-190">string (url)</span><span class="sxs-lookup"><span data-stu-id="5953b-190">string (url)</span></span>      | <span data-ttu-id="5953b-p110">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="5953b-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="5953b-193">关系</span><span class="sxs-lookup"><span data-stu-id="5953b-193">Relationships</span></span>

<span data-ttu-id="5953b-194">**sitePage**资源不具有与其他资源的关系。</span><span class="sxs-lookup"><span data-stu-id="5953b-194">The **sitePage** resource does not have relationships to other resources.</span></span>

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
