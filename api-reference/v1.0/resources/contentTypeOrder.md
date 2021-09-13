---
author: daspek
ms.date: 09/13/2017
title: ContentTypeOrder
ms.localizationpriority: medium
description: contentTypeOrder 资源指定在选择 UI 中显示内容类型的顺序。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: be84be025a17677fa6c8546b1a7ccc9f1b3122c0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049590"
---
# <a name="contenttypeorder-resource-type"></a>ContentTypeOrder 资源类型

命名空间：microsoft.graph

**contentTypeOrder** 资源指定在选择 UI 中显示内容类型的顺序。

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

