---
title: Microsoft Graph 中的工作簿和图表 Api 的错误代码
description: 列出并描述 Microsoft Graph 中的工作簿和图表 Api 的错误代码和消息。
author: grangeryy
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8c975507b826f305ed3a0c994e5aa86384095e94
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643910"
---
# <a name="error-codes-for-workbooks-and-charts-apis-in-microsoft-graph"></a>Microsoft Graph 中的工作簿和图表 Api 的错误代码

本文介绍当通过 API 发送的请求失败时，由 Microsoft Graph 中的工作簿和图表 Api 返回的错误代码。 有关 Microsoft Graph 中的错误响应和资源类型的更多详细信息，请参阅[错误](/concepts/errors.md)。

## <a name="error-code"></a>错误代码

下表列出了当前错误代码和消息。 服务可能会在任何时候添加新的错误代码。

| 代码                      | 消息
|:--------------------------|:--------------
| **accessDenied**      | 调用方没有执行该操作的权限。
| **冲突**          | 当前状态与请求预期的状态的冲突。
| **gatewayTimeout**        | 作为代理的服务器不会及时收到来自上游服务器的响应，因此无法完成该请求。
| **internalServerError**            | 处理请求时出现内部服务器错误。
| **invalidRequest**          | 该请求格式有误或不正确。
| **methodNotAllowed**        |请求中的 HTTP 方法在资源上不允许。
| **notImplemented**          | 所请求的功能未实现。
| **requestSizeExceeded**       | 请求的大小超出最大限制。
| **resourceNotFound**          | 找不到资源。
| **serviceUnavailable**      | 服务不可用。 请再次尝试你的请求。
| **tooManyRequests**     | 应用或用户已被限制。
| **unauthenticated**  | 调用方未进行身份验证。

## <a name="detailed-error-code"></a>详细错误代码
以下是你的应用可能会在第一级嵌套对象中遇到的一些其他错误 `innerError` 。 服务可能会在任何时候添加新的错误代码。

| 代码                               | 消息
|:-----------------------------------|:----------------------------------------------------------
| **accessConflict**   |请求失败，因为与正在访问工作簿的其他客户端发生冲突。
| **accessDenied**         | 无法执行所请求的操作。
| **badRequestUncategorized**               | 该请求格式有误或不正确。
| **conflictUncategorized**                   | 当前状态与请求预期的状态的冲突。
| **filteredRangeConflict**                   | 操作失败，因为它与筛选的区域冲突。
| **forbiddenUncategorized**                    | 不允许该请求。
| **gatewayTimeoutUncategorized**         | 服务无法在时间限制内完成请求。
| **generalException**         | 处理请求时出现内部错误。
| **insertDeleteConflict**         | 尝试的插入或删除操作导致冲突。
| **internalServerErrorUncategorized**       | 发生未指定错误。
| **invalidArgument**         | 自变量无效、缺少或格式不正确。
| **invalidReference**         | 此引用对于当前操作无效。
| **invalidSessionAccessConflict**             | 由于与正在访问工作簿的其他客户端发生冲突，请求中指定的会话无效。
| **invalidSessionAuthentication**         | 由于身份验证错误，请求中指定的会话无效。
| **invalidSessionNotFound**         | 请求中指定的会话无效，因为找不到工作簿。
| **invalidSessionReCreatable**             | 请求中指定的会话不存在或因暂时性错误而无效。
| **invalidSessionRestricted**          | 由于服务配置或限制，在请求中指定的会话无效。
| **invalidSessionUnexpected**                | 由于意外问题，请求中指定的会话无效。
| **invalidSessionUnsupportedWorkbook**              | 请求中指定的会话无效，因为工作簿包含不受支持的功能或超出了大小限制。
| **itemAlreadyExists**         | 所创建的资源已存在。
| **itemNotFound**         | 所请求的资源不存在。
| **methodNotAllowedUncategorized**              | 该资源上不允许请求中指定的 HTTP 方法。
| **nonBlankCellOffSheet**         | 无法插入新单元格，因为它会将非空单元格推送到工作表的末尾。
| **notFoundUncategorized**             | 找不到请求的资源。
| **notImplementedUncategorized**            | 当前未实现请求的功能。
| **payloadTooLargeUncategorized**              | 请求负载超过了大小限制。
| **rangeExceedsLimit**         | 范围中的单元格计数已超过支持的最大数量。
| **requestAborted**         | 请求在运行时已中止。
| **serviceUnavailableUncategorized**      | 服务暂时不可用或已重载。 请再次尝试你的请求。
| **tooManyRequestsUncategorized**             | 已限制客户端应用程序或用户。 请再次尝试你的请求。
| **transientFailure**           | 由于暂时性错误，请求失败。 请再次尝试你的请求。
| **unauthorizedUncategorized**         | 资源所需的身份验证信息缺少或无效。
| **unsupportedOperation**         | 不支持正在尝试的操作。
| **unsupportedWorkbook**         | 请求失败。 工作簿包含不受支持的功能，或超出大小限制。

>**注意：****InnerError**对象可能以递归方式包含更深的**innerError**对象，具有更多的更具体的错误代码。 为使开发人员能够阅读这些更深层的**innerError**代码 intented。
<!-- {
  "type": "#page.annotation",
  "description": "Workbook error code and message",
  "keywords": "error response, error codes, innerError, message, code",
  "section": "documentation",
  "tocPath": ""
} -->
