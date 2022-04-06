---
title: Microsoft 工作簿和图表 API 的错误Graph
description: 列出并描述 Microsoft 工作簿和图表 API 的错误代码和Graph。
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: 981be39ad78af98d131e4b38a9de49e688e27551
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672404"
---
# <a name="error-codes-for-workbooks-and-charts-apis-in-microsoft-graph"></a>Microsoft 工作簿和图表 API 的错误Graph

本文介绍当通过 API 发送的请求失败时，Microsoft 工作簿和图表 API Graph返回的错误代码。 有关 Microsoft 错误响应和资源类型的详细信息，[Graph错误。](/concepts/errors.md) 有关处理来自 Microsoft Excel API 的错误Graph，请参阅[错误处理](workbook-error-handling.md)。

## <a name="error-code"></a>错误代码

下表列出了当前的错误代码和消息。 该服务可能随时添加新的错误代码。 

| 状态代码               | 错误代码                       | 错误消息
|:--------------------------|:--------------------------|:--------------
|400    | **badRequest**          | 该请求格式有误或不正确。
|401    | **未授权**  | 调用方未进行身份验证。
|403    | **禁止**      | 调用方没有执行该操作的权限。
|404    | **notFound**          | 找不到资源。
|405    | **methodNotAllowed**        | 请求中的 HTTP 方法在资源上不允许。
|409    | **conflict**          | 当前状态与请求预期的状态的冲突。
|413    | **payloadTooLarge**       | 请求的大小超出最大限制。
|429    | **tooManyRequests**     | 应用或用户已被限制。
|500    | **internalServerError**            | 处理请求时出现内部服务器错误。
|501    | **notImplemented**          | 所请求的功能未实现。
|502    | **badGateway**          | 服务器遇到临时错误，无法完成您的请求。
|503    | **serviceUnavailable**      | 服务不可用。 请再次尝试你的请求。
|504    | **gatewayTimeout**        | 服务器在充当代理时，未收到来自上游服务器的及时响应以完成请求。

## <a name="detailed-error-code"></a>详细错误代码
下面是你的应用在嵌套对象的第一级中可能会遇到的一些其他错误 `innerError` 代码。 该服务可能随时添加新的错误代码。

- accessConflict
- accessDenied
- badRequestUncategorized
- conflictUncategorized
- filteredRangeConflict
- forbiddenUncategorized
- gatewayTimeoutUncategorized
- generalException
- insertDeleteConflict
- internalServerErrorUncategorized
- invalidArgument
- invalidReference
- invalidSessionAccessConflict
- invalidSessionAuthentication
- invalidSessionNotFound
- invalidSessionReCreatable
- invalidSessionRestricted
- invalidSessionUnexpected
- invalidSessionUnsupportedWorkbook
- itemAlreadyExists
- itemNotFound
- methodNotAllowed
- methodNotAllowedUncategorized
- nonBlankCellOffSheet
- notFoundUncategorized
- notImplementedUncategorized
- payloadTooLargeUncategorized
- rangeExceedsLimit
- requestAborted
- serviceUnavailableUncategorized
- tooManyRequestsUncategorized
- transientFailure
- unauthorizedUncategorized
- unsupportedOperation
- unsupportedWorkbook

>**注意：****innerError** 对象可能以递归方法包含具有更多更具体的错误代码的更深层次的 **innerError** 对象。 这些更 **深层次的 innerError** 代码是让开发人员阅读的。
<!-- {
  "type": "#page.annotation",
  "description": "Workbook error code and message",
  "keywords": "error response, error codes, innerError, message, code",
  "section": "documentation",
  "tocPath": ""
} -->
