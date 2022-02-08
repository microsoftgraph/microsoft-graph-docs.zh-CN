---
title: crossTenantAccessPolicyConfigurationDefault：resetToSystemDefault
description: 将跨租户访问策略中对默认配置所做的更改重置回系统默认值。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
---

# <a name="crosstenantaccesspolicyconfigurationdefault-resettosystemdefault"></a>crossTenantAccessPolicyConfigurationDefault：resetToSystemDefault

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将跨租户访问策略中对默认配置所做的更改重置回系统默认值。

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
POST /policies/crossTenantAccessPolicy/default/resetToSystemDefault
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此操作将返回 响应 `200 OK` 代码和空响应。 若要确认默认配置已还原为系统默认值，请运行 [Get crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-get.md) 并确认 **isSystemDefault** 已设置为 `true`。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "crosstenantaccesspolicyconfigurationdefault_resettosystemdefault"
}
-->

``` http
POST https://graph.microsoft.com/beta/policies/crossTenantAccessPolicy/default/resetToSystemDefault
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationDefault"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{

}
```
