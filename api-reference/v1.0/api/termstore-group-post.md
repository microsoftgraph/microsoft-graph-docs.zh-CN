---
title: 创建组
description: 在术语存储中创建新的组对象。
author: vishriv
ms.localizationpriority: medium
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: ff08b50016ff40065ec09c462f6f14bd6d8face4
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60947449"
---
# <a name="create-termstore-group"></a>创建 termStore 组
命名空间：microsoft.graph.termStore

在术语 [存储中](../resources/termstore-group.md) 创建新的组对象。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户） |TermStore.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST sites/{site-id}/termStore/groups
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供[组](../resources/termstore-group.md)对象的 JSON 表示形式。

下表显示创建 group 对象 [时所需的属性](../resources/termstore-group.md) 。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|要创建的组的名称。|



## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [microsoft.graph.termStore.group](../resources/termstore-group.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "displayName": "myGroup"
}-->

``` http
POST https://graph.microsoft.com/v1.0/sites/microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74/termStore/groups
Content-Type: application/json

{
  "displayName" : "myGroup"
}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
}-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "85825593-5593-8582-9355-828593558285",
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "displayName": "myGroup"  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Create termGroup",
  "suppressions": [
  ]
}
-->


