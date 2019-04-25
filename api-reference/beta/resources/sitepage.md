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
# <a name="sitepage-resource"></a>sitePage 资源

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

此资源表示 "SitePages"[列表][]中的页面。
它包含[web 部件][]s 的标题、布局和集合。

## <a name="tasks-on-a-page"></a>页面上的任务

以下任务可用于**sitePage**资源。
下面的所有示例都是相对于[网站][]而言的`https://graph.microsoft.com/{api-version}/sites/{site-id}`, 例如:。

| 常见任务                     | HTTP 方法
|:--------------------------------|:------------------------------
| [列出页面][]                  | 获取/pages
| [获取页面][]                    | 获取/pages/{page-id}
| [创建][]                      | POST/pages
| [删除][]                      | 删除/pages/{page-id}
| [发布][]                     | POST/pages/{page-id}/publish

[列出页面]: ../api/sitepage-list.md
[获取页面]: ../api/sitepage-get.md
[创建]: ../api/sitepage-create.md
[删除]: ../api/sitepage-delete.md
[发布]: ../api/sitepage-publish.md

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

**sitePage**资源具有以下属性。

| 属性名称    | 类型                         | 说明
|:-----------------|:-----------------------------|:---------------------------
| contentType      | [contentTypeInfo][]          | 页面的内容类型。

## <a name="page-content"></a>页面内容

**sitePage**资源具有以下内容字段。

| 属性名称      | 类型                       | 说明
|:-------------------|:---------------------------|:---------------------------
| title              | 字符串                     | 页面的标题。
| pageLayout         | string                     | 页面的页面布局的名称。
| 部件           | [.webpart][]                | 页面上的 web 部件。

## <a name="authoring-metadata"></a>创作元数据

**sitePage**资源具有以下与创作相关的元数据。 publishingState 属性将反映页面创作状态 (如 "已签出" 或 "已发布")。

| 属性名称          | 类型                   | 说明
|:-----------------------|:-----------------------|:---------------------------
| publishingState        | [publicationFacet][]   | 页面的发布状态和 MM.mm 版本。

以下属性继承自 ** [baseItem][]**。

| 属性名称        | 类型              | 说明
|:---------------------|:------------------|:----------------------------------
| id                   | string            | 项的唯一标识符。只读。
| name                 | string            | 项目名称/标题。
| createdBy            | [identitySet][]   | 此项的创建者的标识。 只读。
| eTag                 | 字符串            | 该项目的 ETag。只读。
| lastModifiedBy       | [identitySet][]   | 此项的最后一个修饰符的标识。 只读。
| lastModifiedDateTime | DateTimeOffset    | 上次修改项目的日期和时间。只读。
| parentReference      | [itemReference][] | 上次修改项目的日期和时间。只读。
| webUrl               | string (url)      | 在浏览器中显示此项目的 URL。只读。

## <a name="relationships"></a>关系

**sitePage**资源不具有与其他资源的关系。

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
[.webpart]: webpart.md

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
