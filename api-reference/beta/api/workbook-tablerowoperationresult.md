---
title: workbook： tableRowOperationResult
description: 异步创建 tableRow 请求的一部分。
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: apiPageTypes
ms.openlocfilehash: 8f9dd564012ce9e873fa5567773f555beb1bc82c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136731"
---
# <a name="workbook-tablerowoperationresult"></a>workbook： tableRowOperationResult
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

此函数是异步创建 [workbookTableRow](../resources/workbooktablerow.md) 资源的一系列步骤中的最后一个函数。

创建多个表行的最佳实践是在一个 [create tableRow](./table-post-rows.md) 操作中批处理这些行，并异步执行该操作。

创建表行的异步请求涉及以下步骤：
1. 发出异步创建 [tableRow](./table-post-rows.md) 请求并获取响应标头中返回的 `Location` 查询 URL。
2. 使用步骤 1 返回的查询 URL 发出 [Get workbookOperation](./workbookoperation-get.md) 请求并获取步骤 3 的操作 ID。 
   或者，为方便起见，在获取 operationStatus 结果后，可以从响应中返回的 `succeeded` [workbookOperation](../resources/workbookoperation.md)的 **resourceLocation** 属性获取查询 URL，将查询 URL 应用到步骤 3。 
3. 使用步骤 2 返回的查询 URL 作为此函数 **tableRowOperationResult** 的 GET 请求 URL。 成功的函数调用将返回 [workbookTableRow](../resources/workbooktablerow.md) 资源中的新表行。

如果单独调用此函数，则此函数不执行任何工作。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Files.ReadWrite|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/drive/items/{id}/workbook/tableRowOperationResult(key={operation-id})
GET /me/drive/root:/{item-path}:/workbook/tableRowOperationResult(key={operation-id})
```

## <a name="function-parameters"></a>函数参数
请求 URL 需要以下查询参数。 

|参数|类型|Description|
|:---|:---|:---|
|Key|String|在之前的 Get **workbookOperation** 请求中返回的 [workbookOperation](./workbookoperation-get.md)响应中提供的 **operationId。**|


## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
| Workbook-Session-Id  | 确定是否保留更改的工作簿会话 ID。 可选。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此函数在响应 `200 OK` 正文中返回 响应代码和 [workbookTableRow](../resources/workbooktablerow.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
以下示例显示了一个请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["0195cfac-bd22-4f91-b276-dece0aa2378b"],
  "name": "workbook_tablerowoperationresult"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/tableRowOperationResult(key='0195cfac-bd22-4f91-b276-dece0aa2378b')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbook-tablerowoperationresult-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbook-tablerowoperationresult-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbook-tablerowoperationresult-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbook-tablerowoperationresult-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "index": 99,
  "values": "[[1, 2, 3]]"
}
```
