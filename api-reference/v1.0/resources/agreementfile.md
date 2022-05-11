---
title: agreementFile 资源类型
description: 表示租户使用 Azure Active Directory (Azure AD) 管理的可自定义使用条款协议文件。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: a48fa216ff9051e04bf57046387fd3e94619f7b2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314948"
---
# <a name="agreementfile-resource-type"></a>agreementFile 资源类型

命名空间：microsoft.graph

表示租户使用 Azure Active Directory (Azure AD) 管理的可自定义使用条款协议文件。 它包含有关协议文件 (的元数据，例如名称、语言以及它是否为默认文件) 。

继承自 [agreementFileProperties](agreementfileproperties.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|表示文件创建时间的日期时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|displayName|String|协议策略文件的本地化显示名称。 本地化显示名称将显示给查看协议的最终用户。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|fileData|[agreementFileData](agreementfiledata.md)|表示使用条款 PDF 文档的数据。 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|fileName|String|例如，协议文件的名称 (TOU.pdf) 。 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|id|String|agreementFileVersion 对象的标识符。 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|isDefault|Boolean|如果没有语言与客户端首选项匹配，则指示这是否是默认协议文件。 如果未将任何文件标记为默认文件，则第一个文件将被视为默认文件。 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|isMajorVersion|Boolean|指示协议文件是否为主要版本更新。 主要版本更新使协议对相应语言的接受无效。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|language|String|协议文件的语言，格式为“languagecode2-country/regioncode2”。 “languagecode2”是派生自 ISO 639-1 的小写双字母代码，而“country/regioncode2”派生自 ISO 3166，通常由两个大写字母或 BCP-47 语言标记组成。 例如，美国英语是 `en-US`. 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|定位|[agreementFileLocalization](agreementfilelocalization.md) 集合|附加到协议的使用条款协议文件的本地化版本。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.agreementFile",
  "keyProperty": "id"
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


