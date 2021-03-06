---
title: Microsoft Graph 安全性 API 错误响应
description: Microsoft Graph 安全性 API 中的错误使用标准的 HTTP 206 部分内容状态代码返回，并通过警告标头进行传递。
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: c36cf3be4cf24a2831918acd994a36bbcfc9e489
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988924"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Microsoft Graph 安全性 API 错误响应

命名空间：microsoft.graph

Microsoft Graph 安全性 API 中的错误使用标准的 HTTP 206 部分内容状态代码返回，并通过警告标头进行传递。

## <a name="errors"></a>错误

Microsoft Graph 安全性 API 是一种联合服务，可接收来自所有数据提供程序的多个响应。 当 Microsoft Graph 安全性 API 收到 HTTP 错误时，它将以以下格式返回一个警告标头：
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

仅当其中一个数据提供程序返回了2xx 或404之外的错误代码时，此警告标头才会发送回客户端。 例如：

- 如果未授予对资源的访问权限，则可能会返回 HttpStatusCode (403) 。
- 如果提供程序超时，则在警告标头中返回 HttpStatusCode (504) 。
- 如果发生内部提供程序错误，则在警告标头中使用 InternalServerError (500) HttpStatusCode。

如果数据提供程序返回2xx 或404，则它不会显示在警告标头中，因为这些代码是成功的，或者是在不分别找到数据时。 在联合系统中，未找到404的次数预期数据只对一个或多个（但不是所有）提供程序已知。

## <a name="example"></a>示例

用户请求 `security/alerts/{alert_id}` 。

```
Provider 1: 404 (provider does not have a record of this alert ID)
Provider 2: 504 (provider timed out)
Provider 3: 200 (success)
Provider 4: 403 (customer has not licensed this provider)
```

由于404和200都是预期条件，因此警告标头包含以下内容：

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **注意：** 每个 HTTP 标头都是一个子项集合，因此用户可以枚举警告标头并选中所有项目。

## <a name="threat-indicator-bulk-action-errors"></a>威胁指示器批量操作错误

 (创建、更新、删除) 的批量操作可生成两个不同的潜在错误代码：

- 400错误代码指示提供的正文在序列化过程中出现错误。
- 206错误代码指示在将一个或多个批量操作与提供程序联合时失败。 响应将包含各个提供商针对每个威胁情报指标的成功/错误数据。 与 [警报](/graph/api/resources/security-api-overview?view=graph-rest-1.0#alerts)不同，所有潜在的错误信息将包含在 [tiIndicator](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) 批量操作的响应正文中。

## <a name="constraints"></a>约束

`$top`OData 查询参数限制为1000个警报。 建议你在第一个 GET 查询中仅包括 `$top`，而不包括 `$skip`。 可使用 `@odata.nextLink` 进行分页。 如果需要使用 `$skip`，它具有 500 个警报的限制。 例如，`/security/alerts?$top=10&$skip=500` 将返回 `200 OK` 响应代码，但 `/security/alerts?$top=10&$skip=501` 将返回 `400 Bad Request` 响应代码。 有关详细信息，请参阅 [Microsoft Graph 安全性 API 错误响应](../resources/security-error-codes.md)。

此限制的解决方法是将 `$filter` OData 查询参数与 `eventDateTime` Microsoft GRAPH 安全 API 中的 alert 实体结合使用， `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` 并将 dateTime 值替换为最后一个 (1500th) 警报。 您还可以为设置区域 `eventDateTime` ; 例如， `alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z` 。

## <a name="see-also"></a>另请参阅

如果您在使用授权时遇到问题，请参阅 [授权和 Microsoft Graph 安全性 API](/graph/security-authorization)。


