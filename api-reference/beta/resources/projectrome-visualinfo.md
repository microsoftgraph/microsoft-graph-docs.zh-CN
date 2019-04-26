---
title: visualInfo 资源类型
description: 一个代表 activity 对象中的**visualElements**属性的复杂类型。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 56d3822c89de074847aeab6c8a0a742ecd7f006f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563358"
---
# <a name="visualinfo-resource-type"></a>visualInfo 资源类型

一个代表[activity](../resources/projectrome-activity.md)对象中的**visualElements**属性的复杂类型。

每个用户活动将在时间轴中显示为一个自适应卡片。 鼓励应用程序开发人员提供自定义卡片, 以捕获应用程序中发生的活动的实质。 可通过在 content 属性中提供自定义 JSON 卡片来实现这一点。

除了具有自适应卡片的可视元数据之外, 应用还可以指定内容元数据–用于在用户活动上建立推断的数据, 以便为将来的重新约定提供新活动。 为此, 可以使用活动的 contentInfo 属性提供一个 JSON 对象, 该对象利用 schema.org 属性来描述内容。

如果未提供自定义卡片, 将使用 "文本" 和 "说明" 属性生成一个简单的卡片。 建议使用自定义卡片展示应用程序中的最佳内容。

## <a name="properties"></a>属性

|名称 | 类型 | 说明|
|:----|:------|:-----------|
|displayText | String | 必需。 用户独特活动的简短文本说明 (例如, 活动引用文档创建时的文档名称)|
|说明 | String | 可选。 用户独特活动的更长文本说明 (示例: 文档名称、第一句和/或元数据)|
|backgroundColor | String | 可选。 用于呈现活动的应用程序源的 UI 品牌颜色中的活动的背景色。 必须是有效的十六进制颜色|
|content | 非类型化 JSON 对象 | 可选。 用于提供自定义内容以在 Windows Shell UI 中呈现活动的自定义数据 JSON 对象块|
|attribution | [imageInfo](../resources/projectrome-imageinfo.md) | 可选。 JSON 对象, 用于表示表示用于生成活动的应用程序的图标|

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
