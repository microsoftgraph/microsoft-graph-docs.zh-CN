---
title: 列出 microsoftApplicationDataAccessSettings
description: 获取 microsoftApplicationDataAccessSettings 对象中的设置，该对象指定从 Microsoft 应用程序访问Microsoft 365组织的用户数据。
author: ttomi
ms.localizationpriority: medium
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 01b0f53b99eaff9abf62b36c8247be44cf5c94e7
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589591"
---
# <a name="list-microsoftapplicationdataaccesssettings"></a>列出 microsoftApplicationDataAccessSettings

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [microsoftApplicationDataAccessSettings](../resources/microsoftapplicationdataaccesssettings.md) 对象中的设置，该对象指定从 Microsoft 应用程序访问以Microsoft 365组织的用户数据。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户） | Organization.Read.All、Organization.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|Application | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}/settings/microsoftApplicationDataAccess
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [microsoftApplicationDataAccessSettings](../resources/microsoftapplicationdataaccesssettings.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_microsoftapplicationdataaccesssettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/microsoftApplicationDataAccess
```

### <a name="response"></a>响应

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftApplicationDataAccessSettings",
  "name": "list_microsoftapplicationdataaccesssettings"
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

## <a name="see-also"></a>另请参阅

[自定义组织的项目](/graph/insights-customize-item-insights-privacy) 见解隐私。
