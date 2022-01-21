---
title: contentType：addCopyFromContentTypeHub
description: 将已发布内容类型的副本从内容类型中心添加或同步到目标网站或列表。
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: 39b147c1c75b535962eaa70d4120304b4e4634ca
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162229"
---
# <a name="contenttype-addcopyfromcontenttypehub"></a>contentType：addCopyFromContentTypeHub
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将已发布内容类型的副本从内容类型中心添加或同步到目标[网站或](../resources/site.md)[列表](../resources/list.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户） | Sites.Manage.All、Sites.FullControl.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Sites.Manage.All、Sites.FullControl.All |


## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /sites/{siteId}/lists/{listId}/contentTypes/addCopyFromContentTypeHub
POST /sites/{siteId}/contentTypes/addCopyFromContentTypeHub
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|说明|
|:---|:---|:---|
|contentTypeId|String| 要添加到目标网站或列表的内容类型集线器中的内容类型的 ID。|



## <a name="response"></a>响应

如果成功，此操作将在响应正文中返回 响应代码和 contentType 对象（如果内容类型是同步添加的）或响应代码（如果内容类型将异步 `200 OK` [](../resources/contenttype.md) `202 Accepted` 同步）。 该响应还将包含一个标头，其中包含为处理复制/同步而创建的 `Location` [richLongRunningOperation](../resources/richLongRunningOperation.md) 的位置。对于异步操作，最多可能需要 70 分钟才能同步或添加内容类型。

## <a name="examples"></a>示例

### <a name="example-1-synchronous-pull"></a>示例 1：同步拉取

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "contenttype_addcopyfromcontenttypehub"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/{siteId}/lists/{listId}/contentTypes/addCopyFromContentTypeHub
Content-Type: application/json
Content-length: 33

{
  "contentTypeId": "String"
}
```


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.contentType",
    "id": "String (identifier)",
    "description": "String",
    "group": "String",
    "hidden": "Boolean",
    "isBuiltIn": "Boolean",
    "name": "String"
  }
}
```
### <a name="example-2-asynchronous-pull"></a>示例 2：异步拉取

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "contenttype_addcopyfromcontenttypehub"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/{siteId}/lists/{listId}/contentTypes/addCopyFromContentTypeHub
Content-Type: application/json
Content-length: 33

{
  "contentTypeId": "String"
}
```


#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
}
-->
``` http
HTTP/1.1 202 Accepted
location: https://graph.microsoft.com/beta/sites/{siteId}/lists/{listId}/operations/{operationId}
```
