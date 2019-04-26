---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
ms.openlocfilehash: bf35a3cbeee8003db8ed121e5bafbc88df098d9a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341237"
---
# <a name="contenttype-resource-type"></a>ContentType 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ContentType** 资源代表 SharePoint 中的_内容类型_。
内容类型使你可以定义一组列，这些列必须存在于 [**list**][list] 中的每个 [**listItem**][listItem] 上。

[list]: list.md
[listItem]: listitem.md

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
| **name**          | string               | 内容类型的名称。
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
