---
title: 删除 samlOrWsFedExternalDomainFederation
description: 删除 samlOrWsFedExternalDomainFederation 对象。
author: namkedia
localization_priority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 98365e11649c5e4bd90ad2893a53a9c65fa36fc1
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697035"
---
# <a name="delete-samlorwsfedexternaldomainfederation"></a>删除 samlOrWsFedExternalDomainFederation
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除 [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) 对象。

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
DELETE directory/federationConfigurations/{samlOrWsFedExternalDomainFederation ID}
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "delete_samlorwsfedexternaldomainfederation"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/directory/federationConfigurations/96db02e2-80c1-5555-bc3a-de92ffb8c5be
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
