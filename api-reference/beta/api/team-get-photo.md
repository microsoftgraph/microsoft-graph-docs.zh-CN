---
title: 获取团队照片
description: 获取团队的照片（图片）。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 72351adf71257c9d8ba10e86a7b017ad865bbc21
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971417"
---
# <a name="get-team-photo"></a>获取团队照片

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取团队的照片（图片），或者获取照片的元数据。 通常情况下，最佳做法是先尝试在元数据中检索想要获取的照片的尺寸，以确保该尺寸可用。 检索到元数据后，使用 `/$value` 路径获取照片的二进制数据。

此方法会先尝试从 Microsoft 365 中检索指定的照片。 如果 Microsoft 365 中没有此照片，则它会改为尝试在 Active Directory 中检索照片。

Microsoft 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648 像素。 如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。

可以获取最大可用照片的元数据，或者也可以指定一个大小来获取该照片大小的元数据。如果请求的大小不可用，仍可获取较小的大小。例如，如果上载的最大照片像素为 504x504 的照片，则除大小为 648x648 的照片之外的所有照片都可供下载。如果在 Microsoft 365 或 Azure Active Directory 中没有可用的指定大小，则会返回 1x1 的大小和剩余的元数据。

> [!Note]
> REST 请求的总大小不得超过 4 MB。 这将照片尺寸限制为小于 4 MB。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All  |

> **注意**：标有 * 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。

> **注意**：此 API 支持管理员权限。全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。

## <a name="http-request"></a>HTTP 请求

### <a name="get-the-metadata-of-the-photo"></a>获取照片的元数据

此终结点将返回照片的元数据。 如果未指定尺寸，则将返回可供使用的最大照片尺寸的元数据。

<!-- {
  "blockType": "ignored"
}-->

```http
GET /teams/{id}/photo
GET /teams/{id}/photo/{size}
```

### <a name="get-the-photo"></a>获取照片

此终结点将在二进制数据中检索照片。 如果未指定尺寸，则将返回可供使用的最大尺寸。

<!-- {
  "blockType": "ignored"
}-->

```http
GET /beta/teams/{id}/photo/$value
GET /beta/teams/{id}/photo/{size}/$value
```

## <a name="path-parameters"></a>路径参数

此方法支持用可选路径参数来指定要检索的照片尺寸。 指定的尺寸不得超过最大可用尺寸。 获取照片元数据以确定最大可用尺寸。

|**参数**|**类型**|**说明**|
|:-----|:-----|:-----|
|size  |String  | 照片尺寸。 Microsoft 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。 如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。 可选。|

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

### <a name="example-2-get-a-specific-size-of-the-team-photo"></a>示例 2：获取团队照片的特定尺寸

下述示例展示了要获取特定尺寸的团队照片的请求。

#### <a name="request"></a>请求

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo/240x240/$value
```

#### <a name="response"></a>响应

包含所请求的 240x240 照片的二进制数据。HTTP 响应代码为 200。

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


