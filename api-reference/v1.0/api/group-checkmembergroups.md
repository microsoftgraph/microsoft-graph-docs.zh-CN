---
title: 组：checkMemberGroups
description: 检查指定组列表中的成员身份。
author: Jordanndahl
ms.localizationpriority: high
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 94e7a00d8a8fb45aed1016e9d322959833c78437
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59114503"
---
# <a name="group-checkmembergroups"></a>组：checkMemberGroups

命名空间：microsoft.graph

检查指定组列表中的成员身份。将列表中具有直接或可传递成员身份的指定组返回。

每个请求最多可检查 20 个组。此功能支持 Microsoft 365 和 Azure AD 中设置的其他类型的组。注意：Microsoft 365 组无法包含组。因此，Microsoft 365 组中的成员身份始终是直接的。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| 委派（工作或学校帐户）     | GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All |
| 委派（个人 Microsoft 帐户） | 不支持。                                                                              |
| 应用程序                            | GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All                               |



## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a>请求标头

| 名称          | 类型   | 说明               |
| :------------ | :----- | :------------------------ |
| Authorization | string | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数 | 类型              | 说明           |
| :-------- | :---------------- | :-------------------- |
| groupIds  | String collection | 组 ID 的数组 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。

## <a name="example"></a>示例

下面是一个如何调用此 API 的示例。

##### <a name="request"></a>请求

下面是一个请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应

这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

