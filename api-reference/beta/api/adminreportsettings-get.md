---
title: 获取 adminReportSettings
description: 获取 Microsoft 365 报表的租户级设置。
ms.localizationpriority: medium
author: qiwhuang
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: b9edf2396cd3409e794386f08eb4a124ce65d892
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856557"
---
# <a name="get-adminreportsettings"></a>获取 adminReportSettings

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 Microsoft 365 报表的租户级设置。

> **注意：** 有关不同报表视图和名称的详细信息，请 [参阅管理中心的 Microsoft 365 报表 - Microsoft 365 应用版使用情况](/microsoft-365/admin/activity-reports/microsoft365-apps-usage)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）           |
|:---------------------------------------|:------------------------------------------------------|
| 委派（工作或学校帐户）     | ReportSettings.Read.All、ReportSettings.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。                                        |
| 应用程序                            | ReportSettings.Read.All、ReportSettings.ReadWrite.All |

> **注意：** 对于允许应用代表用户获取报表设置的委派权限，租户管理员必须为用户分配相应的 Azure Active Directory 受限管理员角色。 有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /admin/reportSettings
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [adminReportSettings](../resources/adminreportsettings.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "get_adminreportsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/reportSettings
```

### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.adminReportSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.adminReportSettings",
    "displayConcealedNames": true
  }
}
```
