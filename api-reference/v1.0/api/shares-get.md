---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 访问共享项目
localization_priority: Normal
ms.openlocfilehash: 1f172060a8b30996ff09b3ca93390da503db9fea
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480654"
---
# <a name="accessing-shared-driveitems"></a>访问共享 DriveItem

通过使用 **shareId** 或共享 URL 访问共享 [DriveItem](../resources/driveitem.md) 或共享项目集合。

要与此 API 一起使用共享 URL，应用需要[将此 URL 转换为共享令牌](#encoding-sharing-urls)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.ReadWrite、Files.ReadWrite.All    |
|应用程序 | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a>路径参数

| 参数名称                 | 值    | 说明                                                                         |
|:-------------------------------|:---------|:------------------------------------------------------------------------------------|
| **shareIdOrEncodedSharingUrl** | `string` | 必需。 API 返回的共享令牌或正确编码的共享 URL。 |

### <a name="encoding-sharing-urls"></a>编码共享 URL

若要编码共享 URL，请使用以下逻辑：

1. 首先，使用 base64 编码 URL。
2. 删除值末尾的 [](https://en.wikipedia.org/wiki/Base64) 字符，将 `=` 替换成 `/`，将 `_` 替换成 `+`，从而将 base64 编码结果转换成`-`。
3. 将 `u!` 追加到字符串的开头。

例如，若要对 URL 进行 C# 编码，请使用以下代码：

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="optional-request-headers"></a>可选的请求标头

| 名称       | 类型   | 说明                                                    |
|:-----------|:-------|:---------------------------------------------------------------|
| **Prefer** | 字符串 | 可选。 将设置为以下记录`prefer`的值之一。  |

### <a name="prefer-header-values"></a>首选标头值

| 名称                          | 说明                                                                                             |
|:------------------------------|:--------------------------------------------------------------------------------------------------------|
| redeemSharingLink             | 如果**shareIdOrEncodedSharingUrl**是共享链接, 则向呼叫者授予对项目的持久访问权限    |
| redeemSharingLinkIfNecessary  | 与 redeemSharingLink 相同, 但仅保证在此请求的持续时间内授予访问权限 |

应将 redeemSharingLink 视为与调用者导航到共享链接的调用者导航到浏览器 (接受共享手势), 而 redeemSharingLinkIfNecessary 的目的是专门用于查看链接的metadata.

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [sharedDriveItem](../resources/shareddriveitem.md) 资源。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是一个请求检索共享项目的示例：

<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="response"></a>响应

下面是一个响应示例。

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.sharedDriveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "B64397C8-07AE-43E4-920E-32BFB4331A5B",
  "name": "contoso project.docx",
  "owner": {
    "user": {
      "id": "98E88F1C-F8DC-47CC-A406-C090248B30E5",
      "displayName": "Ryan Gregg"
    }
  }
}
```

## <a name="access-the-shared-item-directly"></a>直接访问共享项目

虽然 [**SharedDriveItem**](../resources/shareddriveitem.md) 包含一些有用的信息，但大多数应用程序都需要直接访问共享 [DriveItem](../resources/driveitem.md)。**SharedDriveItem** 资源包括**根**和**项目**关系，这些关系可以访问共享项目范围内的内容。

## <a name="example-single-file"></a>示例（单个文件）

### <a name="request"></a>请求

通过请求 **driveItem** 关系，将返回共享的 **DriveItem**。

<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```

### <a name="response"></a>响应

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

## <a name="example-shared-folder"></a>示例（共享文件夹）

### <a name="request"></a>请求

通过请求 **driveItem** 关系并展开**子**集合，将同时返回共享的 **DriveItem** 以及共享文件夹内的文件。

<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```

### <a name="response"></a>响应

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {},
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <a name="error-responses"></a>错误响应

请参阅[错误响应][error-response]主题，详细了解错误返回方式。

## <a name="remarks"></a>注解

* 对于 OneDrive for Business 和 SharePoint，共享 API 始终要求进行身份验证，无法用于在没有用户上下文的情况下访问匿名共享内容。

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link"
} -->
