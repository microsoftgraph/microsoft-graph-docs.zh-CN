---
title: certificateAuthority 资源类型
description: 表示证书颁发机构。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 030e0fbe8fcae0408f51c20882d49e50d825cdb8
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539293"
---
# <a name="certificateauthority-resource-type"></a>certificateAuthority 资源类型

表示证书颁发机构。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|证书|Binary|必需。 表示公共证书的 base64 编码字符串。|
|certificateRevocationListUrl|字符串|证书吊销列表的 URL。|
|deltaCertificateRevocationListUrl|字符串|该 URL 包含自上次创建完整证书 revocaton 列表以来的所有已吊销证书的列表。|
|isRootAuthority|Boolean|必需。 如果受信任的证书是根证书颁发机构，**则为 true** ; 如果受信任的证书是中间颁发机构，则为**false** 。|
|常用|字符串|证书的颁发者，根据**证书**值计算。 只读。 |
|issuerSki|字符串|证书的主题密钥标识符，由**证书**值计算得出。 只读。|

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