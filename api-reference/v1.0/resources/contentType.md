---
author: daspek
description: ContentType 资源代表 SharePoint 中的内容类型。
title: contentType 资源类型
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 6c7c45b74088902f4f1565b52c96577cfcd6e3ca
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191343"
---
# <a name="contenttype-resource-type"></a>contentType 资源类型

命名空间：microsoft.graph


表示SharePoint中的内容类型。
通过内容类型，可以定义一组必须存在于 [**列表**][list]中每个 [**listItem**][listItem] 上的列。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出网站中的 contentTypes](../api/site-list-contenttypes.md)|[contentType](../resources/contenttype.md) 集合|获取 [contentType](../resources/contenttype.md) 对象及其 [在网站](../resources/site.md)中的属性的列表。|
|[列出列表中的 contentTypes](../api/list-list-contenttypes.md)|[contentType](../resources/contenttype.md) 集合|获取 [列表中 contentType](../resources/contenttype.md) 对象及其属性 [的列表](../resources/list.md)。|
|[为网站创建 contentType](../api/site-post-contenttypes.md)|[contentType](../resources/contenttype.md)|在[网站](../resources/site.md)中创建新的 [contentType](../resources/contenttype.md) 对象。|
|[获取 contentType](../api/contenttype-get.md)|[contentType](../resources/contenttype.md)|读取 [contentType](../resources/contenttype.md) 对象的属性和关系。|
|[更新 contentType](../api/contenttype-update.md)|[contentType](../resources/contenttype.md)|更新 [contentType](../resources/contenttype.md) 对象的属性。|
|[删除 contentType](../api/contenttype-delete.md)|无|删除 [contentType](../resources/contenttype.md) 对象。|
|[isPublished](../api/contenttype-ispublished.md)|Boolean| 检查是否已发布 [contentType](../resources/contenttype.md) 。|
|[发布](../api/contenttype-publish.md)|[contentType](../resources/contenttype.md)| 发布 [contentType](../resources/contenttype.md)。|
|[取消发布](../api/contenttype-unpublish.md)|[contentType](../resources/contenttype.md)|取消发布 [contentType](../resources/contenttype.md)。|
|[addCopy](../api/contenttype-addcopy.md)|[contentType](../resources/contenttype.md)|将 [contentType](../resources/contenttype.md) 的副本从 [网站](../resources/site.md) 添加到 [列表](../resources/list.md)。|
|[associateWithHubSites](../api/contenttype-associatewithhubsites.md)|[contentType](../resources/contenttype.md)|将 [contentType](../resources/contenttype.md) 与中心网站列表相关联。|
|[copyToDefaultContentLocation](../api/contenttype-copytodefaultcontentlocation.md)|[contentType](../resources/contenttype.md)| 将文件复制到 [contentType](../resources/contenttype.md) 中的默认内容位置。|
|[List columns](../api/contenttype-list-columns.md)|[columnDefinition](../resources/columnDefinition.md) 集合|获取 **contentType** 中表示为 [columnDefinition](../resources/columnDefinition.md) 资源的列的集合。|
|[创建列](../api/contenttype-post-columns.md)|[columnDefinition](../resources/columnDefinition.md)|将列添加到网站或列表中 **的内容类型** 。|
|[getCompatibleHubContentTypes](../api/contenttype-getcompatiblehubcontenttypes.md)|[contentType](../resources/contenttype.md) 集合|从内容类型中心获取可添加到目标 [网站](../resources/site.md) 或列表的兼容内容类型的 [列表](../resources/list.md)。|
|[addCopyFromContentTypeHub](../api/contenttype-addcopyfromcontenttypehub.md)|[contentType](../resources/contenttype.md)|将已发布内容类型的副本从内容类型中心添加或同步到目标 [网站](../resources/site.md) 或 [列表](../resources/list.md)。|


## <a name="properties"></a>属性

