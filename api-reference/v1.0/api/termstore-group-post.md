---
title: 创建 termStore 组
description: 在术语存储中创建新的组对象。
author: vishriv
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: b8bd550ea4d310099385a6cb9b522250db273612
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191779"
---
# <a name="create-termstore-group"></a>创建 termStore 组
命名空间：microsoft.graph.termStore

在术语存储中创建新的 [组](../resources/termstore-group.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户） |TermStore.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | 不支持。 |

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

下表显示了创建 [组](../resources/termstore-group.md) 对象时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|要创建的组的名称。|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [microsoft.graph.termStore.group](../resources/termstore-group.md) 对象。

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


