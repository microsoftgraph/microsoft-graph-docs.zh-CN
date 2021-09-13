---
title: certificateAuthority 资源类型
description: 表示证书颁发机构。
ms.localizationpriority: medium
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 067eeea8a341525f77427f518b02a07de38a05a1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067484"
---
# <a name="certificateauthority-resource-type"></a>certificateAuthority 资源类型

命名空间：microsoft.graph

表示证书颁发机构。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|证书|Binary|必填。 base64 编码的字符串，表示公共证书。|
|certificateRevocationListUrl|String|证书吊销列表的 URL。|
|deltaCertificateRevocationListUrl|String|URL 包含自上次创建完整证书撤销列表以来所有吊销的证书的列表。|
|isRootAuthority|Boolean|必填。 如果受信任证书是根证书颁发机构，则其为 **true;** 如果受信任证书是中间证书颁发机构，则其为 false。|
|issuer|String|证书的颁发者，根据证书 **值** 计算。 只读。 |
|issuerSki|String|证书的主题密钥标识符，根据 **证书值计算** 。 只读。|

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
