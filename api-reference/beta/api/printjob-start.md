---
title: printJob：start
description: 将打印作业提交到关联的打印机或 printerShare。 完成、中止或取消任何现有待定作业后，将打印该作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 288e3b8cfcd1458f7d71c8fb43ae57ac97237e56
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049875"
---
# <a name="printjob-start"></a>printJob：start

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将打印作业提交到关联的 [打印机或](../resources/printer.md) [printerShare](../resources/printershare.md)。 将在完成、中止或取消任何现有待定作业后打印该作业。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有根据所使用的打印机还是 printerShare 授予获取 [打印机](printer-get.md) 或获取 [printerShare](printershare-get.md) 的权限。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| PrintJob.Create、PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All |
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
如果成功，此方法在 `200 OK` 正文中返回 响应代码和 [printJobStatus](../resources/printjobstatus.md) 对象。

## <a name="example"></a>示例
以下示例演示如何调用此 API。
##### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/print/shares/{id}/jobs/{id}/start
```

##### <a name="response"></a>响应
下面展示了示例响应。 
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

```http
HTTP/1.1 200 OK

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```


