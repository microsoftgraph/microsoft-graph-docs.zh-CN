---
title: List taskTriggers
description: 检索与打印机关联的任务触发器列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 189830fb76de676163a24a8166cff6017cceffc5
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565893"
---
# <a name="list-tasktriggers"></a>List taskTriggers

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索与[打印机](../resources/printer.md)关联的[任务触发器](../resources/printtasktrigger.md)列表。 任务触发器列表定义由于打印过程中发生的事件而将触发的任务。

有关如何使用此 API 将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持请求打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| Printer。 all，完全控制，All，All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/taskTriggers
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

### <a name="exceptions"></a>Exceptions
某些运算符不受支持：、、、、 `$count` `$format` `$search` `$select` `$skip` 、 `$top` 。

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[printTaskTrigger](../resources/printtasktrigger.md)对象集合。
## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer_tasktriggers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/taskTriggers
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-tasktriggers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-tasktriggers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-tasktriggers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('fcc7fe6a-5ba7-4059-8017-702f3a41c8a4')/taskTriggers",
  "value": [
    {
      "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
      "event": "jobStarted"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List taskTriggers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
