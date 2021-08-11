---
title: printCertificateSigningRequest 资源类型
description: 证书签名请求 (CSR) 在通用打印服务注册打印机期间使用。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 0c86e7a2ecbd164f40dcbb0865954c4549622f16aa1f2b008a392f150b626aa8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129974"
---
# <a name="printcertificatesigningrequest-resource-type"></a>printCertificateSigningRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

证书签名请求 (CSR) 在通用打印服务注册打印机期间使用。

## <a name="properties"></a>属性
|属性|类型|说明|
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

