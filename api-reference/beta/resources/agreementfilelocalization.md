---
title: agreementFileLocalization 资源类型
description: 表示 Azure Active Directory (Azure AD) 中的使用条款协议的本地化策略文件。 它包含有关协议文件的元数据 (例如，名称、语言以及它是否为默认文件) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 63d498b37980a57b3653b41cb337e792b8c1a838
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/12/2020
ms.locfileid: "46644024"
---
# <a name="agreementfilelocalization-resource-type"></a>agreementFileLocalization 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户使用 Azure Active Directory (Azure AD) 管理的可自定义使用条款协议文件。 它包含有关协议文件的元数据 (例如，名称、语言以及它是否为默认文件) 。

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
|fileData|[agreementFileData](agreementfiledata.md)|代表使用条款的 PDF 文档的数据。 只读。|
|fileName|String|协议文件的名称 (例如，TOU.pdf) 。 只读。|
|id|String|只读。|
|isDefault|Boolean|指示是否为默认协议文件（如果没有任何区域性与客户端首选项匹配）。 如果没有任何文件被标记为默认值，则第一个文件将被视为默认值。 只读。|
|language|String|协议文件的区域性（格式为 languagecode2/regioncode2）。 languagecode2 是从 ISO 639-1 派生的一个由两个小写字母组成的代码。 国家/regioncode2 派生自 ISO 3166，通常包含两个大写字母或一个 BCP-47 语言标记 (例如 en-us) 。 只读。|


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
  "isDefault": true,
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
