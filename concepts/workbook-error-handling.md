---
title: Microsoft Graph 中的 Excel Api 的错误处理
description: Microsoft Graph 中的 Excel Api 的错误处理说明
author: grangeryy
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 82bbcf6c93146c66aa76d01aa3d111f515a97b61
ms.sourcegitcommit: b6ca83070b6f015c09de215a82cf2b581181c33e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2020
ms.locfileid: "47367220"
---
# <a name="error-handling-for-excel-apis-in-microsoft-graph"></a>Microsoft Graph 中的 Excel Api 的错误处理

本文提供了有关处理通过 API 发送的请求失败时 Microsoft Graph 中的 Excel Api 返回的错误的一般说明和建议。

## <a name="types-of-error-responses"></a>错误响应的类型

Microsoft Graph 中的 Excel Api 返回两种类型的错误。 一个是常规的错误响应，如下所示。

```http
HTTP/1.1 <HTTP status code>
Content-type: application/json

{
  "error": <Error object>
}
```

第二个是来自长时间运行的操作模式，它可以 `200 OK` 在响应正文中返回 HTTP 状态代码和 `failed` 操作状态，如下面的示例所示。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "status": "failed",
  "error": <Error object>
}
```

对于这两个错误响应，error 对象都具有以下结构。

>**注意：** 错误响应遵循 [OData v4](https://docs.oasis-open.org/odata/odata-json-format/v4.0/os/odata-json-format-v4.0-os.html#_Toc372793091) 规范中有关错误响应的定义。

```json
{
  "code": "string",
  "message": "string",
  "innerError": { "@odata.type": "odata.error" }
}
```

`innerError` 对象可能以递归方式包含更多 `innerError` 对象，其中具有其他更多具体的错误代码。 例如，error 对象可能在第二级错误代码和消息中包含更详细的错误信息，如下所示。

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

Microsoft Graph 客户端可以使用以下步骤来处理 Excel Api 中发生的错误。

### <a name="1-determine-whether-it-is-a-long-running-operation-error"></a>1. 确定它是否为长时间运行的操作错误

在处理错误之前，第一步是确定错误响应是否来自长时间运行的操作模式或常规模式。 长时间运行的操作错误将 `200 OK` 在响应正文中返回 HTTP 状态代码和 `failed` 操作状态。 常规错误响应将返回相应的 HTTP 错误状态代码。 

### <a name="2-parse-second-level-error-code"></a>2. 分析第二级错误代码

对于长时间运行的操作模式和常规模式，我们建议您首先遵循第二级错误的说明。 错误代码不区分大小写。 下表列出了一些错误的说明。 服务可能会在任何时候添加新的错误代码。

| 代码                               | 说明
|:-----------------------------------|:---------------------------------------------
| **accessConflict**   | 失败的请求与访问工作簿的其他客户端冲突 (例如，另一个客户端锁定了工作簿以进行编辑) 。 在解决冲突之前，Microsoft Graph 客户端不应重新发送失败的请求。 最终用户 xN 选择手动执行与 Excel Online 相同的操作，以获取有关冲突的更多详细信息。
| **accessDenied**   | 您无法执行请求的操作 (例如，对锁定的单元格) 执行更改。 Microsoft Graph 客户端不应重新发送失败的请求。
| **badRequestUncategorized**    | 在失败的请求中发现未指定的错误。 Microsoft Graph 客户端不应重新发送失败的请求。
| **conflictUncategorized**                   | 失败的请求与特定的服务器状态冲突。 在解决冲突之前，Microsoft Graph 客户端不应重新发送失败的请求。 最终用户可以选择使用 Excel Online 手动执行相同的操作，以获取有关冲突的更多详细信息。
| **filteredRangeConflict**                   | 操作失败，因为它与筛选的区域冲突。 Microsoft Graph 客户端不应重新发送失败的请求。
| **forbiddenUncategorized**                    | 不允许使用失败的请求。 Microsoft Graph 客户端不应重新发送失败的请求。 最终用户可以选择使用 Excel Online 手动执行相同的操作，以获取有关限制的更多详细信息。
| **gatewayTimeoutUncategorized**         | 服务无法在时间限制内完成请求。 Microsoft Graph 客户端在指定的 cooldown 持续时间通过之前，不应重新发送失败的请求。
| **generalException**         | 处理请求时出现内部错误。 Microsoft Graph 客户端不应重新发送失败的请求。
| **insertDeleteConflict**         | 尝试的插入或删除操作导致冲突。 Microsoft Graph 客户端不应重新发送失败的请求。
| **internalServerErrorUncategorized**       | 发生未指定错误。 Microsoft Graph 客户端不应重新发送失败的请求。 如果在失败请求中指定会话，则不需要对会话进行进一步的访问。
| **invalidArgument**         | 自变量无效、缺少或格式不正确。 Microsoft Graph 客户端不应重新发送失败的请求。
| **invalidReference**         | 此引用对于当前操作无效。 Microsoft Graph 客户端不应重新发送失败的请求。
| **invalidSessionAccessConflict**             | 由于与正在访问工作簿的其他客户端发生冲突，请求中指定的会话无效 (例如，另一个客户端已锁定工作簿以进行编辑) 。 对失败的请求中指定的会话的进一步访问不是预期的。 在解决冲突之前，不应在 **createSession** 请求中重新创建会话。 在不同的 **createSession** 请求中重新创建会话可能会或可能不会成功。 最终用户可以选择使用 Excel Online 手动执行相同的操作，以获取有关冲突的更多详细信息。
| **invalidSessionAuthentication**         | 由于身份验证错误，请求中指定的会话无效。 对失败的请求中指定的会话的进一步访问不是预期的。 在提供适当的身份验证信息之前，不应使用相同的 **createSession** 请求重新创建会话。
| **invalidSessionNotFound**         | 请求中指定的会话无效，因为找不到工作簿。 对失败的请求中指定的会话的进一步访问不是预期的。 不应使用相同的 **createSession** 请求重新创建会话。
| **invalidSessionReCreatable**             | 请求中指定的会话不存在或因暂时性错误而无效。 Microsoft Graph 客户端可以尝试重新创建会话并恢复工作。 对失败的请求中指定的会话的进一步访问不是预期的。
| **invalidSessionRestricted**          | 由于服务配置或限制，在请求中指定的会话无效。 对失败的请求中指定的会话的进一步访问不是预期的。 在阻止请求的限制或配置发生更改之前，不应使用相同的 **createSession** 请求重新创建会话。 在不同的 **createSession** 请求中重新创建会话可能会或可能不会成功。 最终用户可以选择使用 Excel Online 手动执行相同的操作，以获取限制的更多详细信息。
| **invalidSessionUnexpected**                | 由于意外问题，请求中指定的会话无效。 对失败的请求中指定的会话的进一步访问不是预期的。 不应使用相同的 **createSession** 请求重新创建会话。 在不同的 **createSession** 请求中重新创建会话可能会或可能不会成功。
| **invalidSessionUnsupportedWorkbook**              | 请求中指定的会话无效，因为工作簿包含不受支持的功能或超出了大小限制。 通常情况下，其他访问工作簿的客户端会引入不受支持的因素。 对失败的请求中指定的会话的进一步访问不是预期的。 在删除不受支持的因素之前，不应使用相同的 **createSession** 请求重新创建会话。 在不同的 createSession 请求中重新创建会话可能会或可能不会成功。 最终用户可以选择使用 Excel Online 手动执行相同的操作，以获取不受支持的因素的更多详细信息，或使用工作簿可能受支持的 Excel 桌面。
| **itemAlreadyExists**         | 所创建的资源已存在。 Microsoft Graph 客户端不应重新发送失败的请求。
| **itemNotFound**         | 所请求的资源不存在。 Microsoft Graph 客户端不应重新发送失败的请求。
| **methodNotAllowed**         | 该资源上不允许请求中指定的 HTTP 方法。 Microsoft Graph 客户端不应重新发送失败的请求。
| **methodNotAllowedUncategorized**              | 该资源上不允许请求中指定的 HTTP 方法。 Microsoft Graph 客户端不应重新发送失败的请求。
| **nonBlankCellOffSheet**         | 无法插入新单元格，因为它会将非空单元格推送到工作表的末尾。 Microsoft Graph 客户端不应重新发送失败的请求。
| **notFoundUncategorized**             | 找不到请求的资源。 Microsoft Graph 客户端不应重新发送失败的请求。
| **notImplementedUncategorized**            | 当前未实现请求的功能。 Microsoft Graph 客户端不应重新发送失败的请求。
| **payloadTooLargeUncategorized**              | 请求负载超过了大小限制。 Microsoft Graph 客户端不应重新发送失败的请求。
| **rangeExceedsLimit**         | 范围中的单元格计数已超过支持的最大数量。 Microsoft Graph 客户端可以尝试发送较小范围大小的请求。
| **requestAborted**         | 请求在运行时被中止，这通常是由工作簿中的函数计算长时间而引起的。 Microsoft Graph 客户端不应重新发送失败的请求。
| **serviceUnavailableUncategorized**      | 服务暂时不可用或已重载。 Microsoft Graph 客户端在指定的 cooldown 持续时间通过之前，不应重新发送失败的请求。
| **tooManyRequestsUncategorized**             | 失败的请求超出了特定频率限制。 Microsoft Graph 客户端在指定的 cooldown 持续时间通过之前，不应重新发送失败的请求。
| **transientFailure**           | 由于暂时性错误，请求失败。 Microsoft Graph 客户端在指定的 cooldown 持续时间通过之前，不应重新发送失败的请求。
| **unauthorizedUncategorized**         | 资源所需的身份验证信息缺少或无效。 Microsoft Graph 客户端不应重新发送失败的请求。
| **unsupportedOperation**         | 不支持正在尝试的操作。 Microsoft Graph 客户端不应重新发送失败的请求。
| **unsupportedWorkbook**         | 请求失败。 工作簿包含不受支持的功能，或超出大小限制。 Microsoft Graph 客户端不应重新发送失败的请求，直到删除不受支持的因素。

>**注意：** 对于常规模式，失败的请求被定义为与响应对应的请求。 对于长时间运行的操作模式，失败的请求是触发失败操作的请求。

### <a name="3-parse-the-top-level-error-code"></a>3. 分析顶级错误代码

如果在 [错误代码](workbook-error-codes.md#error-code) 主题中找不到列出的二级错误代码，我们建议您按照为顶级错误（绑定到状态代码）提供的说明操作。 有关顶级错误代码和消息的详细信息，请参阅 [详细错误代码](workbook-error-codes.md#detailed-error-code)。

### <a name="4-parse-the-status-code"></a>4. 分析状态代码

如果您遇到的错误代码不在第二级列表或顶级列表中，我们建议您根据 HTTP 状态代码执行操作。

### <a name="5-error-recovery-cooldown"></a>5. 错误恢复 cooldown

对于常规模式中的某些响应，可以通过标头提供恢复 cooldown 持续时间（以秒为单位） `Retry-After` 。 当存在恢复 cooldown 持续时间时，Microsoft Graph 客户端不会在指定的持续时间通过之前发送任何后续请求。
<!-- {
  "type": "#page.annotation",
  "description": "Error handling in Excel Graph.",
  "keywords": "error response, error object, error codes, innerError, error handling",
  "section": "documentation",
  "tocPath": ""
} -->
