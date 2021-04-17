---
title: pkcs12CertificateInformation 资源类型
description: 表示 Pkcs12 客户端证书的公共信息。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4c649021d8fe66530edb794a859eecd8ed08def3
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882910"
---
# <a name="pkcs12certificateinformation-resource-type"></a>pkcs12CertificateInformation 资源类型

命名空间：microsoft.graph

表示 Pkcs12 证书的公共信息。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|isActive|Boolean|  表示证书是否是用于调用 API 连接器的活动证书。 活动证书是最近上载的证书，该证书尚未过期，但其未过期时间已过去。|
|thumbprint|String| 证书指纹。 |
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
    "isActive": "Boolean",
    "thumbprint": "String",
    "notAfter": "DateTime",
    "notBefore": "DateTime"
}
```
