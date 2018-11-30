---
title: 创建 MailFolder
description: 使用此 API 新建子 MailFolder。
ms.openlocfilehash: 79ed32a316a9012c33d3c08d0c95f00ad2f90725
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011106"
---
# <a name="create-mailfolder"></a>创建 MailFolder

使用此 API 新建子 MailFolder。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:----------------|:--------------------------------------------|
|委派（工作或学校帐户） | Mail.ReadWrite    |
|委派（个人 Microsoft 帐户） | Mail.ReadWrite    |
|应用程序 | Mail.ReadWrite |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

查询 URL 为文件夹 ID 或已知文件夹名称中指定的父文件夹。 有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。

## <a name="request-headers"></a>请求标头

| 标头 | 值 |
|:-------|:------|
| Authorization | `Bearer {token}`. 必需。 |
| Content-Type | `application/json`. 必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。 **displayName**是[mailFolder](../resources/mailfolder.md)对象的唯一可写属性。

| 参数 | 类型 | 说明 |
|:----------|:-----|:------------|
|displayName|String|新文件夹的显示名称。|

## <a name="response"></a>响应

如果成功，此方法返回`201 Created`响应代码和响应正文的[mailFolder](../resources/mailfolder.md)资源。

## <a name="example"></a>示例

##### <a name="request"></a>请求

下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

##### <a name="response"></a>响应
下面是一个响应示例。

> **注意：** 可能为便于阅读缩短如下所示的响应对象。 所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
