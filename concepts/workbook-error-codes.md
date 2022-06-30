---
title: 工作簿和图表 API 的错误代码
description: 列出并描述在通过 API 发送的请求失败时，Microsoft Graph 中的工作簿和图表 API 返回的错误代码。
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: d51b2da336e5d27177f654dfff25c86adcd0dd79
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555854"
---
# <a name="error-codes-for-workbooks-and-charts-apis"></a>工作簿和图表 API 的错误代码

本文介绍通过这些 API 发送的请求失败时，Microsoft Graph 中的工作簿和图表 API 返回的错误代码。 有关在 Microsoft Graph 中处理来自工作簿和图表 API 的错误响应的详细信息，请参阅 [Microsoft Graph 中 Excel API 的错误处理](workbook-error-handling.md)。 有关 Microsoft Graph 中的错误响应和资源类型的详细信息，请参阅 [Microsoft Graph 错误响应和资源类型](errors.md)。

## <a name="error-codes-and-messages"></a>错误代码和消息

下表列出了当前的错误代码和消息。 该服务可能随时添加新的错误代码。

| 状态代码 | 错误代码            | 错误消息                                                                                                                     |
|:------------|:----------------------|:----------------------------------------------------------------------------------------------------------------------------------|
| 400         | `badRequest`          | 该请求格式有误或不正确。                                                                                            |
| 401         | `unauthorized`        | 调用方未进行身份验证。                                                                                                  |
| 403         | `forbidden`           | 调用方没有执行该操作的权限。                                                                         |
| 404         | `notFound`            | 找不到资源。                                                                                                  |
| 405         | `methodNotAllowed`    | 请求中的 HTTP 方法在资源上不允许。                                                                    |
| 409         | `conflict`            | 当前状态与请求预期的状态的冲突。                                                                        |
| 413         | `payloadTooLarge`     | 请求的大小超出最大限制。                                                                                       |
| 429         | `tooManyRequests`     | 应用或用户已被限制。                                                                                               |
| 500         | `internalServerError` | 处理请求时发生内部服务器错误。                                                                   |
| 501         | `notImplemented`      | 所请求的功能未实现。                                                                                          |
| 502         | `badGateway`          | 服务器遇到临时错误，无法完成请求。                                                     |
| 503         | `serviceUnavailable`  | 服务不可用。 请重试请求。                                                                      |
| 504         | `gatewayTimeout`      | 服务器在充当代理时未收到来自上游服务器的及时响应以完成请求。 |

## <a name="detailed-error-codes"></a>详细的错误代码

下面是应用在嵌套的 **innerError** 对象的第一级中可能会遇到的必需错误代码。 该服务可能随时添加新的错误代码。

- `accessConflict`
- `badRequestUncategorized`
- `conflictUncategorized`
- `forbiddenUncategorized`
- `gatewayTimeoutUncategorized`
- `internalServerErrorUncategorized`
- `invalidSessionAccessConflict`
- `invalidSessionAuthentication`
- `invalidSessionNotFound`
- `invalidSessionReCreatable`
- `invalidSessionRestricted`
- `invalidSessionUnexpected`
- `invalidSessionUnsupportedWorkbook`
- `methodNotAllowedUncategorized`
- `notFoundUncategorized`
- `notImplementedUncategorized`
- `payloadTooLargeUncategorized`
- `serviceUnavailableUncategorized`
- `tooManyRequestsUncategorized`
- `transientFailure`
- `unauthorizedUncategorized`
- `unsupportedWorkbook`

有关嵌套 **innerError** 对象的第一级中的可选错误代码示例，请参阅 [可选的二级错误代码示例](workbook-error-handling.md#optional-second-level-error-code-examples)。

> [!NOTE]
> **innerError** 对象可能以递归方式包含更深的 **innerError** 对象，并包含其他更具体的错误代码。 这些更深入的 **innerError** 代码仅用于诊断目的。

<!-- {
  "type": "#page.annotation",
  "description": "Workbook error code and message",
  "keywords": "error response, error codes, innerError, message, code",
  "section": "documentation",
  "tocPath": ""
} -->

## <a name="see-also"></a>另请参阅

- [使用 Excel REST API](/graph/api/resources/excel)