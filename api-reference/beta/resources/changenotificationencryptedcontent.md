---
title: changeNotificationEncryptedContent 资源类型
description: changeNotificationEncryptedContent 对象代表附加到更改通知的加密数据。
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: eab67f8a390b6522f963b004670e31e256078353
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334105"
---
# <a name="changenotificationencryptedcontent-resource-type"></a>changeNotificationEncryptedContent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示附加到更改通知的加密数据。

有关详细信息，请参阅 [设置包含资源数据更改通知 (预览) ](/graph/webhooks-with-resource-data.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| data | string | 经过 Base64 编码的加密数据，可生成以 JSON 形式重新提供的完整资源。 数据已使用加密套件`dataKey``AES/CBC/PKCS5PADDING`提供的 进行加密。 |
| dataSignature | string | 出于验证目的，使用 Base64 编码的 HMAC-SHA256 哈希数据。 |
| dataKey | string | 由 Microsoft Graph Base64 编码的对称密钥，用于加密数据值并生成数据签名。 此密钥使用订阅期间提供的证书公钥进行加密。 必须先使用证书私钥对其进行解密，然后才能使用证书私钥解密数据或验证签名。 此密钥已使用以下加密套件进行加密： `RSA/ECB/OAEPWithSHA1AndMGF1Padding`。 |
| encryptionCertificateId | string | 用于加密 的证书的 `dataKey`ID。 |
| encryptionCertificateThumbprint | string | 用于加密 的证书指纹的十六进制表示形式 `dataKey`。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotificationEncryptedContent"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.changeNotificationEncryptedContent",
  "data": "String",
  "dataSignature": "String",
  "dataKey": "String",
  "encryptionCertificateId": "String",
  "encryptionCertificateThumbprint": "String"
}
```

<!-- uuid: 564a955a-4837-424d-b7b8-3c6c33d5176d
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "changeNotificationEncryptedContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


