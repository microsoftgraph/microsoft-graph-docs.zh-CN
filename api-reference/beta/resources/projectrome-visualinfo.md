---
title: visualInfo 资源类型
description: 代表活动对象中的**visualElements**属性的复杂类型。
localization_priority: Normal
ms.openlocfilehash: 3e1dd3d7e4ecfaf5053f839f0ac0d0039692b2a4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855312"
---
# <a name="visualinfo-resource-type"></a>visualInfo 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表[活动](../resources/projectrome-activity.md)对象中的**visualElements**属性的复杂类型。

每个用户活动将在日程表中显示为自适应卡片。 鼓励提供用来捕获的活动的应用程序中发生的实质的自定义卡片将应用程序开发人员。 这是通过提供内容的属性中的自定义 JSON 卡片。

除了具有自适应卡片 visual 元数据，应用程序可指定内容元数据 – 为的数据用于根据用户的活动生成推断才能提供的将来重新新活动。 这是通过使用活动的 contentInfo 属性提供一个 JSON 对象，该利用 schema.org 属性来描述内容对象。

如果未提供的自定义卡片，则将生成的简单卡片使用显示文本和说明属性。 自定义卡建议展示从您的应用程序中的最佳内容。

## <a name="properties"></a>属性

|名称 | 类型 | Description|
|:----|:------|:-----------|
|显示文本 | 字符串 | 必需。 短用户的唯一活动 （例如，在其中活动是指创建文档的情况下的文档名称） 的文本的说明|
|说明 | 字符串 | 可选。 更长时间的用户的唯一的活动的文本说明 (示例： 文档名称、 第一句和/或元数据)|
|backgroundColor | 字符串 | 可选。 用于呈现 UI 的品牌颜色活动的应用程序源中的活动的背景色。 必须是有效的十六进制颜色|
|content | 类型化的 JSON 对象 | 可选。 自定义的数据的 JSON 对象，用于提供自定义呈现 Windows 命令行管理程序用户界面中的活动内容|
|属性 | [imageInfo](../resources/projectrome-imageinfo.md) | 可选。 JSON 对象，用于表示一个表示用于生成活动的应用程序图标|

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
    "@data.type": "microsoft.graph.visualInfo",
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
        "@data.type": "microsoft.graph.Json"
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
