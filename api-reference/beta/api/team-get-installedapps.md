---
title: 在团队中获取已安装的应用程序
description: 获取团队中安装的应用程序。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 49903514fb6345978d90ca1df7a8ab5279c61410
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564151"
---
# <a name="get-installed-app-in-team"></a>在团队中获取已安装的应用程序

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索在指定[团队](../resources/team.md)中安装的[应用程序](../resources/teamsappinstallation.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | TeamsAppInstallation、ReadWriteSelfForTeam、TeamsAppInstallation、、、、、、、all、all、all 和 all 的所有读写。 |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | TeamsAppInstallation、ReadWriteSelfForTeam、TeamsAppInstallation、Group. all、、、、all、all、all、all 和 All 的所有读写。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a>请求标头

| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [teamsAppInstallation](../resources/teamsappinstallation.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-get-the-installed-app"></a>示例1：获取已安装的应用程序
#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->

```msgraph-interactive
GET /teams/{id}/installedApps/{id}
```

---

#### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-the-installed-app"></a>示例2：获取已安装应用程序的名称和其他详细信息

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}?$expand=teamsAppDefinition
```

---

#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps_expand",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "displayName": "OneNote",
                "version": "beta"
            }
        }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

