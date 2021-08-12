---
title: agreementFile 资源类型
description: 表示租户使用 Azure AD Azure Active Directory (管理的可自定义使用条款) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 24398d61e8a269615cdf6ad4ef1d15ea587be78680fd0da3bb1b57f8a17a9ecf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54147131"
---
# <a name="agreementfile-resource-type"></a>agreementFile 资源类型

命名空间：microsoft.graph

表示租户使用 Azure AD Azure Active Directory (管理的可自定义使用条款) 。 它包含有关协议文件的元数据 (例如，名称、语言以及它是否是协议文件的默认) 。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|fileData|[agreementFileData](agreementfiledata.md)|表示 PDF 文档的使用条款的数据。 只读。|
|fileName|String|协议文件的名称 (例如，TOU.pdf) 。 只读。|
|id|String|协议文件的标识符。 只读。|
|isDefault|Boolean|如果没有任何语言与客户端首选项匹配，则指示这是默认协议文件。 如果未将任何文件标记为默认文件，则第一个文件将被视为默认文件。 只读。|
|language|String|协议文件的语言，格式为 languagecode2-country/regioncode2。 languagecode2 是从 ISO 639-1 派生的两个字母小写代码。 country/regioncode2 派生自 ISO 3166，通常由两个小写字母或 BCP-47 语言标记 (例如 en-US) 。 只读。|
|isMajorVersion|Boolean|指示协议文件是否是主要版本更新。 主要版本更新使协议在相应语言的接受无效。 |
|createdDateTime|DateTimeOffset|表示文件创建时间的日期时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。|
|displayName|String|协议的显示名称文件的本地化版本。 本地化显示名称向查看协议的最终用户显示。

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|localizations|[agreementFileLocalization](agreementfilelocalization.md) collection|The localized version of the agreement files attached to the agreement.|
-->

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


