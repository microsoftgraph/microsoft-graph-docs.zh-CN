---
title: 'printJob: startPrintJob'
description: 将打印作业提交到关联打印机。 任何现有的挂起作业完成、终止或取消后都将打印。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7c1ba6a188acdfa022af10ff0e31fca65f579517
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674167"
---
# <a name="printjob-startprintjob"></a>printJob: startPrintJob

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将打印作业提交到关联 [打印机](../resources/printer.md)。 它将在任何现有的挂起 **作业** 完成、终止或取消后进行打印。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户或应用程序的租户必须具有活动的通用打印订阅，并且具有授予 [获取打印机](printer-get.md) 访问权限的权限。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| PrintJob、ReadWriteBasic、PrintJob、All、ReadWriteBasic、All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| 不支持。 |

## <a name="http-request"></a>HTTP 请求
```http
POST /print/printers/{id}/jobs/{id}/startPrintJob
```
## <a name="request-headers"></a>请求标头
| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提交此 metho 的请求正文。 

## <a name="response"></a>响应
如果成功，此方法 `200 OK` 在正文中返回响应代码和 [printJobStatus](../resources/printjobstatus.md) 对象。

## <a name="example"></a>示例
以下示例演示如何调用此 API。
##### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/startPrintJob
```

##### <a name="response"></a>响应
下面展示了示例响应。 
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

```http
HTTP/1.1 200 OK

{
    "processingState": "processing",
    "processingStateDescription": "The print job is currently being processed.",
    "acquiredByPrinter": false
}
```
