---
author: rahmit
description: 此资源表示 SitePages 列表中的页面。
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5562c0e60f0e36acf3621a160c1801d49661ea5c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440113"
---
# <a name="sitepage-resource"></a><span data-ttu-id="87a0e-103">sitePage 资源</span><span class="sxs-lookup"><span data-stu-id="87a0e-103">sitePage resource</span></span>

<span data-ttu-id="87a0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87a0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87a0e-105">此资源表示 SitePages 列表中的 [页面][]。</span><span class="sxs-lookup"><span data-stu-id="87a0e-105">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="87a0e-106">它包含标题、布局和 [Web 部件][]的集合。</span><span class="sxs-lookup"><span data-stu-id="87a0e-106">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="87a0e-107">页面上的任务</span><span class="sxs-lookup"><span data-stu-id="87a0e-107">Tasks on a page</span></span>

<span data-ttu-id="87a0e-108">以下任务可用于 **sitePage** 资源。</span><span class="sxs-lookup"><span data-stu-id="87a0e-108">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="87a0e-109">所有示例都相对于 [网站][];例如 `https://graph.microsoft.com/{api-version}/sites/{site-id}` ，。</span><span class="sxs-lookup"><span data-stu-id="87a0e-109">All examples are relative to a [site][]; for example, `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="87a0e-110">常见任务</span><span class="sxs-lookup"><span data-stu-id="87a0e-110">Common task</span></span>                     | <span data-ttu-id="87a0e-111">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="87a0e-111">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="87a0e-112">[列出页面][]</span><span class="sxs-lookup"><span data-stu-id="87a0e-112">[List pages][]</span></span>                  | <span data-ttu-id="87a0e-113">GET /pages</span><span class="sxs-lookup"><span data-stu-id="87a0e-113">GET /pages</span></span>
| <span data-ttu-id="87a0e-114">[获取页面][]</span><span class="sxs-lookup"><span data-stu-id="87a0e-114">[Get page][]</span></span>                    | <span data-ttu-id="87a0e-115">GET /pages/{page-id}</span><span class="sxs-lookup"><span data-stu-id="87a0e-115">GET /pages/{page-id}</span></span>
| <span data-ttu-id="87a0e-116">[创建][]</span><span class="sxs-lookup"><span data-stu-id="87a0e-116">[Create][]</span></span>                      | <span data-ttu-id="87a0e-117">POST /pages</span><span class="sxs-lookup"><span data-stu-id="87a0e-117">POST /pages</span></span>
| <span data-ttu-id="87a0e-118">[删除][]</span><span class="sxs-lookup"><span data-stu-id="87a0e-118">[Delete][]</span></span>                      | <span data-ttu-id="87a0e-119">DELETE /pages/{page-id}</span><span class="sxs-lookup"><span data-stu-id="87a0e-119">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="87a0e-120">[发布][]</span><span class="sxs-lookup"><span data-stu-id="87a0e-120">[Publish][]</span></span>                     | <span data-ttu-id="87a0e-121">POST /pages/{page-id}/publish</span><span class="sxs-lookup"><span data-stu-id="87a0e-121">POST /pages/{page-id}/publish</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="87a0e-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87a0e-127">JSON representation</span></span>

<span data-ttu-id="87a0e-128">下面是 **sitePage** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87a0e-128">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="87a0e-129">属性</span><span class="sxs-lookup"><span data-stu-id="87a0e-129">Properties</span></span>

<span data-ttu-id="87a0e-130">**sitePage** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="87a0e-130">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="87a0e-131">属性名称</span><span class="sxs-lookup"><span data-stu-id="87a0e-131">Property name</span></span>    | <span data-ttu-id="87a0e-132">类型</span><span class="sxs-lookup"><span data-stu-id="87a0e-132">Type</span></span>                         | <span data-ttu-id="87a0e-133">说明</span><span class="sxs-lookup"><span data-stu-id="87a0e-133">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="87a0e-134">contentType</span><span class="sxs-lookup"><span data-stu-id="87a0e-134">contentType</span></span>      | <span data-ttu-id="87a0e-135">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="87a0e-135">[contentTypeInfo][]</span></span>          | <span data-ttu-id="87a0e-136">页面的内容类型。</span><span class="sxs-lookup"><span data-stu-id="87a0e-136">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="87a0e-137">页面内容</span><span class="sxs-lookup"><span data-stu-id="87a0e-137">Page Content</span></span>

<span data-ttu-id="87a0e-138">**sitePage** 资源具有以下内容字段。</span><span class="sxs-lookup"><span data-stu-id="87a0e-138">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="87a0e-139">属性名称</span><span class="sxs-lookup"><span data-stu-id="87a0e-139">Property name</span></span>      | <span data-ttu-id="87a0e-140">类型</span><span class="sxs-lookup"><span data-stu-id="87a0e-140">Type</span></span>                       | <span data-ttu-id="87a0e-141">说明</span><span class="sxs-lookup"><span data-stu-id="87a0e-141">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="87a0e-142">title</span><span class="sxs-lookup"><span data-stu-id="87a0e-142">title</span></span>              | <span data-ttu-id="87a0e-143">字符串</span><span class="sxs-lookup"><span data-stu-id="87a0e-143">string</span></span>                     | <span data-ttu-id="87a0e-144">页面的标题。</span><span class="sxs-lookup"><span data-stu-id="87a0e-144">The title of the page.</span></span>
| <span data-ttu-id="87a0e-145">pageLayout</span><span class="sxs-lookup"><span data-stu-id="87a0e-145">pageLayout</span></span>         | <span data-ttu-id="87a0e-146">string</span><span class="sxs-lookup"><span data-stu-id="87a0e-146">string</span></span>                     | <span data-ttu-id="87a0e-147">页面的页面布局的名称。</span><span class="sxs-lookup"><span data-stu-id="87a0e-147">The name of the page layout of the page.</span></span>
| <span data-ttu-id="87a0e-148">webParts</span><span class="sxs-lookup"><span data-stu-id="87a0e-148">webParts</span></span>           | <span data-ttu-id="87a0e-149">[webPart][]</span><span class="sxs-lookup"><span data-stu-id="87a0e-149">[webPart][]</span></span>                | <span data-ttu-id="87a0e-150">页面上的 Web 部件。</span><span class="sxs-lookup"><span data-stu-id="87a0e-150">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="87a0e-151">创作元数据</span><span class="sxs-lookup"><span data-stu-id="87a0e-151">Authoring Metadata</span></span>

<span data-ttu-id="87a0e-152">**sitePage** 资源具有以下与创作相关的元数据。</span><span class="sxs-lookup"><span data-stu-id="87a0e-152">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="87a0e-153">**publishingState** 属性将反映页面创作状态，如已签出或已发布。</span><span class="sxs-lookup"><span data-stu-id="87a0e-153">The **publishingState** property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="87a0e-154">属性名称</span><span class="sxs-lookup"><span data-stu-id="87a0e-154">Property name</span></span>          | <span data-ttu-id="87a0e-155">类型</span><span class="sxs-lookup"><span data-stu-id="87a0e-155">Type</span></span>                   | <span data-ttu-id="87a0e-156">说明</span><span class="sxs-lookup"><span data-stu-id="87a0e-156">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="87a0e-157">publishingState</span><span class="sxs-lookup"><span data-stu-id="87a0e-157">publishingState</span></span>        | <span data-ttu-id="87a0e-158">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="87a0e-158">[publicationFacet][]</span></span>   | <span data-ttu-id="87a0e-159">页面的MM.mm和发布版本。</span><span class="sxs-lookup"><span data-stu-id="87a0e-159">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="87a0e-160">以下属性继承自 **[baseItem][]**。</span><span class="sxs-lookup"><span data-stu-id="87a0e-160">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="87a0e-161">属性名称</span><span class="sxs-lookup"><span data-stu-id="87a0e-161">Property name</span></span>        | <span data-ttu-id="87a0e-162">类型</span><span class="sxs-lookup"><span data-stu-id="87a0e-162">Type</span></span>              | <span data-ttu-id="87a0e-163">说明</span><span class="sxs-lookup"><span data-stu-id="87a0e-163">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="87a0e-164">id</span><span class="sxs-lookup"><span data-stu-id="87a0e-164">id</span></span>                   | <span data-ttu-id="87a0e-165">string</span><span class="sxs-lookup"><span data-stu-id="87a0e-165">string</span></span>            | <span data-ttu-id="87a0e-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="87a0e-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="87a0e-168">name</span><span class="sxs-lookup"><span data-stu-id="87a0e-168">name</span></span>                 | <span data-ttu-id="87a0e-169">string</span><span class="sxs-lookup"><span data-stu-id="87a0e-169">string</span></span>            | <span data-ttu-id="87a0e-170">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="87a0e-170">The name / title of the item.</span></span>
| <span data-ttu-id="87a0e-171">createdBy</span><span class="sxs-lookup"><span data-stu-id="87a0e-171">createdBy</span></span>            | <span data-ttu-id="87a0e-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="87a0e-172">[identitySet][]</span></span>   | <span data-ttu-id="87a0e-173">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="87a0e-173">Identity of the creator of this item.</span></span> <span data-ttu-id="87a0e-174">只读。</span><span class="sxs-lookup"><span data-stu-id="87a0e-174">Read-only.</span></span>
| <span data-ttu-id="87a0e-175">eTag</span><span class="sxs-lookup"><span data-stu-id="87a0e-175">eTag</span></span>                 | <span data-ttu-id="87a0e-176">字符串</span><span class="sxs-lookup"><span data-stu-id="87a0e-176">string</span></span>            | <span data-ttu-id="87a0e-p106">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="87a0e-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="87a0e-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="87a0e-179">lastModifiedBy</span></span>       | <span data-ttu-id="87a0e-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="87a0e-180">[identitySet][]</span></span>   | <span data-ttu-id="87a0e-181">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="87a0e-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="87a0e-182">只读。</span><span class="sxs-lookup"><span data-stu-id="87a0e-182">Read-only.</span></span>
| <span data-ttu-id="87a0e-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87a0e-183">lastModifiedDateTime</span></span> | <span data-ttu-id="87a0e-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87a0e-184">DateTimeOffset</span></span>    | <span data-ttu-id="87a0e-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="87a0e-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="87a0e-187">parentReference</span><span class="sxs-lookup"><span data-stu-id="87a0e-187">parentReference</span></span>      | <span data-ttu-id="87a0e-188">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="87a0e-188">[itemReference][]</span></span> | <span data-ttu-id="87a0e-189">父信息（如果此项具有父级）。</span><span class="sxs-lookup"><span data-stu-id="87a0e-189">Parent information, if the item has a parent.</span></span> <span data-ttu-id="87a0e-190">只读。</span><span class="sxs-lookup"><span data-stu-id="87a0e-190">Read-only.</span></span>
| <span data-ttu-id="87a0e-191">WebUrl</span><span class="sxs-lookup"><span data-stu-id="87a0e-191">webUrl</span></span>               | <span data-ttu-id="87a0e-192">string (url)</span><span class="sxs-lookup"><span data-stu-id="87a0e-192">string (url)</span></span>      | <span data-ttu-id="87a0e-p110">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="87a0e-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="87a0e-195">关系</span><span class="sxs-lookup"><span data-stu-id="87a0e-195">Relationships</span></span>

<span data-ttu-id="87a0e-196">**sitePage** 资源与其他资源没有关系。</span><span class="sxs-lookup"><span data-stu-id="87a0e-196">The **sitePage** resource does not have relationships to other resources.</span></span>

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


