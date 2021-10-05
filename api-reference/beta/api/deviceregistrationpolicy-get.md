---
title: 获取 deviceRegistrationPolicy
description: 读取 deviceRegistrationPolicy 对象的属性和关系。
author: spunukol
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b02e1c9d6a0de046771e4a437cb1762eea73c6db
ms.sourcegitcommit: 2f394a9f33f2fab3634d0f18882985ee211067d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2021
ms.locfileid: "60127900"
---
# <a name="get-deviceregistrationpolicy"></a>获取 deviceRegistrationPolicy

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md) 对象的属性和关系。 表示 deviceRegistrationPolicy 配额限制、其他身份验证和授权策略，以向组织注册设备标识。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）| Policy.ReadWrite.DeviceConfiguration|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|不支持|

代表用户进行呼叫时，用户需要属于以下 [Azure AD 角色](/azure/active-directory/roles/permissions-reference)：
+ 全局管理员
+ 云设备管理员
+ 全局读取者

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
```http
GET /policies/deviceRegistrationPolicy
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_deviceregistrationpolicy"
}
-->
``` http
GET https://graph.microsoft.com/policies/deviceRegistrationPolicy
```


### <a name="response"></a>响应

下面是显示设备注册策略默认设置的响应示例。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceRegistrationPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#deviceRegistrationPolicy",
    "id": "deviceRegistrationPolicy",
    "displayName": "Device Registration Policy",
    "description": "Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks",
    "userDeviceQuota": 50,
    "multiFactorAuthConfiguration": "0",
    "azureADRegistration": {
        "appliesTo": "1",
        "isAdminConfigurable": false,
        "allowedUsers": [],
        "allowedGroups": []
    },
    "azureADJoin": {
        "appliesTo": "1",
        "isAdminConfigurable": true,
        "allowedUsers": [],
        "allowedGroups": []
    }
}
```
