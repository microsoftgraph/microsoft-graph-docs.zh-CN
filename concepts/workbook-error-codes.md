---
title: Microsoft 工作簿和图表 API 的错误代码Graph
description: 列出并描述 Microsoft 工作簿和图表 API 的错误代码和Graph。
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: cadcbb4ad64d6d441c09e9deb331dfe28edf5d18
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143445"
---
# <a name="error-codes-for-workbooks-and-charts-apis-in-microsoft-graph"></a>Microsoft 工作簿和图表 API 的错误代码Graph

本文介绍当通过 API 发送的请求失败时，Microsoft 工作簿和图表 API Graph返回的错误代码。 有关 Microsoft 错误响应和资源类型的详细信息，Graph错误[。](/concepts/errors.md)

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
下面是你的应用在嵌套对象的第一级中可能会遇到的一些其他 `innerError` 错误。 该服务可能随时添加新的错误代码。

| 代码                               | 消息
|:-----------------------------------|:----------------------------------------------------------
| **accessConflict**   |由于与正在访问工作簿的其他客户端发生冲突，请求失败。
| **accessDenied**         | 无法执行所请求的操作。
| **badRequestUncategorized**               | 该请求格式有误或不正确。
| **conflictUncategorized**                   | 当前状态与请求预期的状态的冲突。
| **filteredRangeConflict**                   | 操作失败，因为它与筛选出的范围冲突。
| **forbiddenUncategorized**                    | 不允许该请求。
| **gatewayTimeoutUncategorized**         | 服务未能在时间限制内完成请求。
| **generalException**         | 处理请求时出现内部错误。
| **insertDeleteConflict**         | 尝试的插入或删除操作导致冲突。
| **internalServerErrorUncategorized**       | 发生未指定错误。
| **invalidArgument**         | 自变量无效、缺少或格式不正确。
| **invalidReference**         | 此引用对于当前操作无效。
| **invalidSessionAccessConflict**             | 由于与访问工作簿的其他客户端冲突，请求中指定的会话无效。
| **invalidSessionAuthentication**         | 由于身份验证错误，请求中指定的会话无效。
| **invalidSessionNotFound**         | 请求中指定的会话无效，因为找不到工作簿。
| **invalidSessionReCreatable**             | 请求中指定的会话不存在或由于暂时性错误而无效。
| **invalidSessionRestricted**          | 由于服务配置或限制，请求中指定的会话无效。
| **invalidSessionUnexpected**                | 由于意外问题，请求中指定的会话无效。
| **invalidSessionUnsupportedWorkbook**              | 请求中指定的会话无效，因为工作簿包含不受支持的功能或超出大小限制。
| **itemAlreadyExists**         | 所创建的资源已存在。
| **itemNotFound**         | 所请求的资源不存在。
| **methodNotAllowed**              | 资源上不允许使用请求中指定的 HTTP 方法。
| **methodNotAllowedUncategorized**              | 资源上不允许使用请求中指定的 HTTP 方法。
| **nonBlankCellOffSheet**         | 无法插入新单元格，因为它将非空单元格推送到工作表末尾。
| **notFoundUncategorized**             | 找不到请求的资源。
| **notImplementedUncategorized**            | 请求的功能当前未实现。
| **payloadTooLargeUncategorized**              | 请求有效负载超出大小限制。
| **rangeExceedsLimit**         | 范围中的单元格计数已超出支持的最大数。
| **requestAborted**         | 请求在运行时已中止。
| **serviceUnavailableUncategorized**      | 服务暂时不可用或过载。 请再次尝试你的请求。
| **tooManyRequestsUncategorized**             | 客户端应用或用户已被限制。 请再次尝试你的请求。
| **transientFailure**           | 由于暂时性错误，请求失败。 请再次尝试你的请求。
| **unauthorizedUncategorized**         | 资源的必需身份验证信息缺失或无效。
| **unsupportedOperation**         | 不支持正在尝试的操作。
| **unsupportedWorkbook**         | 请求失败。 工作簿包含不受支持的功能或超出大小限制。

>**注意：****innerError** 对象可能以递归方法包含具有更多更具体的错误代码的更深层次的 **innerError** 对象。 这些更 **深层次的 innerError** 代码是让开发人员阅读的。
<!-- {
  "type": "#page.annotation",
  "description": "Workbook error code and message",
  "keywords": "error response, error codes, innerError, message, code",
  "section": "documentation",
  "tocPath": ""
} -->
