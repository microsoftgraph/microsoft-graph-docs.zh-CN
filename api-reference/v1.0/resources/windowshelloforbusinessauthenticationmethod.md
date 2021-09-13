---
title: windowsHelloForBusinessAuthenticationMethod 资源类型
description: 注册到Windows Hello的 Business 实例实例的表示形式。 Windows Hello For Business 是一种登录身份验证方法。
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 619733961a54f2b8489d3eacc40a6ca060921ab9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139462"
---
# <a name="windowshelloforbusinessauthenticationmethod-resource-type"></a>windowsHelloForBusinessAuthenticationMethod 资源类型

命名空间：microsoft.graph

注册到用户的 Windows Hello for Business 身份验证方法的表示形式。 Windows Hello For Business 是一种登录身份验证方法，Windows设备。

继承自 [authenticationMethod](../resources/authenticationmethod.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsHelloForBusinessAuthenticationMethods](../api/windowshelloforbusinessauthenticationmethod-list.md)|[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 集合|获取 [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象及其属性的列表。|
|[获取 windowsHelloForBusinessAuthenticationMethod](../api/windowshelloforbusinessauthenticationmethod-get.md)|[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)|读取 [windowsHelloForBusinessAuthenticationMethod 对象的属性和](../resources/windowshelloforbusinessauthenticationmethod.md) 关系。|
|[删除 windowsHelloForBusinessAuthenticationMethod](../api/windowshelloforbusinessauthenticationmethod-delete.md)|无|删除 [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|注册此 Windows Hello for Business 密钥的日期和时间。|
|displayName|String|注册适用于 Business Windows Hello的设备的名称|
|id|String|此身份验证方法的唯一标识符。 继承自 [authenticationMethod](../resources/authenticationmethod.md)|
|keyStrength|authenticationMethodKeyStrength|此密钥的关键强度Windows Hello企业密钥。 可取值为：`normal`、`weak`、`unknown`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|设备|[设备](../resources/device.md)|Business 密钥所在的Windows Hello注册设备。|

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
