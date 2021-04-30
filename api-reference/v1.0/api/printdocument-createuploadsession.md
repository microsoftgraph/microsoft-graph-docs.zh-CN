---
title: printDocument： createUploadSession
description: 创建上载会话以迭代上载 printDocument 的二进制文件范围。
localization_priority: Normal
author: nilakhan
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 164a5ca3bf6b2f53c3c5952d49f605493b4d9275
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080083"
---
# <a name="printdocument-createuploadsession"></a>printDocument： createUploadSession
命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

创建允许应用反复上载链接到打印文档的二进制文件范围的上载会话。

作为响应的一部分，此操作返回可用于后续顺序查询的上载 `PUT` URL。 每个操作的请求头可用于指定要 `PUT` 上载的字节的确切范围。 这允许恢复传输，以防在上载过程中网络连接中断。 

>**注意**：只有在关联的打印作业上存在 [printTask](../resources/printTask.md) 状态（由请求应用创建的触发器启动）时，使用应用程序权限创建上载 `processing` 会话才能成功。 若要详细了解如何注册任务触发器，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有根据使用的打印机还是 printerShare 授予获取 [打印机](printer-get.md) 或获取 [printerShare](printershare-get.md) 访问权限的权限。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | PrintJob.Create、PrintJob.ReadWrite、PrintJob.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | PrintJob.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

若要使用打印机创建上载 **会话**： 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

若要使用 **printerShare (** 仅受委派权限支持，请) ： 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型        | 说明 |
|:-------------|:------------|:------------|
|properties|[printDocumentUploadProperties](../resources/printDocumentUploadProperties.md)|表示要上载的二进制文件的属性。|

请求正文中 **contentType** 属性的值应受 printer/printerShare 支持。 可以通过获取 [printer/printerShare 的 printerCapabilities](../resources/printercapabilities.md) 获取受支持的内容类型。 

对于 **将 OXPS 转换为 PDF，** 你需要为支持 的 `application/oxps` printer/printerShare 传递为 `application/pdf` contentType。 当满足以下所有条件 **时，通用** 打印会将 OXPS 转换为 **PDF：** 
1.  打印机/打印机共享在 `application/pdf` **printerCapabilities 中支持**。 
2.  `application/oxps` **printerCapabilities 不支持打印机/打印机共享**。 
3.  请求正文中 **contentType** 属性的值为 `application/oxps` 。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和新 [uploadSession](../resources/uploadsession.md) 对象。

>**注意**：作为 **uploadSession** 响应对象的一部分返回的 **uploadUrl** 属性是后续查询用于上载文件的字节范围的不透明 `PUT` URL。 它包含过期 `PUT` **expirationDateTime 的后续查询的适当身份验证令牌**。 不要更改此 URL。

## <a name="examples"></a>示例

以下示例演示如何创建可用于后续文件上载操作到指定 printDocument 的上载会话。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "printdocument_createuploadsession"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/createUploadSession
Content-Type: application/json
Content-length: 96

{
  "properties": {
    "documentName": "TestFile.pdf",
    "contentType": "application/pdf", 
    "size": 4533322
  }
}
```


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}",
    "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
    "nextExpectedRanges": [
        "0-4533321"
    ]
}
```

