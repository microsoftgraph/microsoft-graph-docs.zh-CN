---
author: JeremyKelley
ms.date: 09/10/2017
title: 获取特殊文件夹
ms.localizationpriority: medium
ms.prod: sharepoint
description: 使用特殊集合可以按名称访问特殊文件夹。
doc_type: apiPageType
ms.openlocfilehash: 6b836ea0a2be134c498eb02c3c73566a9085d163
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695389"
---
# <a name="get-a-special-folder-by-name"></a>按名称获取特殊文件夹

命名空间：microsoft.graph

使用特殊集合可以按名称访问特殊文件夹。

特殊文件夹可以提供简单别名来访问 OneDrive 中的已知文件夹，无需按路径查找（需要本地化）或通过 ID 引用文件夹。如果特殊文件夹被重命名或移到驱动器中的其他位置，此语法将继续查找该文件夹。

应用程序第一次尝试向特殊文件夹中写入内容时，如果特殊文件夹不存在，系统会自动创建特殊文件夹。如果用户删除某个特殊文件夹，再次向其写入内容时会重新创建特殊文件夹。

> **注意：** 如果你拥有只读权限并且请求不存在的特殊文件夹，将收到 `403 Forbidden` 错误。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|            权限类型             |                                           权限（从最低特权到最高特权）                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| 委派（工作或学校帐户）     | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All                            |
| 委派（个人 Microsoft 帐户） | Files.ReadWrite.AppFolder、Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |
| 应用程序                            | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All                                                         |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored"} -->

```http
GET /me/drive/special/{name}
```

### <a name="special-folder-names"></a>特殊文件夹名称

以下是 OneDrive 和 OneDrive for Business 中可用的特殊文件夹名称。

| 名称        | 文件夹 ID    | 说明                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| Documents   | `documents`  | “文档”文件夹。                                                    |
| Photos      | `photos`     | “照片”文件夹。                                                       |
| Camera Roll | `cameraroll` | “本机照片备份”文件夹。                                           |
| App Root    | `approot`    | 应用程序的个人文件夹。通常位于 `/Apps/{Application Name}` 中 |
| Music       | `music`      | “音乐”文件夹。                                                        |


### <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 `$expand` 和 `$select` [OData 查询参数](/graph/query-parameters)自定义响应。

## <a name="response"></a>响应

此方法在响应正文中返回 `200 OK` 响应代码和 [driveItem](../resources/driveitem.md) 对象。

可以将此处理特殊文件夹内联的方法与对 driveItem 上的属性或关系的其他调用结合使用。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "Documents",
  "eTag": "012345819293.1",
  "specialFolder": {
    "name": "documents"
  }
}
```

## <a name="get-children-of-a-special-folder"></a>获取特殊文件夹的子文件夹

若要请求特殊文件夹的子文件夹，则可以请求 `children` 集合，或使用 [expand](/graph/query-parameters) 选项展开子集合。

### <a name="http-request"></a>HTTP 请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/special/{special-folder-name}/children
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-special-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-special-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-special-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-special-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048 },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ]
}
```

## <a name="remarks"></a>说明

> **注意：** 带有 `specialFolder` facet 的 DriveItem 指示项目是特殊文件夹，且可以通过 `special` 集合访问。

如果应用拥有只读权限，且特殊文件夹尚不存在，那么可能无法请求获取特殊文件夹或其子项，响应为 `404 Not Found` 或 `403 Forbidden` 错误。

<!-- {
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders",
  "suppressions": [
  ]
} -->

