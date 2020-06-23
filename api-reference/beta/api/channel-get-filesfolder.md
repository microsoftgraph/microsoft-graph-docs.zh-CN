---
title: 获取 "获取"
description: 检索频道的 "工作" 导航路径。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d10e0758e0d323f17534c1651268b74fd077fd3d
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845335"
---
# <a name="get-filesfolder"></a>获取 "获取"

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取存储[通道](../resources/channel.md)文件的位置的元数据。 

## <a name="permissions"></a>Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 文件. All、Group. all、Group、Group。全部。    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 文件. All、Group. all、Group、Group。全部。     |


## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/filesFolder

```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法不支持[OData 查询参数](/graph/query-parameters)来自定义响应。

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}. Required.  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [driveItem](../resources/driveitem.md) 对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "get_filesFolder"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/filesFolder
```
### <a name="response"></a>响应
下面展示了示例响应。 

>**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('32e3b156-66b2-4135-9aeb-73295a35a55b')/channels('19%3Af253e46c035b42308e9a4a22a87037af%40thread.skype')/filesFolder/$entity",
    "id": "01H7CFEKENJSSIUHGADZBKODARINQC5JMD",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "lastModifiedDateTime": "2020-01-23T18:47:13Z",
    "name": "Documentation Planning",
    "webUrl": "https://microsoft.sharepoint.com/teams/ExtensibilityandFundamentals/Shared%20Documents/Documentation%20Planning",
    "size": 2374080,
    "parentReference": {
        "driveId": "b!2SInBlQrN0K8-GXMy9qNsPtI5ScW8C5IlZtycoy6ZpJZRRtgE4qVTrE8wrvL0-hd",
        "driveType": "documentLibrary"
    },
    "fileSystemInfo": {
        "createdDateTime": "2020-01-23T18:47:12Z",
        "lastModifiedDateTime": "2020-01-23T18:47:13Z"
    },
    "folder": {
        "childCount": 7
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get filesFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

