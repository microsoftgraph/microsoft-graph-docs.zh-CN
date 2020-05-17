---
title: Microsoft Graph 身份验证方法 API 入门
description: Microsoft Graph 中的身份验证方法 API 使组织能够以编程方式管理其用户的身份验证方法，从而获得注册了多重身份验证（MFA）和自助服务密码重置（SSPR）的用户。
author: mmcla
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8f08ae59f7a2ad0e16c4fc0c3af5637bcbfaaca
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272807"
---
# <a name="get-started-with-the-microsoft-graph-authentication-methods-api"></a>Microsoft Graph 身份验证方法 API 入门

[身份验证方法](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods)是用户在 Azure Active Directory （azure AD）中进行身份验证的方法。 Azure AD 中的身份验证方法包括密码和电话（例如，SMS 和语音呼叫），这些方法可在 Microsoft Graph 中进行管理，如 FIDO2 安全密钥和 Microsoft 身份验证器应用等许多其他内容。 身份验证方法在主要、第二因素和分步身份验证以及自助密码重置（SSPR）过程中也使用。

您可以使用身份验证方法 Api 来管理用户的身份验证方法。 例如，你能够：

* 为用户添加电话号码，如果启用这些号码，则该号码可在策略中使用该号码进行短信和语音呼叫身份验证
* 更新或删除分配给用户的电话号码
* 启用或禁用 SMS 登录号码
* 重置用户密码

Api 是管理用户的身份验证方法的主要工具。

在本教程中，你将了解如何执行以下操作：

> [!div class="checklist"]
> * 使用正确的角色和权限向 Azure AD 进行身份验证
> * 检查用户的身份验证方法
> * 为用户添加新电话号码
> * 从用户中删除电话号码
> * 重置用户的密码

## <a name="step-1-authenticate-to-azure-ad-with-the-right-roles-and-permissions"></a>步骤1：使用正确的角色和权限向 Azure AD 进行身份验证

使用您喜爱的[工具与 Microsoft Graph 交互](use-the-api.md#tools-for-interacting-with-microsoft-graph)，使用具有以下角色之一的帐户登录：

* 全局管理员
* 特权身份验证管理员
* 身份验证管理员

接下来，修改您的权限。 我们将使用[UserAuthenticationMethod](permissions-reference.md#user-authentication-method-permissions-preview) ，以确保在 Graph 资源管理器或你的应用程序中启用了此教程。

在分配并许可范围后，即可开始使用 API。 此处的示例使用名为 "Avery Howard" 的标准用户。 应使用预先存在的测试帐户，或按照[这些说明](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user)创建一个新的测试帐户。 这些 Api 是实时的，因此不会对真实用户进行测试。

## <a name="step-2-check-the-users-authentication-methods"></a>步骤2：检查用户的身份验证方法

打电话以查看用户的身份验证方法。 获取 URL 以查看用户的配置文件并添加 `/authentication/methods` ：

### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a>响应

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/methods",
    "value": [
        {
            "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
            "id": "28c10230-6103-485e-b985-444c60001490",
            "password": null,
            "creationDateTime": null
        }
    ]
}
```

## <a name="step-3-add-new-phone-numbers-for-the-user"></a>步骤3：为用户添加新电话号码

在上一步中，新用户（Avery）仅注册了密码。 若要将新电话号码分配给 Avery 以供使用，请 `POST` 在正文中使用电话类型和号码发出请求。 若要告知系统正在添加的电话号码，您还需要将 URL 的结束值从更改 `methods` 为 `phoneMethods` 。

### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
Content-Type: application/json
```

```json
{
    "phoneType": "mobile",
    "phoneNumber": "+1 2065550123"
}
```

### <a name="response"></a>响应

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "3179e48a-750b-4051-897c-87b9720928f7",
    "phoneNumber": "+1 2065550123",
    "phoneType": "mobile",
    "smsSignInState": "ready"
}
```

若要添加 Avery 的办公室号码，您将 `POST` 再次指向相同的 URL，但会更新电话类型和号码：

### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
Content-Type: application/json
```

```json
{
    "phoneType": "office",
    "phoneNumber": "+1 4255550199"
}
```

