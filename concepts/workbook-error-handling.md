---
title: Microsoft Graph 中 Excel API 的错误处理
description: Microsoft Graph 中 Excel API 的错误处理说明
author: grangeryy
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5d5a420b4968b0a944ac192de5654692678663c8
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50293076"
---
# <a name="error-handling-for-excel-apis-in-microsoft-graph"></a>Microsoft Graph 中 Excel API 的错误处理

本文提供有关处理通过 API 发送的请求失败时 Microsoft Graph 中的 Excel API 返回的错误的一般说明和建议。

## <a name="types-of-error-responses"></a>错误响应的类型

Microsoft Graph 中的 Excel API 返回两种类型的错误。 一种是常规错误响应，如下所示。

```http
HTTP/1.1 <HTTP status code>
Content-type: application/json

{
  "error": <Error object>
}
```

第二个来自长时间运行的操作模式，该模式可在响应正文中返回 HTTP 状态代码和操作 `200 OK` `failed` 状态，如以下示例所示。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "status": "failed",
  "error": <Error object>
}
```

对于这两种错误响应，错误对象具有以下结构。

>**注意：** 错误响应遵循 [OData v4 规范](https://docs.oasis-open.org/odata/odata-json-format/v4.0/os/odata-json-format-v4.0-os.html#_Toc372793091) 中有关错误响应的定义。

```json
{
  "code": "string",
  "message": "string",
  "innerError": { "@odata.type": "odata.error" }
}
```

`innerError` 对象可能以递归方式包含更多 `innerError` 对象，其中具有其他更多具体的错误代码。 例如，错误对象可能包含第二级错误代码和消息中更详细的错误信息，如下所示。

```json
{
  "code": "Top-level error code",
  "message": "Top-level error message",
  "innerError": {
    "code": "Second-level error code",
    "message": "Second-level error message",
    "innerError": { "@odata.type": "odata.error" }
  }
}
```

## <a name="steps-to-handle-error-responses"></a>处理错误响应的步骤

Microsoft Graph 客户端可以使用以下步骤来处理 Excel API 发生的错误。

### <a name="1-determine-whether-it-is-a-long-running-operation-error"></a>1. 确定它是否是长时间运行的操作错误

在处理错误之前，第一步是确定错误响应来自长时间运行的操作模式还是常规模式。 长时间运行的操作错误将在响应正文中返回 `200 OK` HTTP `failed` 状态代码和操作状态。 常规错误响应将返回相应的 HTTP 错误状态代码。 

### <a name="2-parse-second-level-error-code"></a>2. 分析二级错误代码

对于长时间运行的操作模式和常规模式，我们建议您首先按照说明处理二级错误。 错误代码不区分大小写。 下表列出了某些错误的说明。 该服务可能随时添加新的错误代码。

| 代码                               | 说明
|:-----------------------------------|:---------------------------------------------
| **accessConflict**   | 失败的请求与其他访问工作簿的客户端冲突 (例如，另一个客户端锁定工作簿进行编辑) 。 在解决冲突之前，Microsoft Graph 客户端不会重新发送失败的请求。 最终用户可以选择使用 Excel Online 手动执行相同的操作，获取有关冲突的更多详细信息。
| **accessDenied**   | 不能执行请求的操作 (例如，对锁定的单元格执行) 。 Microsoft Graph 客户端不应重新发送失败的请求。
| **badRequestUncategorized**    | 在失败的请求中发现未指定的错误。 Microsoft Graph 客户端不应重新发送失败的请求。
| **conflictUncategorized**                   | 失败的请求与某些服务器状态冲突。 在解决冲突之前，Microsoft Graph 客户端不会重新发送失败的请求。 最终用户可以选择使用 Excel Online 手动执行相同的操作，获取有关冲突的更多详细信息。
| **filteredRangeConflict**                   | 操作失败，因为它与筛选出的范围冲突。 Microsoft Graph 客户端不应重新发送失败的请求。
| **forbiddenUncategorized**                    | 不允许失败的请求。 Microsoft Graph 客户端不应重新发送失败的请求。 最终用户可以选择使用 Excel Online 手动执行相同的操作，获取有关限制的更多详细信息。
| **gatewayTimeoutUncategorized**         | 服务无法在此时间限制内完成请求。
| **generalException**         | 处理请求时出现内部错误。 Microsoft Graph 客户端不应重新发送失败的请求。
| **insertDeleteConflict**         | 尝试的插入或删除操作导致冲突。 Microsoft Graph 客户端不应重新发送失败的请求。
| **internalServerErrorUncategorized**       | 发生未指定错误。 Microsoft Graph 客户端不应重新发送失败的请求。 如果在失败的请求中指定了会话，则不需要进一步访问会话。
| **invalidArgument**         | 自变量无效、缺少或格式不正确。 Microsoft Graph 客户端不应重新发送失败的请求。
| **invalidReference**         | 此引用对于当前操作无效。 Microsoft Graph 客户端不应重新发送失败的请求。
| **invalidSessionAccessConflict**             | 由于与其他访问工作簿的客户端发生冲突，请求中指定的会话无效 (例如，另一个客户端锁定了工作簿进行编辑) 。 不应进一步访问失败请求中指定的会话。 在解决冲突之前，不需要重新创建具有相同 **createSession** 请求的会话。 使用不同的 **createSession** 请求重新创建会话可能会成功，也可能失败。 最终用户可以选择使用 Excel Online 手动执行相同的操作，获取有关冲突的更多详细信息。
| **invalidSessionAuthentication**         | 由于身份验证错误，请求中指定的会话无效。 不应进一步访问失败请求中指定的会话。 在提供适当的身份验证信息之前，不应使用相同的 **createSession** 请求重新创建会话。
| **invalidSessionNotFound**         | 请求中指定的会话无效，因为找不到工作簿。 不应进一步访问失败请求中指定的会话。 不需要使用相同的 **createSession** 请求重新创建会话。
| **invalidSessionReCreatable**             | 请求中指定的会话不存在或由于暂时性错误而无效。 Microsoft Graph 客户端可以尝试重新创建会话并恢复工作。 不应进一步访问失败请求中指定的会话。
| **invalidSessionRestricted**          | 由于服务配置或限制，请求中指定的会话无效。 不应进一步访问失败请求中指定的会话。 在阻止请求的限制或配置更改之前，不需要重新创建具有相同 **createSession** 请求的会话。 使用不同的 **createSession** 请求重新创建会话可能会成功，也可能失败。 最终用户可以选择使用 Excel Online 手动执行相同的操作，获取限制的更多详细信息。
| **invalidSessionUnexpected**                | 由于意外问题，请求中指定的会话无效。 不应进一步访问失败请求中指定的会话。 不需要使用相同的 **createSession** 请求重新创建会话。 使用不同的 **createSession** 请求重新创建会话可能会成功，也可能失败。
| **invalidSessionUnsupportedWorkbook**              | 请求中指定的会话无效，因为工作簿包含不受支持的功能或超出大小限制。 通常，不受支持的因素由访问工作簿的另一个客户端引入。 不应进一步访问失败请求中指定的会话。 在删除不受支持的因素之前，不需要重新创建具有相同 **createSession** 请求的会话。 使用不同的 createSession 请求重新创建会话可能会成功，也可能失败。 最终用户可以选择使用 Excel Online 手动执行相同的操作，获取不受支持因素的更多详细信息，也可以选择使用 Excel 桌面（其中工作簿可能受支持）。
| **itemAlreadyExists**         | 所创建的资源已存在。 Microsoft Graph 客户端不应重新发送失败的请求。
| **itemNotFound**         | 所请求的资源不存在。 Microsoft Graph 客户端不应重新发送失败的请求。
| **methodNotAllowed**         | 资源上不允许使用请求中指定的 HTTP 方法。 Microsoft Graph 客户端不应重新发送失败的请求。
| **methodNotAllowedUncategorized**              | 资源上不允许使用请求中指定的 HTTP 方法。 Microsoft Graph 客户端不应重新发送失败的请求。
| **nonBlankCellOffSheet**         | 无法插入新单元格，因为它会将非空单元格推送到工作表的末尾。 Microsoft Graph 客户端不应重新发送失败的请求。
| **notFoundUncategorized**             | 找不到请求的资源。 Microsoft Graph 客户端不应重新发送失败的请求。
| **notImplementedUncategorized**            | 请求的功能当前未实现。 Microsoft Graph 客户端不应重新发送失败的请求。
| **payloadTooLargeUncategorized**              | 请求有效负载超过大小限制。 Microsoft Graph 客户端不应重新发送失败的请求。
| **rangeExceedsLimit**         | 范围中的单元格计数已超出支持的最大数。 Microsoft Graph 客户端可以尝试发送范围较小的请求。
| **requestAborted**         | 请求在运行期间中止，这通常是由工作簿中函数的长时间计算导致的。 Microsoft Graph 客户端不应重新发送失败的请求。
| **serviceUnavailableUncategorized**      | 服务暂时不可用或过载。 Microsoft Graph 客户端不会重新发送失败的请求，直到指定的关闭持续时间过去。
| **tooManyRequestsUncategorized**             | 失败的请求超出了某些频率限制。 Microsoft Graph 客户端不会重新发送失败的请求，直到指定的关闭持续时间过去。
| **transientFailure**           | 由于暂时性错误，请求失败。 Microsoft Graph 客户端不会重新发送失败的请求，直到指定的关闭持续时间过去。
| **unauthorizedUncategorized**         | 资源所需的身份验证信息缺失或无效。 Microsoft Graph 客户端不应重新发送失败的请求。
| **unsupportedOperation**         | 不支持正在尝试的操作。 Microsoft Graph 客户端不应重新发送失败的请求。
| **unsupportedWorkbook**         | 请求失败。 工作簿包含不受支持的功能或超出大小限制。 在删除不受支持的因素之前，Microsoft Graph 客户端不会重新发送失败的请求。

>**注意：** 对于常规模式，失败的请求定义为与响应对应的请求。 对于长时间运行的操作模式，失败的请求是触发失败操作的请求。

### <a name="3-parse-the-top-level-error-code"></a>3. 分析顶级错误代码

如果找不到"详细错误代码"主题中列出的二级错误代码，我们建议您[](workbook-error-codes.md#detailed-error-code)按照针对顶级错误提供的说明操作。 顶级错误代码绑定到状态代码，你可以根据相应的状态代码采取措施。 有关顶级错误代码和消息的详细信息，请参阅 [错误代码](workbook-error-codes.md#error-code)。

### <a name="4-parse-the-status-code"></a>4. 分析状态代码

如果您遇到的错误代码不在二级列表或顶级列表中，我们建议您根据 HTTP 状态代码采取措施。

### <a name="5-error-recovery-cooldown"></a>5. 错误恢复关闭

对于常规模式中的一些响应，恢复冷持续时间（以秒计）可能通过标头 `Retry-After` 提供。 当存在恢复冷淡持续时间时，Microsoft Graph 客户端不会在指定的持续时间过去之前发送任何后续请求。

## <a name="special-case-handling"></a>特殊情况处理

对于[](excel-manage-sessions.md#request-types)会话请求，如果遇到错误或错误，当二级错误代码在详细错误代码中列出时，请分析二级代码并按照相应的说明操作;否则，我们将重新确认您直接重新创建会话。 `502/badGateway` `503/serviceUnavailable` [](workbook-error-codes.md#detailed-error-code)
<!-- {
  "type": "#page.annotation",
  "description": "Error handling in Excel Graph.",
  "keywords": "error response, error object, error codes, innerError, error handling",
  "section": "documentation",
  "tocPath": ""
} -->
