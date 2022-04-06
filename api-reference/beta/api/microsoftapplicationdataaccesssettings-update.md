---
title: 更新 microsoftApplicationDataAccessSettings
description: 更新 microsoftApplicationDataAccessSettings 对象的属性。
author: ttomi
ms.localizationpriority: medium
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: d7031fefb9f90718dc0e0fb66714cb933fa9dfe9
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589603"
---
# <a name="update-microsoftapplicationdataaccesssettings"></a>更新 microsoftApplicationDataAccessSettings

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [microsoftApplicationDataAccessSettings](../resources/microsoftapplicationdataaccesssettings.md) 对象中的设置，该对象指定从 Microsoft 应用程序访问以Microsoft 365组织的用户数据。

## <a name="permissions"></a>Permissions

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
|isEnabledForAllMicrosoftApplications|Boolean|`true`设置为 时，组织中所有用户都可以在 Microsoft 应用中访问Microsoft 365已授权访问的任何数据。 Microsoft 应用可以是一个Microsoft 365应用 (，例如 Excel、Outlook) 或非 Microsoft 365 应用 (例如 Edge) 。 默认值为 `true`。 <br> 通过指定 **disabledForGroup** 属性中的组，可以禁用 Azure Active Directory (Azure AD) 安全组中用户的此访问权限。 <br> 设置为 时`false`，用户只能在 Microsoft 365应用中访问授权Microsoft 365数据。|
|disabledForGroup|String|仅允许Azure AD安全组的成员仅Microsoft 365其他 Microsoft 应用（如 Edge）Microsoft 365访问数据的安全组的 ID。 <br> This is only applicable if **isEnabledForAllMicrosoftApplications is** set to `true`.|

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [microsoftApplicationDataAccessSettings](../resources/microsoftapplicationdataaccesssettings.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

以下示例请求显示管理员如何更新 **disabledForGroup** 隐私设置，以禁止特定 Azure AD 组的用户使用不是 Microsoft 365 一部分的 Microsoft 应用程序访问 Microsoft 365 数据。

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
