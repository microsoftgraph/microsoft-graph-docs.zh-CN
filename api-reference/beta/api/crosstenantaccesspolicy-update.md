---
title: 更新 crossTenantAccessPolicy
description: 更新跨租户访问策略的属性。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
---

# <a name="update-crosstenantaccesspolicy"></a>更新 crossTenantAccessPolicy

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新跨租户 [访问策略的属性](../resources/crosstenantaccesspolicy.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.ReadWrite.CrossTenantAccess|
|委派（个人 Microsoft 帐户）|不适用|
|应用程序|Policy.ReadWrite.CrossTenantAccess|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/crossTenantAccessPolicy
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|跨显示名称访问策略的组。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) 对象大小当前限制为 25KB。 如果策略大小超过 `400 Bad Request` 25KB，此方法将返回错误代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "update_crosstenantaccesspolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/policies/crossTenantAccessPolicy
Content-Type: application/json

{
  "displayName": "CrossTenantAccessPolicy",
}
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
