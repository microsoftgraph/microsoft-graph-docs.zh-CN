---
title: printDocument： uploadData
description: Upload printDocument 的单个二进制段。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6435a36e7713435dce3f38145d48083bdabcc532
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787595"
---
# <a name="printdocument-uploaddata"></a>printDocument： uploadData

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Upload printDocument 的单个二 **进制段**。

您可以上载整个文件，或将文件拆分为多个字节范围，只要请求不超过 1 MB。

可按任意顺序上传文件的片段，并且最多可并行上传四个并发请求。 当上载文档的所有二进制段时，二进制文件将链接到 **printJob**。

## <a name="permissions"></a>权限
需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有授予 [获取](printer-get.md) 打印机访问权限的权限。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| PrintJob.ReadWrite、PrintJob.ReadWrite.All |
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
| 范围 | bytes={startByteIndex}-{endByteIndex}  |
| Content-Length | {contentLength}  |
| Content-type  | application/json. Required.|

## <a name="request-body"></a>请求正文
请求正文是一个二进制 blob，其中包含在 `Range` 标头中指定为 非独占 字节范围的文档的字节数。 

## <a name="response"></a>响应
如果成功，此方法将返回以下响应之一。 它不会在响应正文中返回任何内容。

| 条件     | 响应代码 |
|:--------------|:--------------|
| 仍然需要上载一个或多个二进制段 | `202 Accepted` |
| 已成功上载所有二进制段 | `201 Created` |

## <a name="example"></a>示例
以下示例演示如何调用此 API 上载文档前 72797 个字节。
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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printdocument-uploaddata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应

缺少一个或多个分段：
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

收到的所有分段：
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 201 Created
```


