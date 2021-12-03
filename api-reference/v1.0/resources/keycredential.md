---
title: keyCredential 资源类型
description: 包含与应用程序或服务主体关联的密钥凭据。 application 和 servicePrincipal 实体的 **keyCredentials** 属性是 **keyCredential 的集合**。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: madansr7
ms.openlocfilehash: e08803389b9e24ab8a4214a4696f672e8167b71a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285110"
---
# <a name="keycredential-resource-type"></a>keyCredential 资源类型

命名空间：microsoft.graph

包含与应用程序或服务主体关联的密钥凭据。 application 和 [servicePrincipal](serviceprincipal.md)实体的 **keyCredentials** 属性是 **keyCredential 的集合**。 [](application.md)

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binary| 自定义密钥标识符 |
| displayName | String | 密钥的友好名称。 可选。 |
|endDateTime|DateTimeOffset|凭据过期的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|key|二进制| 转换为 Base64 字符串的字节数组中的证书原始数据;例如， `[System.Convert]::ToBase64String($Cert.GetRawCertData())` 。 |
|keyId|Guid|唯一标识符 (GUID) 的 GUID 值。|
|startDateTime|DateTimeOffset|凭据生效的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|type|String|密钥凭据的类型;例如， `Symmetric` 。|
|usage|String|一个描述密钥的用途的字符串;例如， `Verify` 。|

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
  "@odata.type": "#microsoft.graph.keyCredential",
  "customKeyIdentifier": "Binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "key": "Binary",
  "keyId": "Guid",
  "startDateTime": "String (timestamp)",
  "type": "String",
  "usage": "String"
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

