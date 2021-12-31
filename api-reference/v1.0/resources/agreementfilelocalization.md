---
title: agreementFileLocalization 资源类型
description: 表示本地协议使用条款的本地化策略Azure Active Directory (Azure AD) 。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 0f2e01a4832ed4f1d7da7a991238b8ef18c81fac
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651468"
---
# <a name="agreementfilelocalization-resource-type"></a>agreementFileLocalization 资源类型

命名空间：microsoft.graph

表示租户使用自定义协议文件管理的可自定义Azure Active Directory (Azure AD) 。 它包含有关协议文件的元数据 (例如，名称、语言以及它是否是协议文件的默认) 。

继承自 [agreementFileProperties](agreementfileproperties.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|表示文件创建时间的日期时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|displayName|String|协议的显示名称文件的本地化版本。 本地化显示名称向查看协议的最终用户显示。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|fileData|[agreementFileData](agreementfiledata.md)|表示 PDF 文档的使用条款的数据。 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|fileName|String|协议文件的名称 (例如，TOU.pdf) 。 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|id|String|agreementFileVersion 对象的标识符。 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|isDefault|Boolean|如果没有任何语言与客户端首选项匹配，则指示这是否是默认协议文件。 如果未将任何文件标记为默认文件，则第一个文件将被视为默认文件。 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|isMajorVersion|Boolean|指示协议文件是否是主要版本更新。 主要版本更新使协议在相应语言的接受无效。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|
|language|String|协议文件的语言，格式为"languagecode2-country/regioncode2"。 "languagecode2"是派生自 ISO 639-1 的两个字母小写代码，而"country/regioncode2"派生自 ISO 3166，通常包含两个小写字母或 BCP-47 语言标记。 例如，美国英语为 `en-US` 。 只读。 继承自 [agreementFileProperties](../resources/agreementfileproperties.md)。|


## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|版本|[agreementFileVersion](agreementfileversion.md) 集合|只读。 租户中的使用条款协议的自定义Azure AD版本。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileLocalization"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": "Boolean",
  "language": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileLocalization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
