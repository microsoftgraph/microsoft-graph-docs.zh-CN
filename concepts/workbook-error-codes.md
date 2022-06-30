---
title: 工作簿和图表 API 的错误代码
description: 列出并描述在通过 API 发送的请求失败时，Microsoft Graph 中工作簿和图表 API 返回的错误代码。
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: 88921271f38f9ae8ad440ea40a2733b890e14d83
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444178"
---
# <a name="error-codes-for-workbooks-and-charts-apis"></a>工作簿和图表 API 的错误代码

本文介绍在通过 API 发送的请求失败时，Microsoft Graph 中工作簿和图表 API 返回的错误代码。 有关 Microsoft Graph 中的错误响应和资源类型的详细信息，请参阅 [“错误](/concepts/errors.md)”。 有关在 Microsoft Graph 中处理来自 Excel API 的错误响应的详细信息，请参阅 [错误处理](workbook-error-handling.md)。

## <a name="error-codes-and-messages"></a>错误代码和消息

下表列出了当前的错误代码和消息。 该服务可能随时添加新的错误代码。

| 状态代码 | 错误代码                | 错误消息
|:------------|:--------------------------|:--------------
|400          | **badRequest**            | 该请求格式有误或不正确。
|401          | **未经 授权**          | 调用方未进行身份验证。
|403          | **禁止**             | 调用方没有执行该操作的权限。
|404          | **notFound**              | 找不到资源。
|405          | **methodNotAllowed**      | 请求中的 HTTP 方法在资源上不允许。
|409          | **冲突**              | 当前状态与请求预期的状态的冲突。
|413          | **payloadTooLarge**       | 请求的大小超出最大限制。
|429          | **tooManyRequests**       | 应用或用户已被限制。
|500          | **internalServerError**   | 处理请求时发生内部服务器错误。
|501          | **notImplemented**        | 所请求的功能未实现。
|502          | **badGateway**            | 服务器遇到临时错误，无法完成请求。
|503          | **serviceUnavailable**    | 服务不可用。 请重试请求。
|504          | **gatewayTimeout**        | 服务器在充当代理时未收到来自上游服务器的及时响应以完成请求。

## <a name="detailed-error-codes"></a>详细的错误代码

以下是应用可能在第一级嵌 `innerError` 套对象中遇到的一些其他错误代码。 该服务可能随时添加新的错误代码。

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

> [!NOTE]
> **innerError** 对象可能以递归方式包含更深的 **innerError** 对象，并包含其他更具体的错误代码。 这些更深入的 **innerError** 代码旨在供开发人员阅读。

<!-- {
  "type": "#page.annotation",
  "description": "Workbook error code and message",
  "keywords": "error response, error codes, innerError, message, code",
  "section": "documentation",
  "tocPath": ""
} -->

## <a name="see-also"></a>另请参阅

- [使用 Excel REST API](/graph/api/resources/excel)