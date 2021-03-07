---
title: 下载 printDocument 二进制文件
description: 下载与文档关联的二进制文件。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 7bde42e03af509f101515dc847283fc1e354c478
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517281"
---
# <a name="download-printdocument-binary-file"></a>下载 printDocument 二进制文件

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

下载与 [printDocument 关联的二进制文件](../resources/printdocument.md)。 调用此方法会生成重定向响应，该响应具有可用于下载有效负载的预身份验证 URL。

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
如果成功，此方法在位置标头中返回和 `302 Found` 预先验证的下载 URL。

## <a name="examples"></a>示例
以下示例演示如何调用此 API 以获取预先验证的下载 URL。 若要开始下载，请按照响应中的重定向 URL 执行。

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/$value
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Found
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
