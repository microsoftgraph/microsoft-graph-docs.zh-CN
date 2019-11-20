---
title: 创建架构
description: 为 Microsoft Search 连接创建架构。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 201f2c474dd0ecdd38b14cbb6af3cb009b51fa82
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747238"
---
# <a name="create-schema"></a>创建架构

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为 Microsoft Search[连接](../resources/externalconnection.md)创建架构。

支持以下两种架构类型：自定义项和文件。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持。 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | ExternalItem.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections/{id}/schema
```

## <a name="request-headers"></a>请求标头

| 名称                  | 说明                                          |
|:----------------------|:-----------------------------------------------------|
| Authorization         | Bearer {token}。必需。                            |
| Content-Type          | application/json. Required.                          |
| 首选：响应-async | 使用此来导致请求以异步方式执行。 可选。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供[架构](../resources/schema.md)对象的 JSON 表示形式。

注册自`schema`定义项目架构时，对象的`baseType`属性必须设置为`microsoft.graph.externalItem` ，并且必须包含`properties`属性。 该`properties`对象必须至少包含一个属性，最多为64。

注册文件架构时， `schema`对象的`baseType`属性必须设置为。 `microsoft.graph.externalFile`

## <a name="response"></a>响应

在请求`Prefer: respond-async`中包含标头的情况下，如果成功，此方法`202 Accepted`将在`Location`响应标头中返回响应代码和 URL，该 URL 可用于[获取操作状态](../api/connectionoperation-get.md)。

如果在`Prefer: respond-async`请求中不包含标头，则此方法在响应正文`201 Created`中返回响应代码和新[架构](../resources/schema.md)对象。

> [!NOTE]
> 创建架构是一个容易导致网关超时的长时间运行的过程。 `Prefer: respond-async`建议使用，以避免超时错误。

## <a name="examples"></a>示例

### <a name="example-1-register-custom-schema-asynchronously"></a>示例1：异步注册自定义架构

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async"
}-->

```http
POST https://graph.microsoft.com/beta/connections/contosohr/schema
Content-type: application/json
Prefer: respond-async

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "title",
      "type": "String",
      "isSearchable": "true",
      "isRetrievable": "true"
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": "true",
      "isRetrievable": "true"
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": "true"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-async-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-async-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-async-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a>响应
<!-- markdownlint-enable MD024 -->

下面是一个响应示例。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
```

### <a name="example-2-register-file-schema-synchronously"></a>示例2：同步注册文件架构

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a>请求
<!-- markdownlint-enable MD024 -->

下面展示了示例请求。

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection"
}-->

```http
POST https://graph.microsoft.com/beta/connections/contosofiles/schema
Content-type: application/json

{
  "baseType": "microsoft.graph.externalFile"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a>响应
<!-- markdownlint-enable MD024 -->

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schema"
} -->

```http
HTTP/1.1 201 Created

{
  "baseType": "microsoft.graph.externalFile"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
