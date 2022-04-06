---
title: 身份验证资源类型
description: 公开表示用户支持的身份验证Azure AD并可以配置用户的关系。
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4c098cc1b813a3805c1afc3956d93b6a416aa239
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510715"
---
# <a name="authentication-resource-type"></a>身份验证资源类型

命名空间：microsoft.graph

公开表示用户支持的身份验证Azure AD并可以配置用户的关系。

继承自 [entity](entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|fido2Methods|[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) 集合|表示注册到用户以进行身份验证的 FIDO2 安全密钥。|
|方法|[authenticationMethod](../resources/authenticationmethod.md) 集合| 表示注册到用户的所有身份验证方法。|
|microsoftAuthenticatorMethods|[microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 集合| 注册到Microsoft Authenticator的用户的应用程序的详细信息。 |
|windowsHelloForBusinessMethods|[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 集合|表示Windows Hello 企业版用户进行身份验证的身份验证方法。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authentication",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authentication"
}
```

