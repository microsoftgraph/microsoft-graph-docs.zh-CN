---
author: daspek
description: ContentType 资源代表 SharePoint 中的内容类型。
title: contentType
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 2af8291f33f62517e33349fb66408131f576e89a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444292"
---
# <a name="contenttype-resource-type"></a>contentType 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 SharePoint _中_ 的内容类型。
内容类型允许您定义一组列，这些列必须存在于列表中的每个 [**listItem**][listItem] [**上**][list]。

## <a name="properties"></a>属性

| 属性名称     | 类型                 | 说明
|:------------------|:---------------------|:----------------------------------
| **说明**   | string               | 项目的描述性文本。
| **group**         | string               | 此内容类型所属的组的名称。 可以帮助组织相关的内容类型。
| **hidden**        | Boolean              | 指示内容类型是否隐藏于此列表的“新建”菜单中。
| **id**            | string               | 内容类型的唯一标识符。
| **inheritedFrom** | [itemReference][]    | 如果此内容类型继承自另一个作用域（如某个站点），则会提供对在其中定义内容类型的项的引用。
| **名称**          | string               | 内容类型的名称。
| **order**         | [contentTypeOrder][] | 指定在选择 UI 中显示内容类型的顺序。
| **parentId**      | string               | 内容类型的唯一标识符。
| **readOnly**      | 布尔              | 如果为 `true`，则不能修改内容类型，除非此值首次设置为 `false`。
| **sealed**        | 布尔              | 如果为 `true`，则不能由用户或通过下推操作修改内容类型。 只有网站集管理员可以密封或解封内容类型。
| **isBuiltIn**            | 布尔| 指定内容类型是内置内容类型。 
| **documentSet**       | [documentSet][]      | [文档集](https://docs.microsoft.com/sharepoint/governance/document-set-planning#about-document-sets) 元数据。
| **documentTemplate**  | [documentSetContent][] | 文档模板元数据。 若要确保文档在网站及其子网站中具有一致的内容，可以将 Word、Excel 或 PowerPoint 模板与网站内容类型关联。
| **associatedHubsUrls**       | 集合 (字符串)  | 与此内容类型关联的中心网站的规范 URL 列表。 这将包含此内容类型已排入队列以强制执行或已强制执行的所有中心网站。 强制执行内容类型意味着内容类型将应用于强制网站中的列表。
| **propagateChanges**   | 布尔              | 如果 `true` ，对内容类型进行的任何更改都将推送到实现内容类型的继承内容类型和列表。



## <a name="relationships"></a>关系

| 属性名称   | 类型                      | 说明
|:----------------|:--------------------------|:-------------------------------
| **base**   | [contentType][]  | 派生此内容类型的父 contentType。 
| **columnLinks** | [columnLink][] 集合 | 此内容类型所需的列集合
| **baseTypes**   | Collection([contentType][])     | 作为此内容类型的上级的内容类型的集合。
| **columnPositions**       | Collection([columnDefinition][]) | 内容类型中的列顺序信息。
| **columns**     | Collection([columnDefinition][])  | 此 contentType 的列定义集合。

请参阅[内容类型和内容类型发布简介][contentTypeIntro]了解详细信息。

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


