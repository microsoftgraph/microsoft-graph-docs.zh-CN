---
title: certificateAuthority 资源类型
description: 表示证书颁发机构。
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 87d439a15f9668931f0488e065cde5beef87ab2e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042700"
---
# <a name="certificateauthority-resource-type"></a>certificateAuthority 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示证书颁发机构。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|证书|Binary|必需。 表示公共证书的 base64 编码字符串。|
|certificateRevocationListUrl|String|证书吊销列表的 URL。|
|deltaCertificateRevocationListUrl|String|该 URL 包含自上次创建完整证书 revocaton 列表以来的所有已吊销证书的列表。|
|isRootAuthority|Boolean|必需。 如果受信任的证书是根证书颁发机构，**则为 true** ; 如果受信任的证书是中间颁发机构，则为**false** 。|
|常用|String|证书的颁发者，根据 **证书** 值计算。 只读。 |
|issuerSki|String|证书的主题密钥标识符，由 **证书** 值计算得出。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateAuthority",
  "baseType": null
}-->

```json
{
  "certificate": "Binary",
  "certificateRevocationListUrl": "String",
  "deltaCertificateRevocationListUrl": "String",
  "isRootAuthority": true,
  "issuer": "String",
  "issuerSki": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateAuthority resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

