---
title: Microsoft Graph 身份验证方法 API 入门
description: Microsoft Graph 中的身份验证方法 API 使组织能够以编程方式管理其用户身份验证方法，从而使已注册用户能够执行多重身份验证 (MFA) 和自助服务密码重置 (SSPR)。
author: mmcla
localization_priority: Priority
ms.prod: identity-and-sign-in
ms.openlocfilehash: 36385345141daa8dc782b64fa154ef97c46b3091
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761449"
---
# <a name="get-started-with-the-microsoft-graph-authentication-methods-api"></a>Microsoft Graph 身份验证方法 API 入门

[身份验证方法](/azure/active-directory/authentication/concept-authentication-methods) 是用户在 Azure Active Directory (Azure AD) 中的身份验证方式。 Azure AD 中的身份验证方法包括密码和手机（例如，短信和语音呼叫），目前可在 Microsoft Graph 中对这些方法进行管理，此外还有 FIDO2 安全密钥和 Microsoft Authenticator 应用。 身份验证方法用于主要、双重因素和分步身份验证，此外还适用于自助式密码重置 (SSPR) 流程。

可使用身份验证方法 API 来管理用户的身份验证方法。 例如，你能够：

* 为用户添加一个电话号码，通过策略启用短信和语音呼叫身份验证后，该用户即可使用该号码进行此类身份验证
* 更新或删除分配给用户的电话号码
* 启用或禁用用于短信登录的号码
* 重置用户密码

API 是用于管理用户身份验证方法的一种关键工具。

在本教程中，你将学习如何：

> [!div class="checklist"]
> * 使用正确的角色和权限对 Azure AD 进行身份验证
> * 检查用户的身份验证方法
> * 为用户添加新的电话号码
> * 删除用户的电话号码
> * 重置用户密码

## <a name="step-1-authenticate-to-azure-ad-with-the-right-roles-and-permissions"></a>步骤 1：使用正确的角色和权限对 Azure AD 进行身份验证

使用你喜欢的[工具与 Microsoft Graph 交互](use-the-api.md#tools-for-interacting-with-microsoft-graph)，使用具有以下一种角色的帐户登录：

* 全局管理员
* 特权身份验证管理员
* 身份验证管理员

接下来，修改你的权限。 在本教程中，我们将使用 [UserAuthenticationMethod.ReadWrite.All](permissions-reference.md#user-authentication-method-permissions-preview)，因此，请确保已在 Graph 浏览器或你的应用中启用此权限。

分配范围并获得同意后，即可开始使用 API。 此处的示例使用名为 Avery Howard 的标准用户。 您应该使用现有的测试帐户，或按照[这些说明](/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user)创建一个新的测试帐户。 这些 API 是实时的，因此请不要在实际用户上对其进行测试。

## <a name="step-2-check-the-users-authentication-methods"></a>步骤 2：检查用户的身份验证方法

拨打电话，以查看用户的身份验证方法。 获取 URL 以查看用户的个人资料并添加 `/authentication/methods`：

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

## <a name="step-3-add-new-phone-numbers-for-the-user"></a>步骤 3：为用户添加新的电话号码

在上一步中，新用户 (Avery) 仅注册了密码。 若要分配新的电话号码供 Avery 使用，请在正文中使用电话类型和号码发出 `POST` 请求。 若要告知系统正在添加电话号码，还需要将 URL 的末尾从 `methods` 更改为 `phoneMethods`。

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

要添加 Avery 的办公室号码，你将再次`POST`访问相同的 URL，但要更新电话类型和电话号码：

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

对电话方法 URL 再执行一次 `GET`，以查看 Avery 的所有电话号码：

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

确认你可以按预期看到这两个号码。

## <a name="step-4-remove-a-phone-number-from-the-user"></a>步骤 4：删除用户的电话号码

在本场景中，Avery 现在在家工作，你需要从他们的帐户中删除他们的办公室号码。 需要在办公室电话 URL 上呼叫 `DELETE`，可以通过将办公室电话的 ID 附加到电话方法 URL 来创建办公室电话 URL。 查看上面的 Avery 电话列表：办公室电话 ID 以“e37f”开头。

### <a name="request"></a>请求

```http
DELETE https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods/e37fc753-ff3b-4958-9484-eaa9425c82bc
```

响应中没有数据，因为没有更多符合预期的办公室电话。 可通过查看 Avery 的所有方法来确认它已删除，与之前的发出的 `GET` 相同：

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

正如预期的那样，用户现在又回到只有一部手机和一个密码的状态。

## <a name="step-5-reset-the-users-password"></a>步骤 5：重置用户密码

在此场景中，Avery 忘记了密码，你需要为他们重置。 若要重置密码，你需要向其密码的 URL 发出 `POST`（请查看 Avery 身份验证方法列表中以“28c1”开头的 ID），并指定“resetPassword”操作。 在请求正文中提供新密码。

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

``` http
Location: https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

由于这是将密码向下同步到租户的本地基础结构中的 Active Directory，可能需要几分钟，因此你有一个可以查看其是否完整的地址。 此地址位于响应的位置标头中，可查看该 URL 上的 `GET` 状态。

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

成功！ 你已经演练了查看用户个人资料、查看用户的身份验证方法、添加和删除电话号码以及重置用户密码。 现在可以开始管理自己用户的方法了。

## <a name="api-reference"></a>API 参考

在查找身份验证方法的 API 参考？

* 请参阅 [Azure AD 身份验证方法 API 概述](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)

## <a name="next-steps"></a>后续步骤

* 了解如何[使用身份验证方法 REST API](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)。
* 使用 Azure AD 对 Microsoft Graph [进行身份验证](./auth/index.yml)。
* 将 [Azure AD 登录](https://azure.microsoft.com/develop/identity/signin/)集成到应用或网站中。
* 有关 Azure AD API 中新增功能的信息，请参阅[更改日志](changelog.md)。
* 浏览[示例](https://developer.microsoft.com/graph/graph/examples)，了解有关如何使用 Microsoft Graph 的更多信息。