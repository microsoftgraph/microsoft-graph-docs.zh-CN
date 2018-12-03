---
title: agreementFile 资源类型
description: 表示使用协议文件租户管理使用 Azure Active Directory (Azure AD) 的可自定义术语。 它包含有关协议文件的元数据 (例如，名称、 语言，以及它是否为默认的文件)。
ms.openlocfilehash: f099715fd25fbae9d7b2a94d6de841b8766c30e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045277"
---
# <a name="agreementfile-resource-type"></a>agreementFile 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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
| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|fileData|[agreementFileData](agreementfiledata.md)|表示使用 PDF 文档中的条款的数据。 只读。|
|fileName|String|协议文件 (例如，TOU.pdf) 的名称。 只读。|
|id|String|只读。|
|isDefault|布尔|指示是否这是默认协议文件，是否无区域性匹配的客户端首选项。 如果没有任何文件被标记为默认值，第一个将被视为默认值。 只读。|
|language|String|区域性格式 languagecode2-国家/地区/regioncode2 中的协议文件。 languagecode2 是小写字母双字母代码派生自 ISO 639-1。 国家/地区/regioncode2 派生自 ISO 3166，它通常包括两个大写字母或 BCP 47 语言标记 (例如，EN-US)。 只读。|

## <a name="relationships"></a>Relationships
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
<!-- {
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
