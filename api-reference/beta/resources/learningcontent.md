---
title: learningContent 资源类型
description: 表示包含有关学习内容的详细信息的实体。
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: resourcePageType
ms.openlocfilehash: 865070a402c68327a1fef41b6c793e5672f878c3
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883257"
---
# <a name="learningcontent-resource-type"></a>learningContent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示员工学习内容的元数据。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 learningContents](../api/learningprovider-list-learningcontents.md)|[learningContent](../resources/learningcontent.md) 集合|获取 [learningContent](../resources/learningcontent.md) 资源及其属性的列表。 此列表表示Viva Learning中指定提供程序内容的元数据。|
|[获取 learningContent](../api/learningcontent-get.md)|[learningContent](../resources/learningcontent.md)|获取指定的 learningContent 资源，该资源表示指定提供程序的引入内容的元数据。|
|[更新 learningContent](../api/learningcontent-update.md)|[learningContent](../resources/learningcontent.md)|更新指定的 [learningContent](../resources/learningcontent.md) 资源。 [学习提供程序](learningprovider.md)用于在Viva Learning中引入或更新其内容的元数据。|
|[删除 learningContent](../api/learningprovider-delete-learningcontents.md)|无|删除表示指定提供程序引入内容的元数据的指定 learningContent 资源。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|additionalTags|字符串集合|与学习内容关联的关键字、主题和其他标记。 可选。|
|contentWebUrl|String|学习内容的内容 Web URL。 必需。|
|贡献|String|学习内容的作者、创建者或参与者。 可选。|
|createdDateTime|DateTimeOffset|创建学习内容的日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 可选。|
|说明|String|学习内容的说明或摘要。 可选。|
|duration|持续时间|学习内容的持续时间（以秒为单位）。 可选。|
|externalId|String|学习内容的唯一外部内容 ID。 必需。|
|format|String|学习内容的格式。 例如， ， `Course``Video`， `Book`， `Book Summary`。 `Audiobook Summary` 可选。|
|isActive|布尔|指示内容是否处于活动状态。 非活动内容不会显示在 UI 中。 默认值为 `true`。 可选。|
|isPremium|布尔|指示学习内容是否要求用户在学习提供程序平台上登录。 默认值为 `false`。 可选。|
|isSearchable|布尔|指示学习内容是否可搜索。 默认值为 `true`。 可选。|
|languageTag|String|学习内容的语言，例如， `en-us` 或 `fr-fr`。 必需。|
|lastModifiedDateTime|DateTimeOffset|上次修改学习内容的日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 可选。|
|numberOfPages|Int32|学习内容的页数，例如 9。 可选。|
|skillTags|字符串集合|与学习内容关联的技能标记。 可选。|
|sourceName|String|学习内容的源名称，例如 `LinkedIn Learning` 或 `Coursera`。 可选。|
|thumbnailWebUrl|String|学习内容缩略图图像的 URL。 可选。|
|title|String|学习内容的标题。 必填。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.learningContent",
  "openType": false
}
-->
``` json
{
    "@odata.type": "#microsoft.graph.learningContent",
    "additionalTags": [
        "String"
    ],
    "contentWebUrl": "String",
    "contributor": "String",
    "createdDateTime": "String (timestamp)",
    "description": "String",
    "duration": "String (duration)",
    "externalId": "String",
    "format": "String",
    "isActive": "Boolean",
    "isPremium": "Boolean",
    "isSearchable": "Boolean",
    "languageTag": "String",
    "lastModifiedDateTime": "String (timestamp)",
    "numberOfPages": "Integer",
    "skillTags": [
        "String"
    ],
    "sourceName": "String",
    "thumbnailWebUrl": "String",
    "title": "String"
}
```

