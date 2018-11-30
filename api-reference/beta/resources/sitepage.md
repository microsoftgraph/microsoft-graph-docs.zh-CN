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
# <a name="sitepage-resource"></a>sitePage 资源

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

此资源代表 SitePages[列表][]中的页面。
它包含标题、 布局和[web 部件][]s 的集合。

## <a name="tasks-on-a-page"></a>页面上的任务

为**sitePage**资源提供了下列任务。
下面的所有示例都是相对于[网站][]，如： `https://graph.microsoft.com/{api-version}/sites/{site-id}`。

| 常见任务                     | HTTP 方法
|:--------------------------------|:------------------------------
| [List pages][]                  | 获取 /pages
| [Get page][]                    | 获取 /pages/ {页-id}
| [Create][]                      | POST /pages
| [删除][]                      | 删除 /pages/ {页-id}
| [Publish][]                     | 发布 /pages/ {页-id} / 发布

[List pages]: ../api/sitepage-list.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[删除]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a>JSON 表示形式

下面是**sitePage**资源的 JSON 表示形式。

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

## <a name="properties"></a>属性

**SitePage**资源具有以下属性。

| 属性名    | 类型                         | 说明
|:-----------------|:-----------------------------|:---------------------------
| contentType      | [contentTypeInfo][]          | 页面内容类型。

## <a name="page-content"></a>页面内容

**SitePage**资源具有以下内容的字段。

| 属性名      | 类型                       | 说明
|:-------------------|:---------------------------|:---------------------------
| title              | 字符串                     | 页面的标题。
| pageLayout         | string                     | 页的页面布局的名称。
| web 部件           | [web 部件][]                | Web 部件页上。

## <a name="authoring-metadata"></a>创作元数据

**SitePage**资源具有创作相关的以下元数据。 PublishingState 属性将反映创作 like 签出或发布的状态页。

| 属性名          | 类型                   | 说明
|:-----------------------|:-----------------------|:---------------------------
| publishingState        | [publicationFacet][]   | 发布状态和页的 MM.mm 版本。

以下属性继承自 ** [baseItem][]**。

| 属性名称        | 类型              | 说明
|:---------------------|:------------------|:----------------------------------
| ID                   | string            | 项的唯一标识符。只读。
| name                 | string            | 项目名称/标题。
| createdBy            | [identitySet][]   | 此项的创建者的标识。 只读。
| eTag                 | string            | 该项目的 ETag。只读。
| lastModifiedBy       | [identitySet][]   | 此项的最后一个修饰符的标识。 只读。
| lastModifiedDateTime | DateTimeOffset    | 上次修改项目的日期和时间。只读。
| parentReference      | [itemReference][] | 上次修改项目的日期和时间。只读。
| WebUrl               | string (url)      | 在浏览器中显示此项目的 URL。只读。

## <a name="relationships"></a>关系

**SitePage**资源没有与其他资源的关系。

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
