---
title: agreementFile 资源类型
description: 表示使用协议文件租户管理使用 Azure Active Directory (Azure AD) 的可自定义术语。 它包含有关协议文件的元数据 (例如，名称、 语言，以及它是否为默认的文件)。
localization_priority: Normal
ms.openlocfilehash: 446173e83d32af96f938cbee15964ea204a62f7e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511427"
---
# <a name="agreementfile-resource-type"></a>agreementFile 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示使用协议文件租户管理使用 Azure Active Directory (Azure AD) 的可自定义术语。 它包含有关协议文件的元数据 (例如，名称、 语言，以及它是否为默认的文件)。

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
|fileData|[agreementFileData](agreementfiledata.md)|表示使用 PDF 文档中的条款的数据。 只读。|
|fileName|String|协议文件 (例如，TOU.pdf) 的名称。 只读。|
|id|String|只读。|
|isDefault|Boolean|指示是否这是默认协议文件，是否无区域性匹配的客户端首选项。 如果没有任何文件被标记为默认值，第一个将被视为默认值。 只读。|
|language|String|区域性格式 languagecode2-国家/地区/regioncode2 中的协议文件。 languagecode2 是小写字母双字母代码派生自 ISO 639-1。 国家/地区/regioncode2 派生自 ISO 3166，它通常包括两个大写字母或 BCP 47 语言标记 (例如，EN-US)。 只读。|

## <a name="relationships"></a>关系
无。


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
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementfile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
