---
title: Excel API 的错误处理
description: 查找有关处理 Microsoft Graph 中 Excel API 在通过 API 发送的请求失败时返回的错误的常规说明和建议。
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: 7e115fe0a09c519ecad98f49524ca3ebd86001fd
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645411"
---
# <a name="error-handling-for-excel-apis"></a>Excel API 的错误处理

本文提供有关处理 Microsoft Graph 中 [Excel API](/graph/api/resources/excel) 在通过 API 发送的请求失败时返回的错误的一般说明和建议。

## <a name="types-of-error-responses"></a>错误响应的类型

Microsoft Graph 中的 Excel API 返回两种类型的错误。 一个是常规错误响应，如下所示。

```http
HTTP/1.1 <HTTP status code>
Content-type: application/json
Retry-After: <Cooldown duration in seconds> (optional)

{
  "error": <Error object>
}
```

第二种 `200 OK` 来自长时间运行的操作模式，该模式可在响应正文中返回 HTTP 状态代码和 `failed` 操作状态，如以下示例所示。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "status": "failed",
  "error": <Error object>
}
```

对于这两个错误响应，错误对象具有以下结构。

> [!NOTE]
> 错误响应遵循错误响应 [OData v4](https://docs.oasis-open.org/odata/odata-json-format/v4.0/os/odata-json-format-v4.0-os.html#_Toc372793091) 规范中的定义。

```json
{
  "code": "string",
  "message": "string",
  "innerError": { "@odata.type": "odata.error" }
}
```

**innerError** 对象可能以递归方式包含更多具有更多、更具体的错误代码的 **innerError** 对象。 例如，错误对象可能包含第二级错误代码和消息中更详细的错误信息，如下所示。

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

Microsoft Graph 客户端应使用以下步骤来处理 Excel API 出现的错误。

### <a name="1-determine-whether-it-is-a-long-running-operation-error"></a>1.确定它是否是长时间运行的操作错误

在处理错误之前，第一步是确定错误响应是来自长时间运行的操作模式还是常规模式。 长时间运行的操作错误将在响应正文中返回 `200 OK` HTTP 状态代码和 `failed` 操作状态。 常规错误响应将返回相应的 HTTP 错误状态代码。 

### <a name="2-parse-second-level-error-code"></a>2. 分析二级错误代码

对于长时间运行的操作模式和常规模式，客户端应首先分析所需的二级错误代码，并根据说明进行处理。 或者，客户端还可以处理其他二级错误代码，或者选择回退到 [顶级错误代码](#3-parse-the-top-level-error-code) 或 [状态代码](#4-parse-the-status-code)。

错误代码不区分大小写。

#### <a name="required-second-level-error-codes"></a>必需的二级错误代码

下表列出了 Microsoft Graph 客户端应处理的必需二级错误代码的说明。 该服务可能随时添加新的错误代码。

| 代码                               | 说明
|:-----------------------------------|:---------------------------------------------
| `accessConflict`   | 失败的请求与访问工作簿 (的其他客户端冲突，例如，另一个客户端锁定了工作簿以进行编辑) 。 在冲突解决之前，预计 Microsoft Graph 客户端不会重新发送失败的请求。 最终用户可以选择使用 Excel Online 手动执行相同的操作，以获取有关冲突的更多详细信息。
| `badRequestUncategorized`    | 在失败的请求中发现未指定的错误。 预计 Microsoft Graph 客户端不会重新发送失败的请求。
| `conflictUncategorized`                   | 失败的请求与某些服务器状态冲突。 在冲突解决之前，预计 Microsoft Graph 客户端不会重新发送失败的请求。 最终用户可以选择使用 Excel Online 手动执行相同的操作，以获取有关冲突的更多详细信息。
| `forbiddenUncategorized`                    | 不允许失败的请求。 预计 Microsoft Graph 客户端不会重新发送失败的请求。 最终用户可以选择使用 Excel Online 手动执行相同的操作，以获取有关限制的更多详细信息。
| `gatewayTimeoutUncategorized`         | 服务无法在时间限制内完成请求。
| `internalServerErrorUncategorized`       | 发生未指定错误。 预计 Microsoft Graph 客户端不会重新发送失败的请求。 如果在失败的请求中指定了会话，则也不会进一步访问会话。
| `invalidSessionAccessConflict`             | 请求中指定的会话无效，因为与其他访问工作簿的客户端发生冲突 (例如，另一个客户端锁定了工作簿以进行编辑) 。 预计不会进一步访问失败请求中指定的会话。 在冲突解决之前，预计不会使用相同的 **createSession** 请求重新创建会话。 使用不同的 **createSession** 请求重新创建会话可能会成功，也可能不成功。 最终用户可以选择使用 Excel Online 手动执行相同的操作，以获取有关冲突的更多详细信息。
| `invalidSessionAuthentication`         | 由于身份验证错误，请求中指定的会话无效。 预计不会进一步访问失败请求中指定的会话。 在提供适当的身份验证信息之前，预计不会使用相同的 **createSession** 请求重新创建会话。
| `invalidSessionNotFound`         | 请求中指定的会话无效，因为找不到工作簿。 预计不会进一步访问失败请求中指定的会话。 不需要使用相同的 **createSession** 请求重新创建会话。
| `invalidSessionReCreatable`             | 请求中指定的会话不存在或由于暂时性错误而无效。 Microsoft Graph 客户端可以尝试重新创建会话并恢复工作。 预计不会进一步访问失败请求中指定的会话。
| `invalidSessionRestricted`          | 由于服务配置或限制，请求中指定的会话无效。 预计不会进一步访问失败请求中指定的会话。 在阻止请求的限制或配置更改之前，预计不会使用相同的 **createSession** 请求重新创建会话。 使用不同的 **createSession** 请求重新创建会话可能会成功，也可能不成功。 最终用户可以选择使用 Excel Online 手动执行相同的操作，以获取有关限制的更多详细信息。
| `invalidSessionUnexpected`                | 由于出现意外问题，请求中指定的会话无效。 预计不会进一步访问失败请求中指定的会话。 不需要使用相同的 **createSession** 请求重新创建会话。 使用不同的 **createSession** 请求重新创建会话可能会成功，也可能不成功。
| `invalidSessionUnsupportedWorkbook`              | 请求中指定的会话无效，因为工作簿包含不受支持的功能或超出了大小限制。 通常，访问工作簿的另一个客户端会引入不受支持的因素。 预计不会进一步访问失败请求中指定的会话。 在删除不受支持的因素之前，预计不会使用相同的 **createSession** 请求重新创建会话。 使用不同的 createSession 请求重新创建会话可能会成功，也可能不成功。 最终用户可以选择使用 Excel Online 手动执行相同的操作，以获取不受支持的因素的更多详细信息，或者使用可能支持工作簿的 Excel Desktop。
| `methodNotAllowedUncategorized`              | 不允许在资源上使用请求中指定的 HTTP 方法。 预计 Microsoft Graph 客户端不会重新发送失败的请求。
| `notFoundUncategorized`             | 找不到请求的资源。 预计 Microsoft Graph 客户端不会重新发送失败的请求。
| `notImplementedUncategorized`            | 当前未实现所请求的功能。 预计 Microsoft Graph 客户端不会重新发送失败的请求。
| `payloadTooLargeUncategorized`              | 请求有效负载超出大小限制。 预计 Microsoft Graph 客户端不会重新发送失败的请求。
| `serviceUnavailableUncategorized`      | 服务暂时不可用或重载。 在指定的冷却持续时间过去之前，预计 Microsoft Graph 客户端不会重新发送失败的请求。
| `tooManyRequestsUncategorized`             | 失败的请求超出了某些频率限制。 在指定的冷却持续时间过去之前，预计 Microsoft Graph 客户端不会重新发送失败的请求。 有关减少限制的最佳做法，请参阅 [“减少限制”错误](workbook-best-practice.md#reduce-throttling-errors)。
| `transientFailure`           | 由于暂时性错误，请求失败。 在指定的冷却持续时间过去之前，预计 Microsoft Graph 客户端不会重新发送失败的请求。
| `unauthorizedUncategorized`         | 资源所需的身份验证信息缺失或无效。 预计 Microsoft Graph 客户端不会重新发送失败的请求。
| `unsupportedWorkbook`         | 请求失败。 工作簿包含不受支持的功能或超出大小限制。 在删除不受支持的因素之前，预计 Microsoft Graph 客户端不会重新发送失败的请求。

> [!NOTE]
> 对于常规模式，失败的请求定义为与响应相对应的请求。 对于长时间运行的操作模式，失败的请求是触发失败操作的请求。

#### <a name="optional-second-level-error-code-examples"></a>可选的二级错误代码示例

下表列出了可选的二级错误代码示例，包括每个错误代码的相应处理说明。 该服务可能随时添加新的错误代码。

| 代码                      | 说明                                                                                                                                                                                                                                                                                                                           |
|:--------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `accessDenied`          | 无法执行请求的操作 (例如，对锁定单元格) 执行更改。 预计 Microsoft Graph 客户端不会重新发送失败的请求。                                                                                                                                                                 |
| `filteredRangeConflict` | 操作失败，因为它与筛选的范围冲突。 预计 Microsoft Graph 客户端不会重新发送失败的请求。                                                                                                                                                                                              |
| `generalException`      | 处理请求时发生内部错误。 预计 Microsoft Graph 客户端不会重新发送失败的请求。                                                                                                                                                                                                      |
| `insertDeleteConflict`  | 尝试的插入或删除操作导致冲突。 预计 Microsoft Graph 客户端不会重新发送失败的请求。 最终用户可以选择使用 Excel Online 手动执行相同的操作，以获取有关冲突的更多详细信息。                                                                     |
| `invalidArgument`       | 参数无效、缺失或格式不正确。 预计 Microsoft Graph 客户端不会重新发送失败的请求。                                                                                                                                                                                                |
| `invalidReference`      | 此引用对于当前操作无效。 预计 Microsoft Graph 客户端不会重新发送失败的请求。                                                                                                                                                                                                        |
| `itemAlreadyExists`     | 所创建的资源已存在。 预计 Microsoft Graph 客户端不会重新发送失败的请求。                                                                                                                                                                                                                    |
| `itemNotFound`          | 所请求的资源不存在。 预计 Microsoft Graph 客户端不会重新发送失败的请求。                                                                                                                                                                                                                         |
| `methodNotAllowed`      | 不允许在资源上使用请求中指定的 HTTP 方法。 预计 Microsoft Graph 客户端不会重新发送失败的请求。                                                                                                                                                                                      |
| `nonBlankCellOffSheet`  | 无法插入新单元格，因为它会将非空单元格推离工作表的末尾。 预计 Microsoft Graph 客户端不会重新发送失败的请求。 最终用户可以删除行或列，为插入内容腾出空间，然后重试。                                                                 |
| `rangeExceedsLimit`     | 范围内的单元格计数已超过支持的最大数目。 Microsoft Graph 客户端可以尝试发送范围较小的请求。 有关详细信息，请参阅 [Office 加载项的资源限制和性能优化](/office/dev/add-ins/concepts/resource-limits-and-performance-optimization#excel-add-ins)。 |
| `requestAborted`        | 请求在运行期间中止，这通常是由于工作簿中函数的长时间计算造成的。 预计 Microsoft Graph 客户端不会重新发送失败的请求。                                                                                                                                    |
| `unsupportedOperation`  | 不支持正在尝试的操作。 预计 Microsoft Graph 客户端不会重新发送失败的请求。                                                                                                                                                                                                               |

> [!NOTE]
> 对于常规模式，失败的请求定义为与响应相对应的请求。 对于长时间运行的操作模式，失败的请求是触发失败操作的请求。

### <a name="3-parse-the-top-level-error-code"></a>3. 分析顶级错误代码

如果找不到任何已知的二级错误代码，应按照针对顶级错误提供的说明操作。 顶级错误代码绑定到状态代码，可以根据相应的状态代码执行操作。 有关顶级错误代码和消息的详细信息，请参阅 [错误代码和消息](workbook-error-codes.md#error-codes-and-messages)。

### <a name="4-parse-the-status-code"></a>4. 分析状态代码

对于常规模式，如果找不到任何已知的二级错误代码或顶级错误代码，则应根据 HTTP 状态代码采取措施。

### <a name="5-error-recovery-cooldown"></a>5. 恢复冷落错误

对于常规模式中的某些响应，可以通过标头提供 `Retry-After` 恢复冷却持续时间（以秒为单位）。 如果存在恢复冷却持续时间，则在指定的持续时间过去之前，Microsoft Graph 客户端不会发送任何后续请求。 有关 `Retry-After` 标头和限制的最佳做法，请参阅 [“减少限制”错误](workbook-best-practice.md#reduce-throttling-errors)。

## <a name="diagnostic-information"></a>诊断信息

响应中未在前面的步骤中使用的所有内容仅用于诊断目的 (包括 **消息** 字段) 中的字符串。 我们不建议你依赖这些内容，因为它们可能会在不通知的情况下更改。

## <a name="special-case-handling"></a>特殊案例处理

对于 [会话请求](excel-manage-sessions.md#request-types)，如果遇到 `502/badGateway` 或 `503/serviceUnavailable` 错误，在找到已知的二级错误代码时，请按照相应的说明操作;否则，应直接重新创建会话。
<!-- {
  "type": "#page.annotation",
  "description": "Error handling in Excel Graph.",
  "keywords": "error response, error object, error codes, innerError, error handling",
  "section": "documentation",
  "tocPath": ""
} -->

## <a name="see-also"></a>另请参阅

- [使用 Excel REST API](/graph/api/resources/excel)
