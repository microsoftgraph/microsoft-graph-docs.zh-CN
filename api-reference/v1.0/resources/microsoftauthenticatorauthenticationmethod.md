---
title: microsoftAuthenticatorAuthenticationMethod 资源类型
description: 注册到Microsoft Authenticator应用的表示形式。 Microsoft Authenticator身份验证方法。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 61f263b45b8e353622f06e6912f0659e2a8e147fabe208d8ea9ea2b94f555884
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54211939"
---
# <a name="microsoftauthenticatorauthenticationmethod-resource-type"></a>microsoftAuthenticatorAuthenticationMethod 资源类型

命名空间：microsoft.graph

注册到Microsoft Authenticator应用的表示形式。 Microsoft Authenticator身份验证方法。

继承自 [authenticationMethod](../resources/authenticationmethod.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 microsoftAuthenticatorAuthenticationMethods](../api/microsoftauthenticatorauthenticationmethod-list.md)|[microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 集合|获取 [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象及其属性的列表。|
|[获取 microsoftAuthenticatorAuthenticationMethod](../api/microsoftauthenticatorauthenticationmethod-get.md)|[microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)|读取 [microsoftAuthenticatorAuthenticationMethod 对象的属性和](../resources/microsoftauthenticatorauthenticationmethod.md) 关系。|
|[删除 microsoftAuthenticatorAuthenticationMethod](../api/microsoftauthenticatorauthenticationmethod-delete.md)|无|删除 [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|注册此应用程序的日期和时间。 如果设备未注册无密码登录，则电话为空。|
|displayName|String|注册此应用的设备的名称。|
|id|String|此身份验证方法的唯一标识符。 继承自 [authenticationMethod](../resources/authenticationmethod.md)|
|deviceTag|String|包含应用元数据的标记。|
|phoneAppVersion|String|此应用程序实例的数字Authenticator版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|设备|[设备](../resources/device.md)|注册设备所在的Microsoft Authenticator。 如果设备未注册无密码登录，则电话为空。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
  "id": "String (Identifier)",
  "displayName": "String",
  "deviceTag": "String",
  "phoneAppVersion": "String",
  "createdDateTime": "DateTimeOffset"
}
```
