---
title: 删除 profileCardProperty
description: 删除 profileCardProperty 对象并删除配置文件卡片中的所有自定义项。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 2dffcc667281d26fb64e44dd7cd45e8e0f1c313f
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080688"
---
# <a name="delete-profilecardproperty"></a>删除 profileCardProperty

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从组织的配置文件卡片中删除由其指定的[profileCardProperty](../resources/profilecardproperty.md)对象 `directoryPropertyName` ，并删除该属性的所有本地化的自定义项。

## <a name="permissions"></a>权限

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 所有用户读写。          |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用程序                            | 不支持。                              |

>**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/organization/settings/profileCardProperties/{directoryPropertyName-Value}
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明    |
|:--------------|:---------------|
| Authorization | Bearer {token}. Required. |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面的示例演示如何从组织的配置文件卡片中删除名为 "Fax" 的属性。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_profilecardproperty"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/settings/profileCardProperties/fax
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-profilecardproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-profilecardproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete profileCardProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
