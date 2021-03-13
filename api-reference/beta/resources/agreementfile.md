---
title: agreementFile 资源类型
description: 表示租户使用 Azure Active Directory 和 Azure AD (管理的可自定义) 。 它包含有关协议文件的元数据 (例如，名称、语言以及它是否是协议文件的默认) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: cd65009ef76c6872b08840157c56255107670bfd
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761875"
---
# <a name="agreementfile-resource-type"></a>agreementFile 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户使用 Azure Active Directory 和 Azure AD (管理的可自定义) 。 它包含有关协议文件的元数据 (例如，名称、语言以及它是否是协议文件的默认) 。

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|fileData|[agreementFileData](agreementfiledata.md)|表示 PDF 文档的使用条款的数据。 只读。|
|fileName|String|协议文件的名称 (例如，TOU.pdf) 。 只读。|
|id|String|只读。|
|isDefault|Boolean|指示当没有任何区域性与客户端首选项匹配时，这是否是默认协议文件。 如果没有文件标记为默认文件，则第一个文件将被视为默认文件。 只读。|
|language|String|格式为 languagecode2-country/regioncode2 的协议文件的区域性。 languagecode2 是从 ISO 639-1 派生的两个字母小写代码。 country/regioncode2 派生自 ISO 3166，通常由两个小写字母或 BCP-47 语言标记 (例如 en-US) 。 只读。|
|isMajorVersion|布尔|指示协议文件是否是主要版本更新。 主要版本更新使协议在相应语言的接受无效。 |
|createdDateTime|DateTimeOffset|表示文件创建时间的日期时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为："2014-01-01T00：00：00Z"。|
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


