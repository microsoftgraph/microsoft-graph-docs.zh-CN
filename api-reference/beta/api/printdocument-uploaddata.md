---
title: printDocument： uploadData
description: 上载 printDocument 的单个二进制段。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 62277a2b933edf9161a51b114c765fde948b4d26
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674013"
---
# <a name="printdocument-uploaddata"></a>printDocument： uploadData

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

上载 **printDocument**的单个二进制段。

您可以上传整个文件，或将文件拆分为多个字节范围，前提是没有请求大于 1 MB。

可以按任意顺序上载文件的各个部分，并且可以并行上传，最大并发请求数为四个。 当上载文档的所有二进制片段时，二进制文件将链接到 **printJob**。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户或应用程序的租户必须具有活动的通用打印订阅，并且具有授予 [获取打印机](printer-get.md) 访问权限的权限。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| PrintJob，PrintJob。 |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/uploadData
```
## <a name="request-headers"></a>请求标头
| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}。必需。 |
| Range | bytes = {startByteIndex}-{endByteIndex}  |
| Content-Length | {contentLength}‬  |
| Content-type  | application/json. Required.|

## <a name="request-body"></a>请求正文
请求正文是一个二进制 blob，其中包含指定为标头中的非独占字节范围的文档的字节数 `Range` 。 

## <a name="response"></a>响应
如果成功，此方法将返回以下响应之一。 它不在响应正文中返回任何内容。

| Condition     | 响应代码 |
|:--------------|:--------------|
| 仍需上载一个或多个二进制段 | `202 Accepted` |
| 已成功上载所有二进制段 | `201 Created` |

## <a name="example"></a>示例
下面的示例演示如何调用此 API 以上载文档的前72797个字节。
##### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printdocument-uploaddata"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/documents/{id}/uploadData
Range: bytes=0-72796
Content-Length: 72797
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printdocument-uploaddata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printdocument-uploaddata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printdocument-uploaddata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应

缺少一个或多个段：
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 202 Accepted
```

接收的所有段：
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 201 Created
```
