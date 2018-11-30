---
title: Microsoft Graph 安全 API 错误响应
description: 返回使用标准 HTTP 206 部分内容状态代码和传递通过警告标头中 Microsoft Graph 中的 Microsoft Graph 安全 API 的错误。
ms.openlocfilehash: 35af0a1ed4c4bf7f6e1afb36039f812ab59f64dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011436"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Microsoft Graph 安全 API 错误响应

返回使用标准 HTTP 206 部分内容状态代码和传递通过警告标头中 Microsoft Graph 中的 Microsoft Graph 安全 API 的错误。

Microsoft Graph 安全 API 为从所有数据提供程序接收多个响应联合的服务。 由 Microsoft Graph 安全 API 收到 HTTP 错误时，它将发送回警告标头采用以下格式：<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

一个数据提供程序返回之外的 2xx 或 404 错误代码时，此警告标头将只发送回客户端。 例如：

- 如果未授予对资源的访问权限，则可能会返回 HttpStatusCode.Forbidden (403)。
- 如果提供程序超时，警告标头中返回 HttpStatusCode.GatewayTimeout (504)。
- 如果内部的提供程序错误发生的情况，警告标头中使用 HttpStatusCode.InternalServerError (500)。

如果数据提供程序返回 2xx 或 404，它不显示警告标头因为需要以获得成功进行这些代码时，或者在未分别找到数据。 在联合系统中，如多次数据到一个或多个，但不是所有的提供程序仅已知预期 404 找不到。

## <a name="example"></a>示例

用户询问的`security/alerts/{alert_id}`。

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

由于 404 和 200 是预期的条件，警告头包含以下信息： 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **注意：** 每个 HTTP 标头是子项，集合，以便用户可以枚举警告标头，并检查所有项目。

## <a name="see-also"></a>另请参阅

如果您遇到授权时遇到问题，请参阅我们的[博客文章](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2)。
