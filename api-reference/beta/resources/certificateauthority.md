---
title: certificateAuthority 资源类型
description: 表示证书颁发机构。
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 64461015136129de452227cb0a8de5c7180cfb32
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135093"
---
# <a name="certificateauthority-resource-type"></a>certificateAuthority 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示证书颁发机构。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|证书|Binary|必填。 base64 编码字符串，表示公共证书。|
|certificateRevocationListUrl|字符串|证书吊销列表的 URL。|
|deltaCertificateRevocationListUrl|字符串|该 URL 包含自上次创建完整证书撤销列表以来所有吊销的证书的列表。|
|isRootAuthority|Boolean|必填。 如果受信任证书是根证书颁发机构，则其为 **true;** 如果受信任证书是中间证书颁发机构，则其为 false。|
|issuer|字符串|根据证书值计算得出的证书 **颁发** 者。 只读。 |
|issuerSki|字符串|证书的主题密钥标识符，根据证书值 **计算** 。 只读。|

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

