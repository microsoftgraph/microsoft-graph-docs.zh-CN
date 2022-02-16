---
title: x509CertificateAuthenticationMethodConfiguration 资源类型
description: 表示租户中 Azure AD 本机 Certificate-Based 身份验证 (CBA) 的详细信息，包括是启用还是禁用身份验证方法，以及可以注册和使用身份验证方法的用户和组。
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 415f17972c6163314cfdb54a5828e4db65dca04a
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854363"
---
# <a name="x509certificateauthenticationmethodconfiguration-resource-type"></a>x509CertificateAuthenticationMethodConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户中 Azure AD 本机 Certificate-Based 身份验证 (CBA) 的详细信息，包括是启用还是禁用身份验证方法，以及可以注册和使用身份验证方法的用户和组。

继承自 [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 x509CertificateAuthenticationMethodConfiguration](../api/x509certificateauthenticationmethodconfiguration-get.md)|[x509CertificateAuthenticationMethodConfiguration](../resources/x509certificateauthenticationmethodconfiguration.md)|读取 x509CertificateAuthenticationMethodConfiguration 对象的属性和关系。|
|[更新 x509CertificateAuthenticationMethodConfiguration](../api/x509certificateauthenticationmethodconfiguration-update.md)|[x509CertificateAuthenticationMethodConfiguration](../resources/x509certificateauthenticationmethodconfiguration.md)|更新 x509CertificateAuthenticationMethodConfiguration 对象的属性。|
|[删除 x509CertificateAuthenticationMethodConfiguration](../api/x509certificateauthenticationmethodconfiguration-delete.md)|无| 删除租户自定义的 x509CertificateAuthenticationMethodConfiguration 对象并还原默认配置。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法策略的标识符。 该值始终为 `X509Certificate`。 继承自 [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)。|
|state|authenticationMethodState|可能的值是：、`enabled``disabled`。 继承自 [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)。|
|certificateUserBindings|[x509CertificateUserBinding](../resources/x509certificateuserbinding.md) 集合|定义 X.509 证书中映射到用户Azure AD属性的字段，以便将证书绑定到用户。 **对象的** 优先级确定绑定执行的顺序。将使用第一个匹配绑定，其余绑定将被忽略。 |
|authenticationModeConfiguration|[x509CertificateAuthenticationModeConfiguration](../resources/x509certificateauthenticationmodeconfiguration.md)|定义强身份验证配置。 此配置包括默认身份验证模式和强身份验证绑定的不同规则。 |


## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|includeTargets|[authenticationMethodTarget](../resources/authenticationmethodtarget.md) 集合|允许使用身份验证方法的用户或组的集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.x509CertificateAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.x509CertificateAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "certificateUserBindings": [
    {
      "@odata.type": "microsoft.graph.x509CertificateUserBinding"
    }
  ],
  "authenticationModeConfiguration": {
    "@odata.type": "microsoft.graph.x509CertificateAuthenticationModeConfiguration"
  }
}
```

