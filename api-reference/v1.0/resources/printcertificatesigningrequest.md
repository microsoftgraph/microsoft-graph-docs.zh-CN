---
title: printCertificateSigningRequest 资源类型
description: 证书签名请求 (CSR) 在向通用打印服务注册打印机期间使用。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 2136ae68a722242e8ad3b7f39743e20d7a54cfe7
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944296"
---
# <a name="printcertificatesigningrequest-resource-type"></a>printCertificateSigningRequest 资源类型

命名空间：microsoft.graph

证书签名请求 (CSR) 在向通用打印服务注册打印机期间使用。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|内容|String|base64 编码的 pkcs10 证书请求。 只读。|
|transportKey|String|由客户端生成的非对称密钥的 base64 编码的公共部分。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printCertificateSigningRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printCertificateSigningRequest",
  "content": "String",
  "transportKey": "String"
}
```

