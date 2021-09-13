---
title: visualInfo 资源类型
description: 表示活动对象中的 **visualElements** 属性的复杂类型。
ms.localizationpriority: medium
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: 3c71a3613c51c1b7494fd44550108d8cd63645ff
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019186"
---
# <a name="visualinfo-resource-type"></a>visualInfo 资源类型

命名空间：microsoft.graph

表示活动对象中的 **visualElements** [属性的复杂类型](../resources/projectrome-activity.md) 。

每个用户活动都将在时间线中显示为自适应卡片。 建议应用开发人员提供自定义卡片，以捕获应用中所发生活动的本质。 这一点在 content 属性中提供自定义 JSON 卡成为可能。

除了具有自适应卡片的可视元数据外，应用还可以指定内容元数据 – 用于生成用户活动推断的数据，以便提供新的活动供将来重新参与。 这通过使用活动的 contentInfo 属性来提供 JSON 对象，该对象利用 schema.org 描述内容。

如果未提供自定义卡片，则使用 displayText 和 description 属性生成简单卡片。 建议使用自定义卡片来展示应用中的最佳内容。

## <a name="properties"></a>属性

|名称 | 类型 | 说明|
|:----|:------|:-----------|
|displayText | String | 必填。 用户唯一活动实例的简短文本 (例如，在活动引用文档创建项目时的文档) |
|说明 | String | 可选。 用户唯一活动较长文本说明 (例如：文档名称、第一句和/或元数据) |
|backgroundColor | String | 可选。 用于在 UI 中呈现活动的背景颜色 - 活动的应用程序源的品牌颜色。 必须为有效的十六进制颜色|
|content | 未键入的 JSON 对象 | 可选。 自定义数据部分 - JSON 对象，用于提供自定义内容以在命令行管理程序 UI Windows活动|
|attribution | [imageInfo](../resources/projectrome-imageinfo.md) | 可选。 JSON 对象，用于表示表示用于生成活动的应用程序的图标|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

