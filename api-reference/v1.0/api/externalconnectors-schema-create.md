---
title: 创建架构
description: 为连接创建Microsoft 搜索架构。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6f271195136a3a469de871e3f17fec5e485ff86c
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580710"
---
# <a name="create-schema"></a>创建架构
命名空间：microsoft.graph.externalConnectors



创建新的 [架构](../resources/externalconnectors-schema.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|不适用|
|委派（个人 Microsoft 帐户）|不适用|
|应用程序| ExternalConnection.ReadWrite.OwnedBy|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /external/connections/{id}/schema
```
在请求正文中，提供架构对象的 JSON [表示](../resources/externalconnectors-schema.md) 形式。

注册自定义项架构时， `schema` 对象必须将 `baseType` 属性设置为 `microsoft.graph.externalItem` ，并且必须包含 `properties` 属性。 `properties`对象必须至少包含一个属性，最多包含 64 个属性。

## <a name="response"></a>响应

在请求中包含 标头后，如果成功，此方法在响应标头中返回 响应代码和 `Prefer: respond-async` `202 Accepted` URL，可用于 `Location` [获取操作状态](../api/externalconnectors-connectionoperation-get.md)。

如果请求中不包含 标头，如果成功，此方法在响应正文中返回 响应 `Prefer: respond-async` `201 Created` 代码和新[](../resources/externalconnectors-schema.md)架构对象。

> [!NOTE]
> 创建架构是一个长时间运行的过程，容易出现网关超时。 我们建议使用 `Prefer: respond-async` 标头以避免超时错误。

## <a name="examples"></a>示例

### <a name="example-register-custom-schema-asynchronously"></a>示例：异步注册自定义架构

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async",
  "@odata.type": "microsoft.graph.externalConnectors.schema"
}-->

```http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/schema
Content-type: application/json
Prefer: respond-async

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "String",
      "isSearchable": "true",
      "isRetrievable": "true",
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": "true",
      "isRetrievable": "true",
      "isSearchable": "false"
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": "true"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-async-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-async-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-async-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schema-from-connection-async-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
```
