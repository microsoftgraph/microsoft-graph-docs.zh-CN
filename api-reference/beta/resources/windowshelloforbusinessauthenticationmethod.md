---
title: windowsHelloForBusinessAuthenticationMethod 资源类型
description: 注册到用户的 Windows Hello 企业实例的表示形式。 Windows Hello 企业应用是一种登录身份验证方法。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3ac3f2cd3aed11943a1ab233cfbb64b7a75b32d0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433101"
---
# <a name="windowshelloforbusinessauthenticationmethod-resource-type"></a>windowsHelloForBusinessAuthenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

注册到用户的 Windows Hello 企业身份验证方法的表示形式。 Windows Hello 企业应用是 Windows 设备的登录身份验证方法。

继承自 [authenticationMethod](../resources/authenticationmethod.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsHelloForBusinessAuthenticationMethods](../api/windowshelloforbusinessauthenticationmethod-list.md)|[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 集合|获取 [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象及其属性的列表。|
|[获取 windowsHelloForBusinessAuthenticationMethod](../api/windowshelloforbusinessauthenticationmethod-get.md)|[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)|读取 [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象的属性和关系。|
|[删除 windowsHelloForBusinessAuthenticationMethod](../api/windowshelloforbusinessauthenticationmethod-delete.md)|无|删除 [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|注册此 Windows Hello 企业密钥的日期和时间。|
|displayName|String|注册 Windows Hello 企业应用的设备的名称|
|id|String|此身份验证方法的唯一标识符。 继承自 [authenticationMethod](../resources/authenticationmethod.md)|
|keyStrength|authenticationMethodKeyStrength|此 Windows Hello 企业密钥的关键强度。 可取值为：`normal`、`weak`、`unknown`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|设备|[设备](../resources/device.md)|此 Windows Hello 企业密钥所在的已注册设备。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
  "id": "String (Identifier)",
  "displayName": "String",
  "createdDateTime": "String",
  "keyStrength": {"@odata.type": "microsoft.graph.authenticationMethodKeyStrength"}
}
```