| 属性     | 类型                 | 说明|
|:------------------|:---------------------|:----------------------------------|
| associatedHubsUrls         | 集合 (字符串)  | 与此内容类型关联的中心网站的规范 URL 列表。 这将包含所有中心网站，其中此内容类型已排队以强制执行或已强制执行。 强制实施内容类型意味着内容类型将应用于强制网站中的列表。|
| 说明       | string               | 项目的描述性文本。|
| documentSet         | [documentSet][]      | [文档集](/sharepoint/governance/document-set-planning#about-document-sets) 元数据。|
| documentTemplate    | [documentSetContent][] | 文档模板元数据。 若要确保文档在网站及其子网站中具有一致的内容，可以将 Word、Excel 或PowerPoint 模板与网站内容类型相关联。|
| 组             | string               | 此内容类型所属的组的名称。 可以帮助组织相关的内容类型。|
| hidden            | Boolean              | 指示内容类型是否隐藏于此列表的“新建”菜单中。|
| id                | string               | 内容类型的唯一标识符。|
| inheritedFrom   | [itemReference][]    | 如果此内容类型继承自另一个作用域（如某个站点），则会提供对在其中定义内容类型的项的引用。|
| isBuiltIn            | Boolean| 指定内容类型是否为内置内容类型。 |
| name              | string               | 内容类型的名称。|
| 以             | [contentTypeOrder][] | 指定在选择 UI 中显示内容类型的顺序。|
| parentId          | string               | 内容类型的唯一标识符。|
| propagateChanges     | Boolean              | 如果 `true`对内容类型所做的任何更改都将推送到实现内容类型的继承内容类型和列表。|
| readOnly          | Boolean              | 如果 `true`是，除非此值首先设置为 `false`，否则无法修改内容类型。|
| sealed            | Boolean              | 如果 `true`用户或通过下推操作无法修改内容类型。 只有网站集管理员可以密封或解封内容类型。|


## <a name="relationships"></a>关系

| 关系    | 类型                      | 说明|
|:----------------|:--------------------------|:-------------------------------|
| 基地     | [contentType][]  | 从中派生此内容类型的父 contentType。 |
| columnLinks   | [columnLink][] 集合 | 此内容类型所需的列的集合。|
| baseTypes     | Collection([contentType][])     | 作为此内容类型的上级的内容类型的集合。|
| columnPositions         | Collection([columnDefinition][]) | 内容类型的列顺序信息。|
| columns       | Collection([columnDefinition][])  | 此 contentType 的列定义集合。|

有关详细信息，请参阅[内容类型和内容类型发布简介][contentTypeIntro]。

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md
[columnDefinition]: columnDefinition.md
[contentType]: contentType.md
[documentSet]: documentSet.md
[documentSetContent]: documentSetContent.md

## <a name="json-representation"></a>JSON 表示形式

以下是 **contentType** 资源的 JSON 表示形式。

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType","keyProperty":"id" } -->

```json
{
  "associatedHubsUrls" : ["string"],
  "base": { "@type": "microsoft.graph.contentType" },
  "baseTypes" : [{ "@type": "microsoft.graph.contentType" }],
  "columns" : [{ "@type": "microsoft.graph.columnDefinition" }],
  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }],
  "columnPositions" : [{ "@type": "microsoft.graph.columnDefinition" }],
  "description": "string",
  "documentSet" : { "@type": "microsoft.graph.documentSet" },
  "documentTemplate" : { "@type": "microsoft.graph.documentSetContent" },
  "group": "string",
  "hidden": false,
  "id": "string",
  "inheritedFrom": { "@type": "microsoft.graph.itemReference" },
  "isBuiltIn" : false,
  "name": "string",
  "order": { "@type": "microsoft.graph.contentTypeOrder" },
  "parentId": "string",
  "propagateChanges" : false,
  "readOnly": false,
  "sealed": false
}
```

[list]: list.md
[listItem]: listitem.md
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType",
  "suppressions": []
}
-->


