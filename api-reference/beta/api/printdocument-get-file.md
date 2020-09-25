---
title: 下载 printDocument 二进制文件
description: 下载与文档相关联的二进制文件。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a7e7de914d8549472e08c23f65af25ca99542a58
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273654"
---
# <a name="download-printdocument-binary-file"></a>下载 printDocument 二进制文件

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

下载与 [printDocument](../resources/printdocument.md)相关联的二进制文件。 调用此方法将生成一个重定向响应，该响应具有可用于下载有效负载的预验证的 URL。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户或应用程序的租户必须具有活动的通用打印订阅，并且具有授予 [获取打印机](printer-get.md) 访问权限的权限。

| 权限类型                        | 权限（从最低特权到最高特权）                  |
| :------------------------------------- | :----------------------------------------------------------- |
| 委派（工作或学校帐户）     | PrintJob、PrintJob、PrintJob、PrintJob、All 和 All |
| 委派（个人 Microsoft 帐户） | 不支持。                                               |
| 应用程序                            | PrintJob、PrintJob 和所有                    |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}/documents/{id}/$value
```
## <a name="request-headers"></a>请求标头
| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法 `302 Found` 将在位置标头中返回和预验证的下载 URL。

## <a name="examples"></a>示例
下面的示例演示如何调用此 API 以获取预先验证的下载 URL。 若要开始下载，请遵循响应中的重定向 URL。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```http
GET https://graph.microsoft.com/beta/print/printers/fcb0bc53-a446-41d0-bfc3-5c56cdbb0f2a/jobs/46140/documents/bd260b1a-044e-4ca6-afa9-17d9a587d254/$value
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Accepted
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
