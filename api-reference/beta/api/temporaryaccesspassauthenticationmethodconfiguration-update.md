---
title: 更新 temporaryAccessPassAuthenticationMethodConfiguration
description: 更新由 temporaryAccessPassAuthenticationMethodConfiguration 对象表示的 Azure AD 租户的临时访问传递策略。
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 23a250df8cb4b58e2654da867867eb96f4ef0641
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093036"
---
# <a name="update-temporaryaccesspassauthenticationmethodconfiguration"></a>更新 temporaryAccessPassAuthenticationMethodConfiguration
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新由 [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) 对象表示的 Azure AD 租户的临时访问传递策略。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.ReadWrite.AuthenticationMethod|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|Policy.ReadWrite.AuthenticationMethod|

对于委派方案，管理员需要以下 [Azure AD 角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：

* 身份验证策略管理员
* 全局管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，使用应更新的字段值提供 [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) 对象的 JSON 表示形式。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

可以更新对象的所有属性和关系。 有关属性和关系的列表，请参阅 [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)。

> [!NOTE]
> 具有值`#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration`**的 @odata.type** 属性必须包含在请求正文中。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_temporaryaccesspassauthenticationmethodconfiguration"
}
-->
```http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/temporaryAccessPass
Content-Type: application/json

{
  "@odata.type":"#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
  "isUsableOnce": true
}
```

### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```