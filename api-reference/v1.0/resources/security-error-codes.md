---
title: Microsoft Graph 安全 API 错误响应
description: Microsoft 安全Graph API 中的错误是使用标准 HTTP 206 部分内容状态代码返回的，并且通过警告标头传递。
author: preetikr
ms.localizationpriority: medium
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: 329b3e9da2276631963f763e756560aa8f9fdc70
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137502"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Microsoft Graph 安全 API 错误响应

命名空间：microsoft.graph

Microsoft 安全Graph API 中的错误是使用标准 HTTP 206 部分内容状态代码返回的，并且通过警告标头传递。

## <a name="errors"></a>错误

Microsoft Graph 安全性 API 是一项联合服务，可接收来自所有数据提供程序的多个响应。 当 Microsoft Graph 安全 API 收到 HTTP 错误时，它将以以下格式发送回警告标头：
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

此警告标头仅在其中一个数据提供程序返回 2xx 或 404 外的错误代码时发送回客户端。 例如：

- 如果未授予 (，) 返回 HttpStatusCode.Forbidden) 403。
- 如果提供程序出现问题，则警告标头 (504) HttpStatusCode.GatewayTimeout。
- 如果发生内部提供程序错误，警告标头 (500) HttpStatusCode.InternalServerError。

如果数据提供程序返回 2xx 或 404，则它将不会显示在警告标头中，因为这些代码预期会成功或找不到数据。 在联合系统中，找不到 404 是预期数据的多次，因为只有一个或多个（但不是全部）提供程序知道数据。

## <a name="example"></a>示例

用户要求 `security/alerts/{alert_id}` 。

```
Provider 1: 404 (provider does not have a record of this alert ID)
Provider 2: 504 (provider timed out)
Provider 3: 200 (success)
Provider 4: 403 (customer has not licensed this provider)
```

由于 404 和 200 都是预期条件，因此警告标头包含以下内容：

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **注意：** 每个 HTTP 标头都是子网站的集合，因此用户可以枚举警告标头并检查所有项目。

## <a name="constraints"></a>约束

`$top`OData 查询参数的限制为 1000 个警报。 建议你在第一个 GET 查询中仅包括 `$top`，而不包括 `$skip`。 可使用 `@odata.nextLink` 进行分页。 如果需要使用 `$skip`，它具有 500 个警报的限制。 例如，`/security/alerts?$top=10&$skip=500` 将返回 `200 OK` 响应代码，但 `/security/alerts?$top=10&$skip=501` 将返回 `400 Bad Request` 响应代码。 有关详细信息，请参阅 [Microsoft Graph 安全性 API 错误响应](../resources/security-error-codes.md)。

此限制的一个工作是，将 OData 查询参数与 Microsoft Graph 安全 API 中的 警报实体的 一同使用，将 dateTime 值替换为最后一个 `$filter` `eventDateTime` (`?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` 1500) 警报。 您还可以为 ;例如 `eventDateTime` *，alerts？$filter=eventDateTime **gt** 2018-11-**11** T00：00：00.000Z&eventDateTime **lt** 2018-11-**12** T00：00：00.000Z*

## <a name="see-also"></a>另请参阅

如果你在授权方面遇到问题，请参阅授权和[Microsoft Graph安全 API。](/graph/security-authorization)

