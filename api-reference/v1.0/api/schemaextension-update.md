---
title: 更新 schemaExtension
description: 更新指定架构Extension 定义中的属性。
ms.localizationpriority: medium
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 29c4e625e026eb65908db36cb123f50b45ffd931
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296456"
---
# <a name="update-schemaextension"></a>更新 schemaExtension

命名空间：microsoft.graph

更新指定 [架构Extension](../resources/schemaextension.md) 定义中的属性。 仅当扩展处于或`Available`状态时，才能对扩展`InDevelopment`进行附加更新。 这意味着无法从定义中删除自定义属性或目标资源类型，但可以添加新的自定义属性并更改扩展说明。

更新适用于扩展的 **targetTypes** 属性中包含的所有资源。 这些资源是 [支持资源类型](/graph/extensibility-overview#supported-resources)之一。

对于委派流，只要扩展的 **所有者** 属性设置为已登录用户拥有的应用程序的 **appId** ，登录用户就可以更新架构扩展。 该应用程序可以是最初创建扩展的应用程序，也可以是已登录用户拥有的其他应用程序。 

**所有者** 属性的此条件允许已登录用户通过他们不拥有的其他应用程序（例如 Microsoft Graph Explorer）进行更新。 使用Graph资源管理器更新 **schemaExtension** 资源时，请将 **所有者** 属性包含在 PATCH 请求正文中。 有关详细信息，请参阅 [Microsoft Graph 的“已知问题](/graph/known-issues)”中的[“扩展](/graph/known-issues#extensions)”部分。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Application.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Application.ReadWrite.All 和 Directory.ReadWrite.All |

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
|properties|[extensionSchemaProperty](../resources/extensionschemaproperty.md) 集合|构成架构扩展定义的属性名称和类型的集合。 仅允许进行添加性更改。 |
|状态|String|架构扩展的生命周期状态。 创建时的初始状态是 `InDevelopment`。 可能的状态转换是从`InDevelopment`来到`Available``Available`向`Deprecated`。|
|targetTypes|String collection|架构扩展适用的支持扩展的 Microsoft Graph 类型集。  仅允许进行添加性更改。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。 尝试从不拥有 (且未将 **所有者** 属性设置为你拥有的应用程序的 **appId** 的应用程序运行此请求) 返回 `403 Forbidden` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。 如果从不拥有的应用程序运行请求，则必须包括 **所有者** 属性。 在这种情况下，请将 **所有者** 属性设置为你拥有的应用程序的 **appId** 。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/exto6x7sfft_courses
Content-type: application/json

{
    "owner": "ef4cb9a8-97c3-4ca7-854b-5cb5ced376fa",
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        },
        {
            "name": "courseSupervisors",
            "type": "String"
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-schemaextension-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-schemaextension-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

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

