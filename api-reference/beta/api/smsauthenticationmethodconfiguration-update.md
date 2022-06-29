---
title: 更新 smsAuthenticationMethodConfiguration
description: 更新 smsAuthenticationMethodConfiguration 对象的属性。
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 65c3f49f7a83eb60ff0bf2f16ce781c758742be7
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445362"
---
# <a name="update-smsauthenticationmethodconfiguration"></a>更新 smsAuthenticationMethodConfiguration
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) 对象的属性，该对象表示 Azure AD 租户的文本消息身份验证方法策略。

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
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，使用应更新的字段值提供 [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) 对象的 JSON 表示形式。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

下表显示了更新 [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) 对象时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法策略标识符。|
|state|authenticationMethodState|可取值为：`enabled`、`disabled`。|

>**注意：**`@odata.type`具有值的`#microsoft.graph.smsAuthenticationMethodConfiguration`属性必须包含在正文中。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新 [的 smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_smsauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
    "id": "Sms",
    "state": "enabled"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-smsauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-smsauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-smsauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-smsauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-smsauthenticationmethodconfiguration-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-smsauthenticationmethodconfiguration-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.smsAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
  "id": "713980c7-80c7-7139-c780-3971c7803971",
  "state": "String"
}
```

