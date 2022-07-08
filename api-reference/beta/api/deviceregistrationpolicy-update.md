---
title: 更新 deviceRegistrationPolicy
description: 更新 deviceRegistrationPolicy 对象的属性。
author: myra-ramdenbourg
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: df37115ff775d204a68c2d95f59d644de5d62d6a
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2022
ms.locfileid: "66689993"
---
# <a name="update-deviceregistrationpolicy"></a>更新 deviceRegistrationPolicy

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [deviceRegistrationPolicy 对象的](../resources/deviceregistrationpolicy.md) 属性。 表示 deviceRegistrationPolicy 配额限制、其他身份验证和授权策略，用于向组织注册设备标识。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.ReadWrite.DeviceConfiguration|
|委派（个人 Microsoft 帐户）|不支持|
|Application|不支持|

代表用户调用时，用户需要属于以下 [Azure AD 角色](/azure/active-directory/roles/permissions-reference)：
+ 全局管理员
+ 云设备管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
```http
PUT /policies/deviceRegistrationPolicy
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，*仅* 提供应更新的属性的值。未包含在请求正文中的现有属性将保留其以前的值或根据对其他属性值的更改重新计算。

下表指定可更新的属性。


|属性|类型|说明|
|:---|:---|:---|
|userDeviceQuota|Int32|指定在阻止新设备注册之前，用户可在组织中拥有的最大设备数。 |
|multiFactorAuthConfiguration|multiFactorAuthConfiguration|指定用户使用组织内注册的 Azure AD Join 或 Azure AD 完成注册的身份验证策略。 可能的值是：`notRequired` 或 `required`。 |
|azureADRegistration|[azureADRegistrationPolicy](../resources/azureadregistrationpolicy.md)|指定用于在组织内使用 Azure AD 注册控制新设备注册的授权策略。 必填。 有关详细信息，请参阅[什么是设备标识？](/azure/active-directory/devices/overview) 如果启用Intune，则无法修改此属性。|
|azureADJoin|[azureAdJoinPolicy](../resources/azureadjoinpolicy.md)|指定用于在组织内使用 Azure AD Join 控制新设备注册的授权策略。 必填。 有关详细信息，请参阅[什么是设备标识？](/azure/active-directory/devices/overview)|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_deviceregistrationpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/beta/deviceRegistrationPolicy
Content-Type: application/json

{
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-deviceregistrationpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-deviceregistrationpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-deviceregistrationpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-deviceregistrationpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

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
