---
title: fido2AuthenticationMethod 资源类型
description: 向用户注册的 FIDO2 安全密钥的表示形式。 FIDO2 是一种登录身份验证方法。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c4d10252201781d1339e6baa26aea248429ae462
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418236"
---
# <a name="fido2authenticationmethod-resource-type"></a>fido2AuthenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

向用户注册的 FIDO2 安全密钥的表示形式。 FIDO2 是一种登录身份验证方法。


## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List](../api/fido2authenticationmethod-list.md)|[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) 集合|检索用户的 fido2AuthenticationMethod 对象及其属性的列表。|
|[获取](../api/fido2authenticationmethod-get.md)|[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|读取用户的 fido2AuthenticationMethod 对象的属性和关系。|
|[删除](../api/fido2authenticationmethod-delete.md)|无|删除用户的 fido2AuthenticationMethod 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|身份验证方法标识符。|
|displayName|字符串|用户给定的密钥的显示名称。|
|creationDateTime|DateTimeOffset|此注册表项注册到用户时的时间戳。|
|aaGuid|字符串|身份验证器证明 GUID，该标识符指示 (的类型，例如，) 身份验证程序的模型。|
|model|String|制造商分配的 FIDO2 安全密钥的模型。|
|attestationCertificates|字符串集合|证明证书 (s) 附加到此安全密钥。|
|attestationLevel|attestationLevel|此 FIDO2 安全密钥的证明级别。 可能的值为： `attested` 或 `notAttested` 。|


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fido2AuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2AuthenticationMethod",
  "id": "String (identifier)",
  "displayName": "String",
  "creationDateTime": "String (timestamp)",
  "aaGuid": "String",
  "model": "String",
  "attestationCertificates": [
    "String"
  ],
  "attestationLevel": "String"
}
```

