---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
ms.openlocfilehash: ee869e5f2925af92fea9eef04fd26ec483baad5b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="contenttype-resource-type"></a>ContentType 资源类型

**contentType** 资源表示 SharePoint 中的_内容类型_。
内容类型允许定义一组列，这些列必须显示在 [**list**][list] 中的每个 [**listItem**][listItem] 上。

[list]: list.md
[listItem]: listItem.md

## <a name="json-representation"></a>JSON 表示形式

下面是 **contentType** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType" } -->

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
| **description**   | string               | 项目的描述性文本。
| **group**         | string               | 此内容类型所属组的名称。 帮助组织相关的内容类型。
| **hidden**        | boolean              | 指示内容类型是否在列表的“新建”菜单中隐藏。
| **id**            | string               | 内容类型的唯一标识符。
| **inheritedFrom** | [itemReference][]    | 如果此内容类型继承自另一个范围（如网站），则提供对定义内容类型的项的引用。
| **name**          | string               | 内容类型的名称。
| **order**         | [contentTypeOrder][] | 指定内容类型出现在选择 UI 中的顺序。
| **parentId**      | string               | 内容类型的唯一标识符。
| **readOnly**      | boolean              | 如果值为 `true`，则无法修改内容类型，除非首先将此值设为 `false`。
| **sealed**        | boolean              | 如果值为 `true`，则无法由用户或通过下推操作修改内容类型。 只有网站集管理员才能封装或解封内容类型。

## <a name="relationships"></a>关系

| 属性名称   | 类型                      | 说明
|:----------------|:--------------------------|:-------------------------------
| **columnLinks** | [columnLink][] 集合 | 此内容类型所需列的集合

有关详细信息，请参阅[内容类型和内容类型发布简介][contentTypeIntro]。

[columnLink]: columnLink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemReference.md
[contentTypeOrder]: contentTypeOrder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->
