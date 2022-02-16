---
title: selfSignedCertificate 资源类型
description: 包含有关签名证书的公共部分的信息。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: alamaral
ms.openlocfilehash: 281c3881d02548e3a1146bba140c8a7514b65a3c
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62853940"
---
# <a name="selfsignedcertificate-resource-type"></a>selfSignedCertificate 资源类型

命名空间：microsoft.graph

包含签名证书的公共部分。 

此资源类型是 [addSelfSignedSigningCertificate 操作返回](../api/serviceprincipal-addtokensigningcertificate.md) 的类型。 服务提供商使用签名证书的公共部分来验证令牌的颁发者。

## <a name="properties"></a>属性
属性|类型|说明
----|--|---
|customKeyIdentifier|Binary| 自定义密钥标识符。 |
| displayName | String | 密钥的友好名称。 |
|endDateTime|DateTimeOffset|凭据过期的日期和时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|keyId|GUID|唯一标识符 (GUID) 的 GUID 值。|
|startDateTime|DateTimeOffset|凭据生效的日期和时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
|type|字符串|密钥凭据的类型。 "AsymmetricX509Cert"。|
|usage|String|一个描述密钥的用途的字符串。 可能的值是 `Verify`。|
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
  "@odata.type": "#microsoft.graph.selfSignedCertificate",
  "customKeyIdentifier": "String (Binary)",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "key": "String (Binary)",
  "keyId": "GUID",
  "startDateTime": "String (timestamp)",
  "thumbprint": "String",
  "type": "String",
  "usage": "String"
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

