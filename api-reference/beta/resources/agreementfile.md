---
title: agreementFile 资源类型
description: 表示租户使用自定义协议文件管理的可自定义Azure Active Directory (Azure AD) 。 它包含有关协议文件的元数据 (例如，名称、语言以及它是否是协议文件的默认) 。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 041075c1d37b7f0eb8a7de83aab496c6d6fa0739
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451133"
---
# <a name="agreementfile-resource-type"></a>agreementFile 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户使用自定义协议文件管理的可自定义Azure Active Directory (Azure AD) 。 它包含有关协议文件的元数据 (例如，名称、语言以及它是否是协议文件的默认) 。

继承自 [agreementFileProperties](agreementfileproperties.md)。


## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|表示文件创建时间的日期时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|displayName|字符串|协议的显示名称文件的本地化版本。 本地化显示名称向查看协议的最终用户显示。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|fileData|[agreementFileData](agreementfiledata.md)|表示 PDF 文档的使用条款的数据。 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|fileName|String|协议文件的名称 (例如，TOU.pdf) 。 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|id|字符串|agreementFileVersion 对象的标识符。 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|isDefault|Boolean|如果没有任何语言与客户端首选项匹配，则指示这是否是默认协议文件。 如果未将任何文件标记为默认文件，则第一个文件将被视为默认文件。 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|isMajorVersion|布尔值|指示协议文件是否是主要版本更新。 主要版本更新使协议在相应语言的接受无效。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|language|String|协议文件的语言，格式为"languagecode2-country/regioncode2"。 "languagecode2"是派生自 ISO 639-1 的两个字母小写代码，而"country/regioncode2"派生自 ISO 3166，通常包含两个小写字母或 BCP-47 语言标记。 例如，美国英语为 `en-US`。 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|本地化|[agreementFileLocalization](agreementfilelocalization.md) 集合|附加到该协议的使用条款协议文件的本地化版本。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFile"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "language": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


