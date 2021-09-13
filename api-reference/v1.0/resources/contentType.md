---
author: daspek
description: ContentType 资源代表 SharePoint 中的内容类型。
title: contentType 资源类型
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 3acff5d1fe0661cee9d94ff96d8ffc7d470d624b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049625"
---
# <a name="contenttype-resource-type"></a>contentType 资源类型

命名空间：microsoft.graph


表示内容类型SharePoint。
内容类型允许您定义一组列，这些列必须存在于列表中的每个 [**listItem**][listItem] [**上**][list]。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出网站中的 contentTypes](../api/site-list-contenttypes.md)|[contentType](../resources/contenttype.md) 集合|获取网站 中的 [contentType](../resources/contenttype.md) 对象及其属性 [的列表](../resources/site.md)。|
|[列出列表中的 contentTypes](../api/list-list-contenttypes.md)|[contentType](../resources/contenttype.md) 集合|在列表中获取 [contentType](../resources/contenttype.md) 对象及其属性 [的列表](../resources/list.md)。|
|[为网站创建 contentType](../api/site-post-contenttypes.md)|[contentType](../resources/contenttype.md)|在网站 [中创建新的 contentType](../resources/contenttype.md) [对象](../resources/site.md)。|
|[获取 contentType](../api/contenttype-get.md)|[contentType](../resources/contenttype.md)|读取 [contentType](../resources/contenttype.md) 对象的属性和关系。|
|[更新 contentType](../api/contenttype-update.md)|[contentType](../resources/contenttype.md)|更新 [contentType 对象](../resources/contenttype.md) 的属性。|
|[删除 contentType](../api/contenttype-delete.md)|无|删除 [contentType](../resources/contenttype.md) 对象。|
|[isPublished](../api/contenttype-ispublished.md)|布尔值| 检查 [contentType 是否](../resources/contenttype.md) 发布。|
|[发布](../api/contenttype-publish.md)|[contentType](../resources/contenttype.md)| 发布 [contentType](../resources/contenttype.md)。|
|[取消发布](../api/contenttype-unpublish.md)|[contentType](../resources/contenttype.md)|取消发布 [contentType](../resources/contenttype.md)。|
|[addCopy](../api/contenttype-addcopy.md)|[contentType](../resources/contenttype.md)|将网站中的[contentType](../resources/contenttype.md) [副本添加到](../resources/site.md)[列表中](../resources/list.md)。|
|[associateWithHubSites](../api/contenttype-associatewithhubsites.md)|[contentType](../resources/contenttype.md)|将 [contentType](../resources/contenttype.md) 与中心网站列表关联。|
|[copyToDefaultContentLocation](../api/contenttype-copytodefaultcontentlocation.md)|[contentType](../resources/contenttype.md)| 将文件复制到 contentType 中的默认 [内容位置](../resources/contenttype.md)。|
|[List columns](../api/contenttype-list-columns.md)|[columnDefinition](../resources/columnDefinition.md) 集合|获取 contentType 中表示为 [columnDefinition](../resources/columnDefinition.md) 资源的 **列的集合**。|
|[创建列](../api/contenttype-post-columns.md)|[columnDefinition](../resources/columnDefinition.md)|向网站或 **列表中的内容** 类型添加列。|


## <a name="properties"></a>属性

| 属性名称     | 类型                 | 说明|
|:------------------|:---------------------|:----------------------------------|
| **说明**   | string               | 项目的描述性文本。|
| **group**         | string               | 此内容类型所属的组的名称。 可以帮助组织相关的内容类型。|
| **hidden**        | Boolean              | 指示内容类型是否隐藏于此列表的“新建”菜单中。|
| **id**            | string               | 内容类型的唯一标识符。|
| **inheritedFrom** | [itemReference][]    | 如果此内容类型继承自另一个作用域（如某个站点），则会提供对在其中定义内容类型的项的引用。|
| **name**          | string               | 内容类型的名称。|
| **order**         | [contentTypeOrder][] | 指定在选择 UI 中显示内容类型的顺序。|
| **parentId**      | string               | 内容类型的唯一标识符。|
| **readOnly**      | Boolean              | 如果 `true` 为 ，则不能修改内容类型，除非此值首先设置为 `false` 。|
| **sealed**        | Boolean              | 如果 `true` 为 ，则用户无法通过向下推送操作修改内容类型。 只有网站集管理员可以密封或解封内容类型。|
| **isBuiltIn**            | Boolean| 指定内容类型是否内置内容类型。 |
| **documentSet**       | [documentSet][]      | [文档集](/sharepoint/governance/document-set-planning#about-document-sets) 元数据。|
| **documentTemplate**  | [documentSetContent][] | 文档模板元数据。 若要确保文档在网站及其子网站中具有一致的内容，您可以将 Word、Excel 或 PowerPoint 模板与网站内容类型关联。|
| **associatedHubsUrls**       | 集合 (字符串)  | 与此内容类型关联的中心网站的规范 URL 列表。 这将包含此内容类型已排队以强制执行或已强制执行的所有中心网站。 强制实施内容类型意味着内容类型将应用于强制网站中的列表。|
| **propagateChanges**   | 布尔值              | 如果 `true` 为 ，则对内容类型进行的任何更改都将推送到实现该内容类型的继承内容类型和列表。|



## <a name="relationships"></a>关系

| 属性名称   | 类型                      | 说明|
|:----------------|:--------------------------|:-------------------------------|
| **base**   | [contentType][]  | 派生此内容类型的父 contentType。 |
| **columnLinks** | [columnLink][] 集合 | 此内容类型所需的列的集合。|
| **baseTypes**   | Collection([contentType][])     | 作为此内容类型的上级的内容类型的集合。|
| **columnPositions**       | Collection([columnDefinition][]) | 内容类型中的列顺序信息。|
| **columns**     | Collection([columnDefinition][])  | 此 contentType 的列定义集合。|

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

下面是 **contentType** 资源的 JSON 表示形式。

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType","keyProperty":"id" } -->

```json
{
  "description": "string",
  "group": "string",
  "hidden": false,
  "id": "string",
  "inheritedFrom": { "@type": "microsoft.graph.itemReference" },
  "name": "string",
  "order": { "@type": "microsoft.graph.contentTypeOrder" },
  "parentId": "string",
  "readOnly": false,
  "sealed": false,
  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }],
  "base": { "@type": "microsoft.graph.contentType" },
  "columnPositions" : [{ "@type": "microsoft.graph.columnDefinition" }],
  "isBuiltIn" : false,
  "documentSet" : { "@type": "microsoft.graph.documentSet" },
  "documentTemplate" : { "@type": "microsoft.graph.documentSetContent" },
  "associatedHubsUrls" : ["string"],
  "propagateChanges" : false,
  "baseTypes" : [{ "@type": "microsoft.graph.contentType" }],
  "columns" : [{ "@type": "microsoft.graph.columnDefinition" }]
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


