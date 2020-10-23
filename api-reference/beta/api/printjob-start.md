---
title: printJob： start
description: 将打印作业提交到关联的打印机或 printerShare。 任何现有的挂起作业完成、终止或取消后都将打印。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a78e55b0c3c317c350bcc321fe3463a4541693f1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48714769"
---
# <a name="printjob-start"></a>printJob： start

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将打印作业提交到关联的 [打印机](../resources/printer.md) 或 [printerShare](../resources/printershare.md)。 它将在任何现有的挂起 **作业** 完成、终止或取消后进行打印。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户或应用程序的租户还必须具有活动的通用打印订阅，并且拥有授予 [获取打印机](printer-get.md) 或 [获取 printerShare](printershare-get.md) 的权限，具体取决于打印机或 printerShare 是否正在使用。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| PrintJob、ReadWriteBasic、PrintJob、All、ReadWriteBasic、All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| 不支持。 |

## <a name="http-request"></a>HTTP 请求
```http
POST /print/shares/{id}/jobs/{id}/start
```
## <a name="request-headers"></a>请求标头
| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提交此方法的请求正文。 

## <a name="response"></a>响应
如果成功，此方法 `200 OK` 在正文中返回响应代码和 [printJobStatus](../resources/printjobstatus.md) 对象。

## <a name="example"></a>示例
以下示例演示如何调用此 API。
##### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/print/shares/{id}/jobs/{id}/start
```

##### <a name="response"></a>响应
下面展示了示例响应。 
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

```http
HTTP/1.1 200 OK

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```


