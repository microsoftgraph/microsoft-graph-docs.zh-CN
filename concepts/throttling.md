---
title: Microsoft Graph 限制指南
description: 查找在出现大量请求时维护 Microsoft Graph 服务最佳性能的最佳做法。
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: d26976bad505adfb2564e50609ea5d6186148b4e
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671365"
---
# <a name="microsoft-graph-throttling-guidance"></a>Microsoft Graph 限制指南

限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。

根据该方案，执行的限制会有所不同。例如，如果你正在执行大量的写入操作，限制的可能性会比仅执行读取时要高。

> [!NOTE]
> 需要从 Microsoft Graph 提取大量数据的解决方案应使用 [Microsoft Graph Data Connect](data-connect-concept-overview.md) 而不是 Microsoft Graph REST API。 Microsoft Graph Data Connect 允许组织批量提取 Microsoft 365 数据，不受限制。

<!-- markdownlint-disable MD033 -->
<br/>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a>在限制时，会发生什么情况？
<!-- markdownlint-enable MD026 -->

超出限制阈值后，Microsoft Graph 会在一段时间内限制来自该客户端的任何进一步的请求。发生限制时，Microsoft Graph 将返回 HTTP 状态代码 429（请求过多），同时请求失败。在失败的请求的响应标头中返回建议的等待时间。限制行为取决于请求的类型和数量。例如，如果你有大量的请求，则所有请求类型受限。阈值限制根据请求类型而有所不同。因此，你可能会遇到这样一种场景，在场景中，写入被限制，但仍允许读取。

## <a name="common-throttling-scenarios"></a>常见的限制场景

客户端受限的最常见原因包括：

- 来自租户中所有应用程序的请求太多。
- 来自所有租户中特定应用程序的请求太多。

## <a name="sample-response"></a>示例响应

每当超出限制阈值时，Microsoft Graph 都会提供与此类似的响应。

```http
HTTP/1.1 429 Too Many Requests
Content-Type: application/json
Retry-After: 10

{
  "error": {
    "code": "TooManyRequests",
    "innerError": {
      "code": "429",
      "date": "2020-08-18T12:51:51",
      "message": "Please retry after",
      "request-id": "94fb3b52-452a-4535-a601-69e0a90e3aa2",
      "status": "429"
    },
    "message": "Please retry again later."
  }
}
```

## <a name="best-practices-to-handle-throttling"></a>处理限制的最佳实践

以下是处理限制的最佳做法：

- 减少每个请求的操作数量。
- 减少调用频率。
- 不要立即重试，因为所有请求都会计入使用限制。

进行错误处理时，使用 HTTP 错误代码 429 检测限制。失败的响应包括 `Retry-After` 响应标头。使用 `Retry-After` 延迟回退请求是从限制中恢复的最快速的方式，因为 Microsoft Graph 会在客户端受限时继续记录资源使用状况。

1. 等待 `Retry-After` 标头中指定的秒数。
2. 请重试请求。
3. 如果请求再次失败，并显示 429 错误代码，则表示你仍然受限。继续使用建议的 `Retry-After` 延迟并重试请求直到成功。

除非另有说明，否则[服务特定限制](throttling-limits.md)部分中所述的所有资源和 API 均提供 `Retry-After` 标头。

有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式](/azure/architecture/patterns/throttling)。

> [!NOTE]
> 如果响应未提供 `Retry-After` 标头，我们建议实施指数退避重试策略。 构建大型应用程序时，还可以实现[更高级的模式](/azure/architecture/patterns/category/resiliency)。
>
> Microsoft Graph SDK 已实施依赖于 `Retry-After` 标头或默认为指数退避重试策略的处理程序。

## <a name="best-practices-to-avoid-throttling"></a>避免限制的最佳做法

如持续轮询资源以检查更新以及定期扫描资源集合以检查新资源或已删除资源之类的编程模式，更有可能导致应用程序受到限制并降低整体性能。如果可用，你应该改为使用[更改跟踪](delta-query-overview.md)和[更改通知](webhooks.md)。

>[!NOTE]
>[大规模发现文件和检测更改的最佳做法](/onedrive/developer/rest-api/concepts/scan-guidance)详细介绍最佳做法。

## <a name="throttling-and-batching"></a>限制和批处理

[JSON 批处理](./json-batching.md)使你能够通过将多个请求合并为单个 JSON 对象来优化应用程序。 批次中的请求将根据限制进行单独评估，如果任何请求超出限制，则它将失败，并出现 `status` `429` 以及类似于上述内容的错误。 批次本身失败，状态代码为 `424`（失败的相关性）。 多个请求可能会在单个批次中受到限制。 应使用 JSON 内容的 `retry-after` 响应标头中提供的值，尝试批次中每个失败的请求。 你可以在最长 `retry-after` 值之后重试新批次中所有失败的请求。

如果在受限制请求未经批处理时，SDK 自动重试这些请求，则不会自动重试属于批次的受限制请求。

## <a name="next-steps"></a>后续步骤

确定适用于每个 Microsoft Graph 资源的 [节流限制](throttling-limits.md)。