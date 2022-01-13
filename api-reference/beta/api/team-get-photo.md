---
title: 获取团队照片
description: 获取团队的照片（图片）。
author: akjo
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3e05c5ab8ab5bcf9650285dd7e9c24fffad06b4a
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61862781"
---
# <a name="get-team-photo"></a>获取团队照片

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取团队的照片（图片），或者获取照片的元数据。

此方法会先尝试从 Microsoft 365 中检索指定的照片。 如果 Microsoft 365 中没有此照片，则它会改为尝试在 Active Directory 中检索照片。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Team.ReadBasic.All、TeamSettings.Read.All、TeamSettings.ReadWrite.All、Group.Read.All **、Group.ReadWrite.All**、Directory.Read.All **、Directory.ReadWrite.All** |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | TeamSettings.Read.Group *、TeamSettings.ReadWrite.Group*、Team.ReadBasic.All、TeamSettings.Read.All、TeamSettings.ReadWrite.All、Group.Read.All **、Group.ReadWrite.All**、Directory.Read.All **、Directory.ReadWrite.All**  |

> **注意**：标有 * 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。 标记为 **的权限已弃用，不应使用。

> **注意**：此 API 支持管理员权限。全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。

## <a name="http-request"></a>HTTP 请求

### <a name="get-the-metadata-of-the-photo"></a>获取照片的元数据

此终结点将返回照片的元数据。

<!-- {
  "blockType": "ignored"
}-->

```http
GET /teams/{id}/photo
```

### <a name="get-the-photo"></a>获取照片

此终结点将在二进制数据中检索照片。

<!-- {
  "blockType": "ignored"
}-->

```http
GET /beta/teams/{id}/photo/$value
```

## <a name="request-headers"></a>请求标头

| 标头        | 值           |
|:--------------|:--------------  |
| Authorization | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此请求的正文。

## <a name="response"></a>响应

### <a name="response-for-getting-the-metadata-of-a-photo"></a>针对获取照片元数据的响应

如果成功，此方法会返回 `200 OK` 响应代码和照片元数据。

### <a name="response-for-getting-the-photo"></a>针对获取照片的响应

如果成功，此方法会返回 `200 OK` 响应代码和照片的二进制数据。

## <a name="examples"></a>示例

### <a name="example-1-get-the-photo-metadata"></a>示例 1：获取照片元数据

#### <a name="request"></a>请求

下述示例展示了要获取团队照片元数据的请求。

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo_metadata"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo
```

#### <a name="response"></a>响应

下面是一个响应示例。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

### <a name="example-2-get-the-team-photos-binary-data"></a>示例 2：获取团队照片的二进制数据

以下示例展示了要获取团队照片二进制数据的请求。

#### <a name="request"></a>请求

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo/$value
```

#### <a name="response"></a>响应

包含所请求照片的二进制数据。HTTP 响应代码为 200。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


