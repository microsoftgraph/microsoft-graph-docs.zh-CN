---
title: call： keepAlive
description: 每15至45分钟向此 API 发出一次请求，以确保正在进行的呼叫仍处于活动状态。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 50eec71f674f9f2dfaef1e405b7261c47199f5e6
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871755"
---
# <a name="call-keepalive"></a>call： keepAlive

每15至45分钟向此 API 发出一次请求，以确保正在进行的呼叫仍处于活动状态。 在45分钟内未收到此请求的呼叫被视为非活动状态，随后将结束。

必须在前一个请求的45分钟内或开始呼叫开始时至少执行一次成功的请求。

我们建议您以较短的时间间隔（每15分钟）发送请求。 确保这些请求成功，以阻止调用超时和结束。

尝试向已结束的呼叫发送请求将导致`404 Not-Found`错误。 应在应用程序一侧清理与此呼叫相关的资源。

## <a name="permissions"></a>权限
若要调用此 API，可能需要以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
| :-------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | 不支持        |
| 委派（个人 Microsoft 帐户） | 不支持        |
| 应用程序     | 无                                        |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/keepAlive
```


## <a name="request-headers"></a>请求标头
| 名称          | 说明               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
此方法返回一个`200 OK` HTTP 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。

<!-- {
  "blockType": "request",
  "name": "keep-alive"
}-->

```http
POST https://graph.microsoft.com/beta/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab/keepAlive
```

### <a name="response"></a>响应
以下示例显示了相应的响应。
<!-- {
  "blockType": "response",
  "name": "keep-alive",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 200 OK
```


<!--
{
  "type": "#page.annotation",
  "description": "call: keepAlive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
