---
title: keyCredential 资源类型
description: 包含与应用程序或服务主体关联的密钥凭据。 **应用程序和 servicePrincipal 实体的 keyCredentials** 属性是 **keyCredential 的集合**。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: cc6d66a4361f760b702844991e6fdc3f590c4007
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721486"
---
# <a name="keycredential-resource-type"></a>keyCredential 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含与应用程序或服务主体关联的密钥凭据。 应用程序和 [](application.md)[servicePrincipal](serviceprincipal.md)实体的 **keyCredentials** 属性是 **keyCredential 的集合**。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binary| 自定义密钥标识符 |
| displayName | String | 密钥的友好名称。 可选。 |
|endDateTime|DateTimeOffset|凭据过期的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|keyId|Guid|该密钥 (GUID) 标识符。|
|startDateTime|DateTimeOffset|凭据生效的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|type|String|密钥凭据的类型;例如，"Symmetric"。|
|usage|String|描述密钥的用途的字符串;例如，"Verify"。|
|key|二进制| 密钥凭据的值。 应为 Base 64 编码值。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


