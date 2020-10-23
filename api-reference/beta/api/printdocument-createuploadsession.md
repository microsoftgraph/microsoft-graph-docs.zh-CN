---
title: printDocument： createUploadSession
description: 创建一个上载会话，以以迭代方式上载 printDocument 的二进制文件的范围。
localization_priority: Normal
author: nilakhan
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 47043b64806cfa9ef3a66026a60b84ae11112168
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704942"
---
# <a name="printdocument-createuploadsession"></a>printDocument： createUploadSession

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建一个上载会话，该会话允许应用程序以迭代方式上载链接到打印文档的二进制文件的范围。

作为响应的一部分，此操作将返回可在后续顺序查询中使用的上载 URL `PUT` 。 每个操作的请求标头 `PUT` 可用于指定要上载的确切字节范围。 这样，如果在上载过程中断开网络连接，则可以恢复传输。 

## <a name="permissions"></a>权限

若要调用此 API，必须有以下权限之一。 要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。
除了以下权限之外，用户或应用程序的租户必须具有活动的通用打印订阅，并且拥有授予 [获取打印机](printer-get.md) 或 [获取 printerShare](printershare-get.md) 访问权限的权限，具体取决于打印机或 printerShare 是否正在使用。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | PrintJob，PrintJob。 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | PrintJob.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

若要使用 **打印机**创建上载会话，请执行以下操作： 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

使用 **printerShare**创建上传会话的步骤： 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}。必需。 |
| Content-type | application/json. Required.|


## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型        | 说明 |
|:-------------|:------------|:------------|
|properties|[printDocumentUploadProperties](../resources/printDocumentUploadProperties.md)|表示要上载的二进制文件的属性。|

## <a name="response"></a>响应

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和新的 [uploadSession](../resources/uploadsession.md) 对象。

>**注意**：作为**uploadSession** response 对象的一部分返回的**uploadUrl**属性是一个不透明的 URL，用于随后的 `PUT` 查询，用于上传文件的字节范围。 它包含针对 ExpirationDateTime 到期的后续查询的相应 auth 令牌 `PUT` 。 **expirationDateTime** 请勿更改此 URL。

## <a name="examples"></a>示例

下面的示例演示如何创建可在后续文件上载操作中用于指定 printDocument 的上载会话。

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
}-->
```http
POST https://graph.microsoft.com/beta/print/shares/1c879027-5120-4aaf-954a-ebfd509a3bcc/jobs/46207/documents/9001bcd9-e36a-4f51-bfc6-140c3ad7f9f7/createUploadSession
Content-type: application/json

{
  "properties": {
    "documentName": "TestFile.pdf",
    "contentType": "application/pdf", 
    "size": 4533322
  }
}
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}",
    "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
    "nextExpectedRanges": [
        "0-4533321"
    ]
}
```
