---
author: JeremyKelley
ms.date: 09/10/2017
title: 列出与我共享的文件
ms.localizationpriority: high
ms.prod: sharepoint
description: 检索已与驱动器所有者共享的 DriveItem 资源的集合。
doc_type: apiPageType
ms.openlocfilehash: 5b6c28f38c92e11ca6ba145b7a6e9a5585aec752
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59090682"
---
# <a name="list-items-shared-with-the-signed-in-user"></a>列出与已登录用户共享的项目

命名空间：microsoft.graph

检索已与[驱动器](../resources/drive.md)所有者共享的 [DriveItem](../resources/driveitem.md) 资源的集合。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.Read.All、Files.ReadWrite.All    |
|应用程序 | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |

**注意：** 虽然 /sharedWithMe 请求可通过 Files.Read 或 Files.ReadWrite 权限成功发出，但一些属性可能会丢失。
此外，如果没有 **All** 权限之一，则无法访问从此 API 返回的共享项。

## <a name="http-request"></a>HTTP 请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "shared-with-me", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```msgraph-interactive
GET /me/drive/sharedWithMe
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shared-with-me-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shared-with-me-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shared-with-me-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shared-with-me-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a>响应

此方法返回 [DriveItem](../resources/driveitem.md) 资源的集合，这些资源包含已与驱动器所有者共享的 DriveItem 资源。在此示例中，由于此驱动器是用户的默认驱动器，此方法将返回与已登录用户共享的项目。

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc",
      "remoteItem": {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    },
    {
      "id": "1312def",
      "remoteItem": {
        "id": "1991210caf!1991",
        "name": "Team Roster.xlsx",
        "file": { },
        "size": 37619,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a>注解

从 **sharedWithMe** 操作返回的 driveItem 始终都将包括 [**remoteItem**](../resources/remoteitem.md) 方面，这表明它们是其他驱动器中的项目。若要访问共享的 DriveItem 资源，你将需要使用 **remoteItem** 中提供的信息发出请求，信息格式如下：

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

默认情况下，**sharedWithMe** 将返回在你自己的租户内共享的项目。 若要包括从外部租户共享的项目，请将 `?allowexternal=true` 附加到 GET 请求。



<!-- {
  "type": "#page.annotation",
  "description": "List the items shared with the owner of a drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Sharing/Shared with me",
  "suppressions": [
  ]
} -->

