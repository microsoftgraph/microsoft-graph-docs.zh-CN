---
title: 更新 schemaExtension
description: 更新指定 schemaExtension 的定义中的属性。
ms.localizationpriority: medium
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 2cfe89bb5ece2c691976e21a81bcbe33680713a1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59099272"
---
# <a name="update-schemaextension"></a>更新 schemaExtension

命名空间：microsoft.graph

更新指定 [schemaExtension 的定义中的属性](../resources/schemaextension.md)。 

这意味着无法从定义中删除自定义属性或目标资源类型，但可以添加新的自定义属性并更改扩展的说明。

只有当扩展位于"开发中"或"可用"状态时，才能对 **扩展进行附加****更新。** 

此更新适用于扩展的 **targetTypes** 属性中包含的所有资源。 这些资源是支持 [的资源类型之一](/graph/extensibility-overview#supported-resources)。

对于委派流，登录用户可以更新架构扩展，只要该扩展的所有者属性设置为已登录用户拥有的应用程序的 **appId。** 该应用程序可以是最初创建扩展的应用程序，或者是登录用户拥有的一些其他应用程序。 

owner 属性 **的** 此条件允许登录用户通过他们并不拥有的其他应用程序（如 Microsoft Graph Explorer）进行更新。 使用 Graph Explorer 更新 **schemaExtension** 资源时，请包含 PATCH 请求正文中的 owner 属性。 有关详细信息，请参阅 Microsoft [](/graph/known-issues#extensions) Graph[已知问题中的扩展Graph。](/graph/known-issues)

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Application.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a>可选的请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Content-Type   | application/json |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|说明|String|架构扩展的说明。|
|properties|[extensionSchemaProperty](../resources/extensionschemaproperty.md) 集合|构成架构扩展定义的属性名称和类型的集合。 只允许进行增量更改。 |
|status|String|架构扩展的生命周期状态。 创建时的初始状态为 **InDevelopment**。 可能的状态转换从"开发 **中"转换为****"可用**"和 **"** 可用"**到"已弃用"。**|
|targetTypes|String collection|架构扩展适用的支持扩展的 Microsoft Graph 类型集。  只允许进行增量更改。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

##### <a name="request"></a>请求

下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用架构扩展向组添加自定义数据](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