### <a name="response"></a>响应

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc",
    "phoneNumber": "+1 4255550199",
    "phoneType": "office",
    "smsSignInState": "notSupported"
}
```

对电话方法 URL 执行更多操作 `GET` ，以查看所有 Avery 的电话号码：

### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
```

### <a name="response"></a>响应

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods",
    "value": [
        {
            "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc",
            "phoneNumber": "+1 4255550199",
            "phoneType": "office",
            "smsSignInState": "notSupported"
        },
        {
            "id": "3179e48a-750b-4051-897c-87b9720928f7",
            "phoneNumber": "+1 2065550123",
            "phoneType": "mobile",
            "smsSignInState": "ready"
        }
    ]
}
```

确认您可以按预期看到两个数字。

## <a name="step-4-remove-a-phone-number-from-the-user"></a>步骤4：从用户中删除电话号码

在这种情况下，Avery 现在在家工作，您需要从其帐户中删除其办公室号码。 您需要通过将 `DELETE` office PHONE ID 追加到电话方法 url 来创建 office 电话 url。 查看上 Avery 的手机列表： office 电话 ID 以 "e37f" 开头。

### <a name="request"></a>请求

```http
DELETE https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods/e37fc753-ff3b-4958-9484-eaa9425c82bc
```

由于没有其他需要的办公室电话，响应中没有数据。 您可以通过查看所有 Avery 的方法来确认它是否已消失，这与 `GET` 之前所做的完全相同：

### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a>响应

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/methods",
    "value": [
        {
            "@odata.type": "#microsoft.graph.phoneAuthenticationMethod",
            "id": "3179e48a-750b-4051-897c-87b9720928f7",
            "phoneNumber": "+1 2065550123",
            "phoneType": "mobile",
            "smsSignInState": "ready"
        },
        {
            "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
            "id": "28c10230-6103-485e-b985-444c60001490",
            "password": null,
            "creationDateTime": null
        }
    ]
}
```

正如预期一样，用户现在可以返回到仅拥有一个移动电话和一个密码。

## <a name="step-5-reset-the-users-password"></a>步骤5：重置用户的密码

在这种情况下，Avery 忘记了密码，你需要为其重置。 若要重置，您将 `POST` 为其密码的 URL （请参阅在 Avery 的身份验证方法列表中以 "28c1" 开头的 ID），并指定 "resetPassword" 操作。 在请求正文中提供新密码。

### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword
Content-Type: application/json
```

```json
{
    "newPassword": "29sdjfw#fajsdA_a_3an3223"
}
```

### <a name="response"></a>响应

```
Location: https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

由于这会将密码同步到租户的本地基础结构中的 Active Directory，因此可能需要几分钟时间，因此您有一个地址，您可以在其中查看它是否已完成。 此地址位于响应的位置标头中，可查看该 URL 上的状态 do `GET` 。

### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

### <a name="response"></a>响应

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('ed178e23-7447-4892-baf8-fc46f8af26ce')/authentication/operations/$entity",
    "id": "74bfa1a6-c0e0-4957-8c37-f91048f4959e",
    "createdDateTime": "2020-05-14T00:23:40Z",
    "lastActionDateTime": "2020-05-14T00:23:41Z",
    "status": "succeeded",
    "statusDetail": "ResetSuccess",
    "resourceLocation": "https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/methods/28c10230-6103-485e-b985-444c60001490"
}
```

和成功！ 您已完成查看用户的配置文件、其身份验证方法、添加和删除电话号码以及重置其密码。 现在，你可以开始管理自己的用户的方法。

## <a name="api-reference"></a>API 参考

查找身份验证方法的 API 参考？

* 请参阅[AZURE AD 身份验证方法 API 概述](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)

## <a name="next-steps"></a>后续步骤

* 了解如何[使用身份验证方法 REST api](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)。
* 使用 Azure AD 对 Microsoft Graph [进行身份验证](/graph/auth)。
* 将 [Azure AD 登录](https://azure.microsoft.com/develop/identity/signin/)集成到应用或网站中。
* 有关 Azure AD API 中新增功能的信息，请参阅[更改日志](changelog.md)。
* 浏览[示例](https://developer.microsoft.com/graph/graph/examples)，了解有关如何使用 Microsoft Graph 的更多信息。
