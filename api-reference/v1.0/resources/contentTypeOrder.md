---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
ms.openlocfilehash: fe7309373ded16fe2660e0c5a69773c18ffb581a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="contenttypeorder-resource-type"></a>ContentTypeOrder 资源类型

**contentTypeOrder** 资源指定 Content Type 将显示在选择 UI 中的顺序。

## <a name="json-representation"></a>JSON 表示形式

下面是 **contentTypeOrder** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a>属性

| 属性名称 | 类型    | 说明
|:--------------|:--------|:----------------------------------------------------
| **default**   | boolean | 这是否为默认的内容类型
| **position**  | Int32   | 指定在选择 UI 中显示内容类型的位置。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
