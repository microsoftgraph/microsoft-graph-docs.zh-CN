---
title: printCertificateSigningRequest 资源类型
description: 证书签名请求 (CSR) 在使用通用打印服务的打印机注册过程中使用。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 786c5224826040e685f27a131cb81f07e1eebd7f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084008"
---
# <a name="printcertificatesigningrequest-resource-type"></a>printCertificateSigningRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

证书签名请求 (CSR) 在使用通用打印服务的打印机注册过程中使用。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|内容|String|Base64 编码的 pkcs10 证书请求。 只读。|
|transportKey|字符串|由客户端生成的非对称密钥的 base64 编码的公共部分。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printCertificateSigningRequest"
}-->

```json
{
  "content": "String",
  "transportKey": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printCertificateSigningRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


