---
title: 身份验证资源类型
description: 公开表示 Azure AD 支持的身份验证方法且可为用户配置的关系。
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 34a7877f8b88e319cfb4ff0e710b064f56365eae
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971376"
---
# <a name="authentication-resource-type"></a>身份验证资源类型

命名空间：microsoft.graph

公开表示 Azure AD 支持的身份验证方法且可为用户配置的关系。

继承自 [entity](entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|fido2Methods|[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) 集合|表示注册给用户进行身份验证的 FIDO2 安全密钥。|
|方法|[authenticationMethod](../resources/authenticationmethod.md) 集合| 表示注册到用户的所有身份验证方法。|
|microsoftAuthenticatorMethods|[microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 集合| 注册给用户进行身份验证的 Microsoft Authenticator 应用的详细信息。 |
|temporaryAccessPassMethods|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 集合|表示通过时间限制的密码注册给用户进行身份验证的临时访问通行证。|
|windowsHelloForBusinessMethods|[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 集合|表示注册给用户进行身份验证的 Windows Hello 企业版身份验证方法。|

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
