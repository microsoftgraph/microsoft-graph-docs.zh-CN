---
title: fido2AuthenticationMethod 资源类型
description: 注册到用户的 FIDO2 安全密钥的表示形式。 FIDO2 是一种登录身份验证方法。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a6cfed32f6e657608b70c799d348c6818e56a8c7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440323"
---
# <a name="fido2authenticationmethod-resource-type"></a>fido2AuthenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

注册到用户的 FIDO2 安全密钥的表示形式。 FIDO2 是一种登录身份验证方法。


## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[List](../api/fido2authenticationmethod-list.md)|[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) 集合|检索用户的 fido2AuthenticationMethod 对象及其属性的列表。|
|[获取](../api/fido2authenticationmethod-get.md)|[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|读取用户 fido2AuthenticationMethod 对象的属性和关系。|
|[删除](../api/fido2authenticationmethod-delete.md)|无|删除用户的 fido2AuthenticationMethod 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法标识符。|
|displayName|String|用户显示名称的键的键值。|
|creationDateTime|DateTimeOffset|向用户注册此密钥的时间戳。|
|aaGuid|String|验证器证明 GUID，一个指示验证 (类型的标识符，例如验证) 和型号。|
|model|String|FIDO2 安全密钥的制造商分配模型。|
|attestationCertificates|字符串集合|证明证书 () 安全密钥的证书。|
|attestationLevel|attestationLevel|此 FIDO2 安全密钥的证明级别。 可能的值是： `attested` 或 `notAttested` 。|


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

