---
title: 下载 printDocument 二进制文件
description: 下载与文档关联的二进制文件。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 7808484095c576ce23cfc0cbda7a3d637ec7c784
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60927933"
---
# <a name="download-printdocument-binary-file"></a>下载 printDocument 二进制文件

命名空间：microsoft.graph

下载与 [printDocument 关联的二进制文件](../resources/printdocument.md)。 调用此方法会生成重定向响应，该响应具有可用于下载有效负载的预验证 URL。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有授予获取打印机[访问权限的权限。](printer-get.md)

| 权限类型                        | 权限（从最低特权到最高特权）                  |
| :------------------------------------- | :----------------------------------------------------------- |
| 委派（工作或学校帐户）     | PrintJob.Read、PrintJob.Read.All、PrintJob.ReadWrite、PrintJob.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。                                               |
| 应用程序                            | PrintJob.Read.All、PrintJob.ReadWrite.All                    |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/$value
```
## <a name="request-headers"></a>请求标头
| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在 Location 标头中返回 和预先 `302 Found` 验证的下载 URL。

## <a name="examples"></a>示例
以下示例演示如何调用此 API 以获取预先验证的下载 URL。 若要开始下载，请遵循响应中的重定向 URL。

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/$value
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-document-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-document-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-document-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-document-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Found
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
