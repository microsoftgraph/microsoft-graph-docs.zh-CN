---
title: Microsoft Graph 安全 API 错误响应
description: 返回使用标准 HTTP 206 部分内容状态代码和传递通过警告标头中 Microsoft Graph 安全 API 的错误。
ms.openlocfilehash: 9ac124f763e7668471f89beffb968cb883217e80
ms.sourcegitcommit: 4aebfaefc23e02a98b2fec35958cd2110020f15f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/06/2018
ms.locfileid: "27184495"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Microsoft Graph 安全 API 错误响应

返回使用标准 HTTP 206 部分内容状态代码和传递通过警告标头中 Microsoft Graph 安全 API 的错误。

## <a name="errors"></a>错误

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

## <a name="constraints"></a>约束

`$top` OData 查询参数的限制为 1000年警报和组合`$top`  +  `$skip`参数不能超过 6000 通知的 OData 查询。 例如，`/security/alerts?$top=10&$skip=5990`会返回`200 OK`响应代码，但`/security/alerts?$top=10&$skip=5991`将返回`400 Bad Request`响应代码。

解决此限制的方法是使用`$filter`OData 查询参数`eventDateTime`从 Microsoft Graph 安全 API，警报实体的使用`?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}`和 dateTime 值替换 (6000th) 的最后一个通知。 您还可以设置范围`eventDateTime`;例如， *alerts?$ filter = eventDateTime **gt** 2018-11-**11**T00:00:00.000Z = eventDateTime **lt** 2018-11-**12**T00:00:00.000Z*

## <a name="see-also"></a>另请参阅

如果您遇到授权时遇到问题，请参阅[Authorization and Microsoft Graph 安全 API](/graph/security-authorization)。
