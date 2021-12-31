---
title: agreementFileProperties 资源类型
description: 表示使用条款协议文件的属性;包括本地化语言和显示名称。
author: raprakasMSFT
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e3c5ac4199d603f336c10dc732bc2f54110f7a3a
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650787"
---
# <a name="agreementfileproperties-resource-type"></a>agreementFileProperties 资源类型

命名空间：microsoft.graph

表示使用条款协议文件的属性;包括本地化语言和显示名称。

继承自 [实体](entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|表示文件创建时间的日期时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|displayName|String|协议的显示名称文件的本地化版本。 本地化显示名称向查看协议的最终用户显示。|
|fileData|[agreementFileData](agreementfiledata.md)|表示 PDF 文档的使用条款的数据。 只读。|
|fileName|String|协议文件的名称 (例如，TOU.pdf) 。 只读。|
|id|String|agreementFileVersion 对象的标识符。 只读。|
|isDefault|Boolean|如果没有任何语言与客户端首选项匹配，则指示这是否是默认协议文件。 如果未将任何文件标记为默认文件，则第一个文件将被视为默认文件。 只读。|
|isMajorVersion|Boolean|指示协议文件是否是主要版本更新。 主要版本更新使协议在相应语言的接受无效。|
|language|String|协议文件的语言，格式为"languagecode2-country/regioncode2"。 "languagecode2"是派生自 ISO 639-1 的两个字母小写代码，而"country/regioncode2"派生自 ISO 3166，通常包含两个小写字母或 BCP-47 语言标记。 例如，美国英语为 `en-US` 。 只读。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.agreementFileProperties",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.agreementFileProperties",
  "id": "String (identifier)",
  "fileName": "String",
  "language": "String",
  "isDefault": "Boolean",
  "isMajorVersion": "Boolean",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "fileData": {
    "@odata.type": "microsoft.graph.agreementFileData"
  }
}
```

