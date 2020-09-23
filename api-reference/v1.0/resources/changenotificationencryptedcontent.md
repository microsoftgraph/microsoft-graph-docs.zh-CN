---
title: changeNotificationEncryptedContent 资源类型
description: 一个 changeNotificationEncryptedContent 对象，代表附加到更改通知的加密数据。
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f86dc032e3f9e14790358a03e8026f1932ae9431
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193630"
---
# <a name="changenotificationencryptedcontent-resource-type"></a>changeNotificationEncryptedContent 资源类型

命名空间：microsoft.graph

代表附加到更改通知的加密数据。

有关详细信息，请参阅 [设置包含资源数据 (preview) 的更改通知 ](/graph/webhooks-with-resource-data.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| data | string | 以 Base64 编码的加密数据，生成完整的资源 respresented 作为 JSON。 数据已使用密码套件的提供进行了加密 `dataKey` `AES/CBC/PKCS5PADDING` 。 |
| dataSignature | string | 用于验证目的的用于数据的 Base64 编码的 HMAC 哈希值。 |
| dataKey | string | 由 Microsoft Graph 生成的 Base64 编码的对称密钥，用于加密数据值并生成数据签名。 此密钥使用订阅过程中提供的证书公钥进行加密。 必须使用证书私钥对其进行解密，然后才能将其用于解密数据或验证签名。 已使用以下密码套件对此项进行了加密： `RSA/ECB/OAEPWithSHA1AndMGF1Padding` 。 |
| encryptionCertificateId | string | 用于加密的证书的 ID `dataKey` 。 |
| encryptionCertificateThumbprint | string | 用于加密的证书的指纹的十六进制表示形式 `dataKey` 。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotificationEncryptedContent"
}-->

```json
{
  "data": "{encrypted data that produces a full resource}",
  "dataSignature": "<HMAC-SHA256 hash>",
  "dataKey": "{encrypted symmetric key from Microsoft Graph}",
  "encryptionCertificateId": "MySelfSignedCert/DDC9651A-D7BC-4D74-86BC-A8923584B0AB",
  "encryptionCertificateThumbprint": "07293748CC064953A3052FB978C735FB89E61C3D"
}
```

<!-- uuid: 6bb14c3d-16ef-4ea3-8dc7-c88b9190081c
2020-08-05 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "changeNotificationEncryptedConent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
