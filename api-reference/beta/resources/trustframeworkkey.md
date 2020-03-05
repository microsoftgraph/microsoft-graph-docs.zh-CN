---
title: trustFrameworkKey 资源类型
description: 表示 JWK （JSON Web 密钥）。 TrustFrameworkKey 是一个 JSON 数据结构，它表示加密密钥。 此资源的结构遵循 RFC 7517 第4节中定义的格式。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a9b94075b7a81fdb596038afac21fbf6cbc68f42
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519650"
---
# <a name="trustframeworkkey-resource-type"></a>trustFrameworkKey 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 JWK （JSON Web 密钥）。 TrustFrameworkKey 是一个 JSON 数据结构，它表示加密密钥。 此资源的结构遵循[RFC 7517 第4节](https://tools.ietf.org/html/rfc7517#section-4)中定义的格式。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| 式 | string | 键的唯一标识符。   |
| kty | string | "Kty" （key type）参数标识密钥使用的加密算法系列，有效值为 "rsa，oct"。 |
| 改用 | string | "使用" （公钥使用）参数标识公钥的用途。  使用 "use" 参数来指示是否使用公钥对数据进行加密或验证数据签名。 可能的值为1。 "sig" （签名）2。  "enc" （加密）   |
| x5c | string 集合 | "X5c" （X. x.509 证书链）参数包含一个或多个 PKIX 证书[RFC 5280](https://tools.ietf.org/html/rfc5280)的链。 |
| x5t | string | "X5t" （x.509 证书 SHA-1 指纹）参数是 base64url 编码的 SHA-1 指纹（a.k.a。 摘要）的 x.509 证书[RFC 5280](https://tools.ietf.org/html/rfc5280)的 DER 编码。 |
| e | string | RSA Key-公共指数 |
| d| string | RSA Key-专用指数。 字段无法读回。 |
| n | string | RSA Key-模数 |
| p | string | RSA 键-第一个质数。 字段无法读回。 |
| q | 字符串 | RSA 键-第二个质数。 字段无法读回。 |
| 分发 | string | RSA Key-第一个指数。 字段无法读回。 |
| dq | string | RSA 键-第二个指数。 字段无法读回。 |
| qi | string | RSA 键-系数。 字段无法读回。 |
| kb | string | Oct 密钥类型的对称密钥。 字段无法读回。   |
| nbf | int | 此值是在 RFC 7519 中定义的 NumericDate （一个 JSON 数值，表示从 1970-01-01T00：00： 00Z UTC 到指定 UTC 日期/时间之间的秒数，忽略闰秒。） |
| exp | int | 此值是在 RFC 7519 中定义的 NumericDate （一个 JSON 数值，表示从 1970-01-01T00：00： 00Z UTC 到指定 UTC 日期/时间之间的秒数，忽略闰秒。） |



## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKey",
  "baseType": null
}-->

```json
{
  "d": "String",
  "dp": "String",
  "dq": "String",
  "e": "String",
  "exp": 1024,
  "k": "String",
  "kid": "String",
  "kty": "String",
  "n": "String",
  "nbf": 1024,
  "p": "String",
  "q": "String",
  "qi": "String",
  "use": "String",
  "x5c": ["String"],
  "x5t": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKey resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
