---
title: 创建 externalDomainName
description: 创建新的 externalDomainName 对象。
author: namkedia
localization_priority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1eb7e580fb5e2c469eaece2889a236b4cde02b6d
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697009"
---
# <a name="create-externaldomainname"></a>创建 externalDomainName
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过创建新的 [externalDomainName](../resources/externaldomainname.md) 对象，WS-Fed个或多个域添加到基于 SAML 或基于 SAML 的配置，并将其添加到现有 [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)中。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|Domain.ReadWrite.All|
|委派（个人 Microsoft 帐户）| 不支持。|
|应用程序|Domain.ReadWrite.All|

工作或学校帐户需要属于 Azure AD 角色Azure Active Directory ([之) 之一](/azure/active-directory/roles/permissions-reference)：

* 全局管理员
* 外部标识提供程序管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /directory/federationConfigurations/{samlOrWsFedExternalDomainFederation ID}/microsoft.graph.samlOrWsFedExternalDomainFederation/domains
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [externalDomainName](../resources/externaldomainname.md) 对象的 JSON 表示形式。

下表显示创建 [externalDomainName 时所需的属性](../resources/externaldomainname.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|要添加到 [samlOrWsFedExternalDomainFederation 的外部组织的域名](../resources/samlorwsfedexternaldomainfederation.md)。 继承自 [实体](../resources/entity.md)。|

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [externalDomainName](../resources/externaldomainname.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_externaldomainname_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/directory/federationConfigurations/d5a56845-6845-d5a5-4568-a5d54568a5d5/microsoft.graph.samlOrWsFedExternalDomainFederation/domains
Content-Type: application/json
Content-length: 60

{
    "@odata.type": "microsoft.graph.externalDomainName",
    "id": "contososuites.com"
}
```

### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalDomainName"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalDomainName",
  "id": "contososuites.com"
}
```
