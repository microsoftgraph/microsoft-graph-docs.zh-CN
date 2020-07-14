---
title: Microsoft Graph 错误响应和资源类型
description: "  "
localization_priority: Priority
ms.openlocfilehash: cc3a0a0acacd7477c1cf686089c0235850059443
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091422"
---
# <a name="microsoft-graph-error-responses-and-resource-types"></a>Microsoft Graph 错误响应和资源类型

<!--In this article:
  
-   [Status code](#msg-status-code)
-   [Error resource type](#msg-error-resource-type)
-   [Code property](#msg-code-property)

<a name="msg_error_response"> </a> -->

使用标准的 HTTP 状态代码以及 JSON 错误响应对象返回 Microsoft Graph 中的错误。

## <a name="http-status-codes"></a>HTTP 状态代码

下表列出并描述可以返回的 HTTP 状态代码。

| 状态代码 | 状态消息                  | 说明                                                                                                                            |
|:------------|:--------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------|
| 400         | 错误的请求 (Bad Request)                     | 无法处理请求，因为格式有误或者不正确。                                                                       |
| 401         | 未经授权 (Unauthorized)                    | 资源所需的身份验证信息缺少或无效。                                                   |
| 403         | 禁止访问 (Forbidden)                       | Access is denied to the requested resource. The user might not have enough permission. <br /><br /> **重要说明：** 如果向资源应用了条件访问策略，可能会返回 HTTP 403 禁止错误 (error=insufficent_claims)。 有关 Microsoft Graph 和条件访问的详细信息，请参阅 [Azure Active Directory 条件性访问开发人员指南](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer)  |
| 404         | 未找到 (Not Found)                       | 所请求的资源不存在。                                                                                                  |
| 405         | 方法不允许 (Method Not Allowed)              | 请求中的 HTTP 方法在资源上不允许。                                                                         |
| 406         | 不接受 (Not Acceptable)                  | 该服务不支持“Accept”标头中请求的格式。                                                                |
| 409         | 冲突 (Conflict)                        | The current state conflicts with what the request expects. For example, the specified parent folder might not exist.                   |
| 410         | 不存在 (Gone)                            | 所请求的资源在服务器不再可用。                                               |
| 411         | 需要长度 (Length Required)                 | 请求上需要 Content-Length 标头。                                                                                    |
| 412         | 前提条件不满足 (Precondition Failed)             | 请求中提供的前提条件（例如“If-Match”标头）与资源的当前状态不匹配。                       |
| 413         | 请求实体太大 (Request Entity Too Large)        | 请求的大小超出最大限制。                                                                                            |
| 415         | 媒体类型不受支持 (Unsupported Media Type)          | 请求的内容类型的格式不受服务支持。                                                      |
| 416         | 请求的范围不满足 (Requested Range Not Satisfiable) | 指定的字节范围无效或不可用。                                                                                    |
| 422         | 实体无法处理 (Unprocessable Entity)            | 无法处理请求，因为语义上不正确。                                                                        |
| 423         | 已锁定                          | 正在访问的资源被锁定。                                                                                          |
| 429         | 请求过多 (Too Many Requests)               | 客户端应用程序已被限制，经过一段时间之后再尝试重复的请求。                |
| 500         | 内部服务器错误 (Internal Server Error)           | 处理请求时出现内部服务器错误。                                                                       |
| 501         | 未实现 (Not Implemented)                 | 所请求的功能未实现。                                                                                               |
| 503         | 服务不可用             | The service is temporarily unavailable for maintenance or is overloaded. You may repeat the request after a delay, the length of which may be specified in a Retry-After header.|
| 504         | 网关超时                 | The server, while acting as a proxy, did not receive a timely response from the upstream server it needed to access in attempting to complete the request. May occur together with 503. |
| 507         | 存储不足 (Insufficient Storage)            | 已达到最大存储配额。                                                                                            |
| 509         | 超出带宽限制 (Bandwidth Limit Exceeded)        | Your app has been throttled for exceeding the maximum bandwidth cap. Your app can retry the request again after more time has elapsed. |

The error response is a single JSON object that contains a single property named **error**. This object includes all the details of the error. You can use the information returned here instead of or in addition to the HTTP status code. The following is an example of a full JSON error body.

<!-- { "blockType": "ignored", "@odata.type": "odata.error", "expectError": true, "name": "example-error-response" } -->
```json
{
  "error": {
    "code": "invalidRange",
    "message": "Uploaded fragment overlaps with existing data.",
    "innerError": {
      "requestId": "request-id",
      "date": "date-time"
    }
  }
}
```

<!--<a name="msg_error_resource_type"> </a> -->

## <a name="error-resource-type"></a>错误的资源类型

只要处理请求的过程中出现错误，就会返回错误资源。

错误响应遵循错误响应 [OData v4](https://docs.oasis-open.org/odata/odata-json-format/v4.0/os/odata-json-format-v4.0-os.html#_Toc372793091) 规范中的定义。

### <a name="json-representation"></a>JSON 表示形式

错误资源包括以下资源：

<!-- { "blockType": "resource", "@odata.type": "odata.error" } -->
```json
{
  "error": { "@odata.type": "odata.error" }  
}
```

#### <a name="odataerror-resource-type"></a>odata.error 资源类型

错误响应内是错误资源，其中包括以下属性：

<!-- { "blockType": "resource", "@odata.type": "odata.error", "optionalProperties": [ "target", "details", "innererror"] } -->
```json
{
  "code": "string",
  "message": "string",
  "innererror": { "@odata.type": "odata.error" }
}
```

| 属性名称  | 值                  | 说明\                                                                                               |
|:---------------|:-----------------------|:-----------------------------------------------------------------------------------------------------------|
| **code**       | string                 | 发生的错误的错误代码字符串                                                            |
| **message**    | string                 | A developer ready message about the error that occurred. This should not be displayed to the user directly. |
| **innererror** | error object           | Optional. Additional error objects that may be more specific than the top level error.                     |

<!--<a name="msg_code_property"> </a> -->

#### <a name="code-property"></a>代码属性

The `code` property contains one of the following possible values. Your apps should be prepared to handle any one of these errors.

| 代码                      | 说明
|:--------------------------|:--------------
| **accessDenied**          | 调用方没有执行该操作的权限。 
| **activityLimitReached**  | 应用或用户已被限制。
| **generalException**      | 发生未指定错误。
| **invalidRange**          | 指定的字节范围无效或不可用。
| **invalidRequest**        | 该请求格式有误或不正确。
| **itemNotFound**          | 找不到资源。
| **malwareDetected**       | 所请求的资源中检测到恶意软件。
| **nameAlreadyExists**     | 指定的项目名称已存在。
| **notAllowed**            | 系统不允许执行此操作。
| **notSupported**          | 系统不支持该请求。
| **resourceModified**      | 正在更新的资源自上次调用方读取时已进行了更改，通常是 eTag 不匹配。
| **resyncRequired**        | 增量令牌将不再有效，并且应用必须重置同步状态。
| **serviceNotAvailable**   | The service is not available. Try the request again after a delay. There may be a Retry-After header. 
| **syncStateNotFound**     | 找不到同步状态生成。 增量令牌已过期，必须重新进行数据同步。 
| **quotaLimitReached**     | 用户已达到其配额限制。
| **unauthenticated**       | 调用方未进行身份验证。

The `innererror` object might recursively contain more `innererror` objects with additional, more specific error codes. When handling an error, apps should loop through all the error codes available and use the most detailed one that they understand. Some of the more detailed codes are listed at the bottom of this page.

To verify that an error object is an error you are expecting, you must loop over the `innererror` objects, looking for the error codes you expect. For example:

```csharp
public bool IsError(string expectedErrorCode)
{
    OneDriveInnerError errorCode = this.Error;
    while (null != errorCode)
    {
        if (errorCode.Code == expectedErrorCode)
            return true;
        errorCode = errorCode.InnerError;
    }
    return false;
}
```

有关介绍如何正确处理错误的示例，请参阅 [错误代码处理](https://gist.github.com/rgregg/a1866be15e685983b441)。

The `message` property at the root contains an error message intended for the developer to read. Error messages are not localized and shouldn't be displayed directly to the user. When handling errors, your code should not key off of `message` values because they can change at any time, and they often contain dynamic information specific to the failed request. You should only code against error codes returned in `code` properties.

#### <a name="detailed-error-codes"></a>详细的错误代码
The following are some additional errors that your app might encounter within the nested `innererror` objects. Apps are not required to handle these, but can if they choose. The service might add new error codes or stop returning old ones at any time, so it is important that all apps be able to handle the [basic error codes](#code-property).

| 代码                               | 说明
|:-----------------------------------|:----------------------------------------------------------
| **accessRestricted**               | 访问仅限于该项目的所有者。
| **cannotSnapshotTree**             | Failed to get a consistent delta snapshot. Try again later.
| **childItemCountExceeded**         | 已达到最大子项目数限制。
| **entityTagDoesNotMatch**          | ETag 与当前项目的值不匹配。
| **fragmentLengthMismatch**         | 为此片段声明的总大小与上载会话的大小不同。
| **fragmentOutOfOrder**             | 已上载的片段无序。
| **fragmentOverlap**                | 上载的片段与现有数据重叠。
| **invalidAcceptType**              | 接受类型无效。
| **invalidParameterFormat**         | 参数格式无效。
| **invalidPath**                    | 名称包含无效字符。
| **invalidQueryOption**             | 查询选项无效。
| **invalidStartIndex**              | 开始索引无效。
| **lockMismatch**                   | 锁定令牌与现有锁定不匹配。
| **lockNotFoundOrAlreadyExpired**   | 该项目上目前没有未过期的锁定。
| **lockOwnerMismatch**              | 锁定所有者 ID 与提供的 ID 不匹配。
| **malformedEntityTag**             | ETag header is malformed. ETags must be quoted strings.
| **maxDocumentCountExceeded**       | 已达到最大文档数量限制。
| **maxFileSizeExceeded**            | 已超出最大文件大小。
| **maxFolderCountExceeded**         | 已达到最大文件夹数量限制。
| **maxFragmentLengthExceeded**      | 已超出最大文件大小。
| **maxItemCountExceeded**           | 已达到最大项目数量限制。
| **maxQueryLengthExceeded**         | 已超出最大查询长度。
| **maxStreamSizeExceeded**          | 已达到最大流大小。
| **parameterIsTooLong**             | 参数超出最大长度。
| **parameterIsTooSmall**            | 参数小于最小值。
| **pathIsTooLong**                  | 路径超出最大长度。
| **pathTooDeep**                    | 已达到文件夹层次结构深度限制。
| **propertyNotUpdateable**          | 属性无法更新。
| **resyncApplyDifferences**         | Resync required. Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.
| **resyncRequired**                 | 需要重新同步。
| **resyncUploadDifferences**        | Resync required. Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).
| **serviceNotAvailable**            | 服务器无法处理当前的请求。
| **serviceReadOnly**                | 资源暂时是只读的。
| **throttledRequest**               | 请求过多。
| **tooManyResultsRequested**        | 请求的结果过多。
| **tooManyTermsInQuery**            | 查询中的术语过多。
| **totalAffectedItemCountExceeded** | 因为受影响的项目数量超出阈值，所以不允许该操作。
| **truncationNotAllowed**           | 不允许数据截断。
| **uploadSessionFailed**            | 上载会话失败。
| **uploadSessionIncomplete**        | 上载会话未完成。
| **uploadSessionNotFound**          | 上载会话未找到。
| **virusSuspicious**                | 此文档可疑，可能存在病毒。
| **zeroOrFewerResultsRequested**    | 请求的结果为零或更少。


<!-- {
  "type": "#page.annotation",
  "description": "Understand the error format for the API and error codes.",
  "keywords": "error response, error, error codes, innererror, message, code",
  "section": "documentation",
  "suppressions": [
    " Warning: /concepts/errors.md:
      Multiple resources found in file, but we only support one per file. 'odata.error,odata.error'. Skipping."
  ],
  "tocPath": "Misc/Error Responses"
} -->
