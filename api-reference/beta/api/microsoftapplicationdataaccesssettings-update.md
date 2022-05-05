---
title: 更新 microsoftApplicationDataAccessSettings
description: 更新 microsoftApplicationDataAccessSettings 对象的属性。
author: ttomi
ms.localizationpriority: medium
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 411a1b8cad849979cb3c0d49500c45d1e452037e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212411"
---
# <a name="update-microsoftapplicationdataaccesssettings"></a>更新 microsoftApplicationDataAccessSettings

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [microsoftApplicationDataAccessSettings](../resources/microsoftapplicationdataaccesssettings.md) 对象中的设置，该对象指定从 Microsoft 应用程序访问Microsoft 365组织中的用户数据。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Organization.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}/settings/microsoftApplicationDataAccess
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
|isEnabledForAllMicrosoftApplications|Boolean|设置为`true`后，组织中的所有用户都可以在 Microsoft 应用中访问用户有权访问的任何Microsoft 365数据。 Microsoft 应用可以是Microsoft 365应用 (，例如，Excel、Outlook) 或非Microsoft 365应用 (例如 Edge) 。 默认值为 `true`。 <br> 可以通过在 **disabledForGroup** 属性中指定组，为Azure Active Directory (Azure AD) 安全组中的一部分用户禁用此访问权限。 <br> 设置为`false`后，用户只能在Microsoft 365应用中访问授权Microsoft 365数据。|
|disabledForGroup|String|Azure AD安全组的 ID，其成员只能使用Microsoft 365应用访问Microsoft 365数据，但不允许使用其他 Microsoft 应用（如 Edge）。 <br> 仅当 **isEnabledForAllMicrosoftApplications** 设置为 `true`.|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [microsoftApplicationDataAccessSettings](../resources/microsoftapplicationdataaccesssettings.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

以下示例请求演示管理员如何更新 **disabledForGroup** 隐私设置，以禁止特定Azure AD组中的用户使用不属于Microsoft 365的 Microsoft 应用程序访问Microsoft 365数据。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_microsoftapplicationdataaccesssettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/microsoftApplicationDataAccess
Content-Type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-microsoftapplicationdataaccesssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-microsoftapplicationdataaccesssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-microsoftapplicationdataaccesssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-microsoftapplicationdataaccesssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-microsoftapplicationdataaccesssettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-microsoftapplicationdataaccesssettings-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftApplicationDataAccessSettings",
  "name": "update_microsoftapplicationdataaccesssettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.microsoftApplicationDataAccessSettings",
  "isEnabledForAllMicrosoftApplications": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
