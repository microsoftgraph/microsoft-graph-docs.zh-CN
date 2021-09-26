---
title: 获取 workbookOperation
description: 检索 workbookOperation 对象的状态。
ms.localizationpriority: medium
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 36268886b2b46ffc02c2bbf4e0da36dad36dc14a
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767039"
---
# <a name="get-workbookoperation"></a>获取 workbookOperation

命名空间：microsoft.graph

如果单独调用此 url，则无意义。 此请求是 excel 的所有异步请求的一部分。 这用于检索 [workbookOperation 对象](../resources/workbookoperation.md) 的状态。

目前并非所有请求都支持异步。 以创建会话请求为例。

发出异步[创建会话](./workbook-createsession.md)请求，按照文档操作，你可以获取状态代码，异步操作从此处开始，你可以从位置部分的响应标头找到此文档 `202 Accepted` 所需的URL。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Files.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/items/{id}/workbook/operations/{operation-id}
```

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | Bearer {token}。必需。 |
| Workbook-Session-Id  | 确定是否保留更改的工作簿会话 ID。 可选。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [workbookOperation](../resources/workbookoperation.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

#### <a name="response-running"></a>响应正在运行

以下是状态为 的响应 `running` 。 获取此状态后，再次轮询请求，直到收到相同的响应。


<!-- {
  "blockType": "response",
  "truncated": true,
  "sampleKeys": ["0195cfac-bd22-4f91-b276-dece0aa2378b"],
  "@odata.type": "microsoft.graph.workbookOperation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0195cfac-bd22-4f91-b276-dece0aa2378b",
  "status": "running"
}
```

#### <a name="response-succeeded"></a>响应成功

以下是状态为 的响应 `succeeded` 。 **resourceLocation** 是一组 URL，表示原始长时间运行的操作的返回值。 请参阅下表，详细了解如何从 **resourceLocation** 属性获取结果。

| 操作      |resourceLocation|
|:----------|:----------|
| 创建会话 | [sessionInfoResource](../resources/workbooksessioninfo.md) |
| 创建 tableRow | [tableRowOperationResult](./workbook-tablerowoperationresult.md) |
| 删除 tableRow| 不需要 resourceLocation。 |

<!-- {
  "blockType": "response",
  "truncated": true,
  "sampleKeys": ["01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ", "0195cfac-bd22-4f91-b276-dece0aa2378b", "Y2x1c3Rlcj1QU0c0JnNlc3Npb249MTUuU0cyUEVQRjAwMDI4RjI1MS5BMTE2LjEuVTM2LmM4MGRiNjkwLTQwMTktNGNkNS1hYWJiLTJmYzczM2YxZTQ5ZjE0LjUuZW4tVVM1LmVuLVVTMjQuMTAwM2JmZmRhYzUyMzkzOS1Qcml2YXRlMS5TMjQuJTJmUEI0JTJmWjJqZmt1aXhJZHBjeE8xYmclM2QlM2QxNi4xNi4wLjE0NDEwLjM1MDUwMTQuNS5lbi1VUzUuZW4tVVMxLk0xLk4wLjEuUyZ1c2lkPWExOTMyNTU0LTlhNDAtNzYzNi1mNDU3LWEyNjExMmFkNDg2YQ=="],
  "@odata.type": "microsoft.graph.workbookOperation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0195cfac-bd22-4f91-b276-dece0aa2378b",
  "status": "succeeded",
  "resourceLocation":"https://graph.microsoft.com/beta/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/sessionInfoResource(key='0195cfac-bd22-4f91-b276-dece0aa2378b')?sessionId=Y2x1c3Rlcj1QU0c0JnNlc3Npb249MTUuU0cyUEVQRjAwMDI4RjI1MS5BMTE2LjEuVTM2LmM4MGRiNjkwLTQwMTktNGNkNS1hYWJiLTJmYzczM2YxZTQ5ZjE0LjUuZW4tVVM1LmVuLVVTMjQuMTAwM2JmZmRhYzUyMzkzOS1Qcml2YXRlMS5TMjQuJTJmUEI0JTJmWjJqZmt1aXhJZHBjeE8xYmclM2QlM2QxNi4xNi4wLjE0NDEwLjM1MDUwMTQuNS5lbi1VUzUuZW4tVVMxLk0xLk4wLjEuUyZ1c2lkPWExOTMyNTU0LTlhNDAtNzYzNi1mNDU3LWEyNjExMmFkNDg2YQ=="
}
```

#### <a name="response-failed"></a>响应失败

以下是状态为 的响应 `failed` 。

<!-- {
  "blockType": "response",
  "truncated": true,
  "sampleKeys": ["0195cfac-bd22-4f91-b276-dece0aa2378b"],
  "@odata.type": "microsoft.graph.workbookOperation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0195cfac-bd22-4f91-b276-dece0aa2378b",
  "status": "failed",
  "error":
  {
      "code": "internalServerError",
      "message": "An internal server error occurred while processing the request.",
      "innerError": {
          "code": ""internalServerErrorUncategorized",
          "message": "An unspecified error has occurred.",
          "innerError": {
               "code": "GenericFileOpenError",
               "message": "The workbook cannot be opened."
          }
      }
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workbookOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

