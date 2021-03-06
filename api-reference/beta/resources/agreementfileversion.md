---
title: agreementFileVersion 资源类型
description: 表示 Azure Active Directory (Azure AD 协议使用条款的本地化策略文件的自定义) 。 它包含有关协议文件的元数据 (例如，名称、语言以及它是否是协议文件的默认) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: rajadineshmurugesan-microsoft
ms.openlocfilehash: afdfe9ce0e5440218919d0b019da6cbfe21a472f
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761889"
---
# <a name="agreementfileversion-resource-type"></a>agreementFileVersion 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户使用 Azure Active Directory 和 Azure AD (管理的使用条款协议文件的自定义) 。 它包含有关协议文件的元数据 (例如，名称、语言以及它是否是协议文件的默认) 。

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Create agreementFileLocalization](../api/agreementfilelocalization-post-agreementfilelocalizations.md) | [agreementfilelocalization](agreementfilelocalization.md) | Create a new agreementFileLocalization. |
| [List agreementFileLocalizations](../api/agreementfilelocalization-list.md) | [agreementfilelocalization](agreementfilelocalization.md) collection | Get an agreementFileLocalization object collection. |
| [Get agreementFileLocalization](../api/agreementfilelocalization-get.md) | [agreementfilelocalization](agreementfilelocalization.md) | Read properties and relationships of an agreementFileLocalization object. |
| [List agreementFileVersions](../api/agreementfileversion-list.md) | [agreementfileversion](agreementfileversion.md) collection | Get an agreementFileVersion object collection. |
| [Get agreementFileVersion](../api/agreementfileversion-get.md) | [agreementfileversion](agreementfileversion.md) | Read properties and relationships of an agreementFileVersion object. |
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
|createdDateTime|DateTimeOffset|表示文件创建时间的日期时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为："2014-01-01T00：00：00Z"。|
|displayName|String|协议的显示名称文件的本地化版本。 本地化显示名称向查看协议的最终用户显示。

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|versions|[agreementFileVersion](agreementfileversion.md) collection|The version history for the localized agreement file.|
-->

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileVersion"
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
