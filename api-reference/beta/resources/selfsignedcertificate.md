---
title: selfSignedCertificate 资源类型
description: 包含有关签名证书的公共部分的信息。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: luleonpla
ms.openlocfilehash: 09e6ed6adfdfe2803e287bb60496e1b0eeb96a6b
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723680"
---
# <a name="selfsignedcertificate-resource-type"></a>selfSignedCertificate 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含签名证书的公共部分。 它是操作 [addTokenSigningCertificate 的返回类型](../api/serviceprincipal-addtokensigningcertificate.md)。 服务提供商使用签名证书的公共部分来验证令牌的颁发者。

## <a name="properties"></a>属性

| 属性            | 类型           | 说明                                                                                                                                                                                                                           |
| ------------------- | -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| customKeyIdentifier | Binary         | 自定义密钥标识符。                                                                                                                                                                                                                |
| displayName         | String         | 密钥的友好名称。                                                                                                                                                                                                        |
| endDateTime         | DateTimeOffset | 凭据过期的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。       |
| keyId               | Guid           | 该密钥 (GUID) 的唯一标识符。                                                                                                                                                                                             |
| startDateTime       | DateTimeOffset | 凭据生效的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| type                | String         | 密钥凭据的类型。 "AsymmetricX509Cert"。                                                                                                                                                                                     |
| usage               | String         | 一个描述密钥的用途的字符串。 例如，"Verify"。                                                                                                                                             |
| key                 | 二进制         | 密钥凭据的值。 应为 Base64 编码值。                                                                                                                                                                  |
| thumbprint          | String         | 键的指纹值。                                                                                                                                                                                                     |

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
  "keyId": "Guid",
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
