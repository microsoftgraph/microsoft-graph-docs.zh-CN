---
title: x509CertificateUserBinding 资源类型
description: 定义 X.509 证书中映射到 Azure AD 对象的属性的字段，以便将证书绑定到用户帐户。
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="x509certificateuserbinding-resource-type"></a>x509CertificateUserBinding 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义 X.509 证书中映射到 Azure AD 对象的属性的字段，以便将证书绑定到用户帐户。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|priority|Int32|绑定的优先级。 Azure AD使用优先级最高的绑定。 此值必须为非负整数，并且对于 **x509CertificateAuthenticationMethodConfiguration** 对象的 **certificateUserBindings** 属性中的对象集合是唯一的。 必需|
|userProperty|String|定义Azure AD绑定的用户对象的 user 属性。 可能的值是：**userPrincipalName**、、`onPremisesUserPrincipalName``email`。 必需。|
|x509CertificateField|String|X.509 证书上用于绑定的字段。 可能的值是：、`PrincipalName``RFC822Name`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.x509CertificateUserBinding"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.x509CertificateUserBinding",
  "x509CertificateField": "String",
  "userProperty": "String",
  "priority": "Integer"
}
```

