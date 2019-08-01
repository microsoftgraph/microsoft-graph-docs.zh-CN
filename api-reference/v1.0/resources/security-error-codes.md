---
title: Microsoft Graph 安全性 API 错误响应
description: Microsoft Graph 安全性 API 中的错误使用标准的 HTTP 206 部分内容状态代码返回, 并通过警告标头进行传递。
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: 2d77a0f21623a98e4041b845e92a23c7574a415d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034466"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Microsoft Graph 安全性 API 错误响应

Microsoft Graph 安全性 API 中的错误使用标准的 HTTP 206 部分内容状态代码返回, 并通过警告标头进行传递。

## <a name="errors"></a>错误

Microsoft Graph 安全性 API 是一种联合服务, 可接收来自所有数据提供程序的多个响应。 当 Microsoft Graph 安全性 API 收到 HTTP 错误时, 它将以以下格式返回一个警告标头:
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

仅当其中一个数据提供程序返回了2xx 或404之外的错误代码时, 此警告标头才会发送回客户端。 例如：

- 如果未授予对资源的访问权限, 则可能会返回 HttpStatusCode (403)。
- 如果提供程序超时, 则在警告标头中返回 HttpStatusCode GatewayTimeout (504)。
- 如果发生内部提供程序错误, 则在警告标头中使用 InternalServerError (500) HttpStatusCode。

如果数据提供程序返回2xx 或 404, 则它不会显示在警告标头中, 因为这些代码是成功的, 或者是在不分别找到数据时。 在联合系统中, 未找到404的次数预期数据只对一个或多个 (但不是所有) 提供程序已知。

## <a name="example"></a>示例

用户请求`security/alerts/{alert_id}`。

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

由于404和200都是预期条件, 因此警告标头包含以下内容:

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **注意:** 每个 HTTP 标头都是一个子项集合, 因此用户可以枚举警告标头并选中所有项目。

## <a name="constraints"></a>约束

Odata 查询参数的限制为1000个警报, 而`$top`  +  `$skip` odata 查询参数的组合不能超过6000个警报。 `$top` 例如，`/security/alerts?$top=10&$skip=5990` 将返回 `200 OK` 响应代码，但 `/security/alerts?$top=10&$skip=5991` 将返回 `400 Bad Request` 响应代码。

此限制的解决方法是将`$filter` OData 查询参数与 Microsoft GRAPH 安全 API 中`eventDateTime`的 alert 实体结合使用, `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}`并将 dateTime 值替换为最后的 (6000th) 警报。 您还可以为设置区域`eventDateTime`;例如,*警报？ $filter = eventDateTime **gt** 2018-11-**11**T00:00: 00.000 z&eventDateTime **lt** 2018-11-**12**T00:00: 00.000 z*

## <a name="see-also"></a>另请参阅

如果您在使用授权时遇到问题, 请参阅[授权和 Microsoft Graph 安全性 API](/graph/security-authorization)。
