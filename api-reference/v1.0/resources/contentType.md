---
author: daspek
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
description: ContentType 资源代表 SharePoint 中的内容类型。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1b307fb0b11b0608c15c46b618775dcef431815c4302a092e7e89f9cb7cb5942
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229288"
---
# <a name="contenttype-resource-type"></a>ContentType 资源类型

命名空间：microsoft.graph

**ContentType** 资源代表 SharePoint 中的 _内容类型_。
内容类型允许您定义一组列，这些列必须存在于列表中的每个 [**listItem**][listItem] [**上**][list]。

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a>JSON 表示形式

下面是 **contentType** 资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
 "baseType": "microsoft.graph.entity",
 "@odata.type": "microsoft.graph.contentType" } -->

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

  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }]
}
```

## <a name="properties"></a>属性

| 属性名称     | 类型                 | 说明
|:------------------|:---------------------|:----------------------------------
| **说明**   | string               | 项目的描述性文本。
| **group**         | string               | 此内容类型所属的组的名称。 可以帮助组织相关的内容类型。
| **hidden**        | boolean              | 指示内容类型是否隐藏于此列表的“新建”菜单中。
| **id**            | string               | 内容类型的唯一标识符。
| **inheritedFrom** | [itemReference][]    | 如果此内容类型继承自另一个作用域（如某个站点），则会提供对在其中定义内容类型的项的引用。
| **名称**          | string               | 内容类型的名称。
| **order**         | [contentTypeOrder][] | 指定在选择 UI 中显示内容类型的顺序。
| **parentId**      | string               | 内容类型的唯一标识符。
| **readOnly**      | boolean              | 如果为 `true`，则不能修改内容类型，除非此值首次设置为 `false`。
| **sealed**        | boolean              | 如果为 `true`，则不能由用户或通过下推操作修改内容类型。 只有网站集管理员可以密封或解封内容类型。

## <a name="relationships"></a>关系

| 属性名称   | 类型                      | 说明
|:----------------|:--------------------------|:-------------------------------
| **columnLinks** | [columnLink][] 集合 | 此内容类型所需的列集合

请参阅[内容类型和内容类型发布简介][contentTypeIntro]了解详细信息。

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath&quot;: &quot;Resources/ContentType"
} -->

