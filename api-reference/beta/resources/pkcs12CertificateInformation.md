---
title: pkcs12CertificateInformation 资源类型
description: 表示 Pkcs12 客户端证书的公共信息。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ada0d5d56d9fc785f6056862324aebd69d7358b3
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509372"
---
# <a name="pkcs12certificateinformation-resource-type"></a>pkcs12CertificateInformation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Pkcs12 证书的公共信息。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|isActive|布尔|  表示证书是否是用于调用 API 连接器的活动证书。 活动证书是最近上载的证书，该证书尚未过期，但其未过期时间已过去。|
|thumbprint|字符串| 证书指纹。 |
|notAfter|整数| 证书已过期。 此值是 RFC 7519 (中定义的 NumericDate 一个 JSON 数值，表示从 1970-01-01T00：00：00Z UTC 到指定的 UTC 日期/时间（忽略跃点秒）的秒数。) |
|notBefore|整数| 证书的颁发时间 (之前) 。 此值是 RFC 7519 (中定义的 NumericDate 一个 JSON 数值，表示从 1970-01-01T00：00：00Z UTC 到指定的 UTC 日期/时间（忽略跃点秒）的秒数。) |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pkcs12CertificateInformation"
}
-->

``` json
{
    "isActive": true,
    "thumbprint": "string",
    "notAfter": 0000000000,
    "notBefore": 0000000000,
}
```
