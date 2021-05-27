---
title: 删除 acceptedSender
description: '从接受发件人列表中删除用户或组。 '
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f06e44853c7b78e50ff41a2569f4509ee232b6a3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681867"
---
# <a name="remove-acceptedsender"></a>删除 acceptedSender

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从指定组的接受发件人列表中删除用户或组。 

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）  |
|:---------------------------------------|:-------------------------------------------- |
| 委派（工作或学校帐户）     | Group.ReadWrite.All    |
| 委派（个人 Microsoft 帐户） | 不支持。|
| 应用程序                            | 不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id={id}
```

## <a name="request-headers"></a>请求标头
| 标头         | 值                      |
|:---------------|:---------------------------|
| Authorization  | Bearer {token}。必需。  

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例
### <a name="example-1-remove-a-user-from-the-accepted-senders-list-for-the-group"></a>示例 1：从组的接受发件人列表中删除用户。
#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "remove_user_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{user-id}
```

#### <a name="response"></a>响应
下面介绍响应示例。 

<!-- {
  "blockType": "response",
  "name": "remove_user_from_acceptedsenderslist_of_group",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-accepted-senders-list-for-the-group"></a>示例 2：从该组的接受发件人列表中删除组。
#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "remove_group_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a>响应
下面展示了示例响应。 

<!-- {
  "blockType": "response",
  "name": "remove_group_from_acceptedsenderslist_of_group",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


