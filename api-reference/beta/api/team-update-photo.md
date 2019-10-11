---
title: 更新团队照片
description: 更新团队的照片（图片）。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6c19e09713d16f8c2739b1a8398509953a19ddd0
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418333"
---
# <a name="update-team-photo"></a>更新团队照片

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新团队的照片（图片）。 Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648 像素。 如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。

> [!Note]
> 请求的总大小不得超过 4 MB。 这会将照片大小限制为小于 4 MB。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Group.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}-->

```http
PUT /beta/teams/{id}/photo
```

## <a name="request-headers"></a>请求标头

| 标头        | 值           |
|:--------------|:--------------  |
| Authorization | Bearer {token}。必需。  |
| Content-type | image/jpeg。必需。  |

## <a name="request-body"></a>请求正文

在请求正文中包括照片的二进制数据。

## <a name="response"></a>响应

如果成功，此方法返回 `200 OK` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是更新团队照片的请求示例。

<!-- {
  "blockType": "ignored",
  "name": "update_team_photo"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{id}/photo
Content-type: image/jpeg

{
  <Binary data for the image>
}
```

### <a name="response"></a>响应 

下面是一个响应示例。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update team photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
