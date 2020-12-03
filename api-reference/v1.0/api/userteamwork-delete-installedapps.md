---
title: 为用户卸载应用
description: 卸载指定用户的个人范围内的应用。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aeb49691e8bf85abbefc86805783ff6aa0991c7d
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564027"
---
# <a name="uninstall-app-for-user"></a>为用户卸载应用

命名空间：microsoft.graph

从指定[用户](../resources/user.md)的个人作用域中卸载[应用程序](../resources/teamsappinstallation.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | ReadWriteSelfForUser、TeamsAppInstallation、TeamsAppInstallation TeamsAppInstallation |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | TeamsAppInstallation、TeamsAppInstallation、all、TeamsAppInstallation、All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/teamwork/installedApps/{id}
```

## <a name="request-headers"></a>请求标头

| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "user_delete_teamsApp"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk
```

### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User delete teamsAppInstallations,
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
