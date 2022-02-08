---
title: 获取 crossTenantAccessPolicyConfigurationDefault
description: 读取跨租户访问策略的默认配置。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
---

# <a name="get-crosstenantaccesspolicyconfigurationdefault"></a>获取 crossTenantAccessPolicyConfigurationDefault

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [跨租户](../resources/crosstenantaccesspolicyconfigurationdefault.md) 访问策略的默认配置。 此默认配置可能是 **isServiceDefault** `true` Azure AD (分配的服务默认值) 或在租户中自定义 (**isServiceDefault**) `false` 。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.Read.All、Policy.ReadWrite.CrossTenantAccess|
|委派（个人 Microsoft 帐户）|不适用|
|应用程序|Policy.Read.All、Policy.ReadWrite.CrossTenantAccess|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/crossTenantAccessPolicy/default
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_crosstenantaccesspolicyconfigurationdefault"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/crossTenantAccessPolicy/default
```

### <a name="response"></a>响应

以下响应对象显示继承自 Azure AD 的默认跨租户策略，由 **isServiceDefault** `true`设置为 标识。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
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
  "isServiceDefault": true,
  "inboundTrust":
  {
    "isMfaAccepted": false,
    "isCompliantDeviceAccepted": false,
    "isHybridAzureADJoinedDeviceAccepted": false,
  },
  "b2bCollaborationOutbound":
  {
    "usersAndGroups":
    {
      "accessType": "allowed",
      "targets": [
        {
          "target": "AllUsers",
          "targetType": "user"
        }
      ]
    },
    "applications":
    {
      "accessType": "allowed",
      "targets": [
        {
          "target": "AllApplications",
          "targetType": "application"
        }
      ]
    }
  },
  "b2bCollaborationInbound":
  {
    "usersAndGroups":
    {
      "accessType": "allowed",
      "targets": [
        {
          "target": "AllUsers",
          "targetType": "user"
        }
      ]
    },
    "applications":
    {
      "accessType": "allowed",
      "targets": [
        {
          "target": "AllApplications",
          "targetType": "application"
        }
      ]
    }
  },
  "b2bDirectConnectOutbound":
  {
    "usersAndGroups":
    {
      "accessType": "blocked",
      "targets": [
        {
          "target": "AllUsers",
          "targetType": "user"
        }
      ]
    },
    "applications":
    {
      "accessType": "blocked",
      "targets": [
        {
          "target": "AllApplications",
          "targetType": "application"
        }
      ]
    }
  },
  "b2bDirectConnectInbound":
  {
    "usersAndGroups":
    {
      "accessType": "blocked",
      "targets": [
        {
          "target": "AllUsers",
          "targetType": "user"
        }
      ]
    },
    "applications":
    {
      "accessType": "blocked",
      "targets": [
        {
          "target": "AllApplications",
          "targetType": "application"
        }
      ]
    }
  }
}
```
