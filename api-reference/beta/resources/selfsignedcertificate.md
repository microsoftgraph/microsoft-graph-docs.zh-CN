---
title: selfSignedCertificate 资源类型
description: 包含有关签名证书的公共部分的信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: luleonpla
ms.openlocfilehash: a32720520c804d13048babe8a779132780abc782
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266862"
---
# <a name="selfsignedcertificate-resource-type"></a>selfSignedCertificate 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含签名证书的公共部分。 它是操作 [addSelfSignedSigningCertificate 的返回类型](../api/serviceprincipal-addtokensigningcertificate.md)。 服务提供商使用签名证书的公共部分来验证令牌的颁发者。

## <a name="properties"></a>属性
属性|类型|说明
----|--|---
|customKeyIdentifier|二进制| 自定义密钥标识符。 |
| displayName | String | 密钥的友好名称。 |
|endDateTime|DateTimeOffset|凭据过期的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。 |
|keyId|Guid|该密钥 (GUID) 标识符。|
|startDateTime|DateTimeOffset|凭据生效的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。 |
|type|String|密钥凭据的类型。 "AsymmetricX509Cert"。|
|usage|String|一个描述密钥的用途的字符串。 例如，"Verify"。|
|key|二进制| 密钥凭据的值。 应为 Base64 编码的值。 |
|thumbprint| String | 键的指纹值。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.selfSignedCertificate"
}-->

```json
{
    "customKeyIdentifier": "string (binary)",
    "displayName": "string",
    "endDateTime": "string (timestamp)",
    "key": "string (binary)",
    "keyId": "guid",
    "startDateTime": "String (timestamp)",
    "type": "string",
    "thumbprint":"string",
    "usage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "selfSignedCertificate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

