---
title: call： updateRecordingStatus
description: 更新与呼叫关联的应用程序录制状态。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 4b1757c3a4a3c28613ff8c45c4ced22beeb9e207
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608007"
---
# <a name="call-updaterecordingstatus"></a>call： updateRecordingStatus

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新与呼叫关联的应用程序录制状态。 这需要使用基于Teams[录制解决方案](/MicrosoftTeams/teams-recording-policy)。

> 其他限制：如果不首先调用 **updateRecordingStatus** API 以指示录制已开始，并且从该 API 收到成功回复，则不得使用媒体访问 API 记录或以其他方式保留应用程序访问的呼叫或会议中的媒体内容，或者记录派生自该媒体内容 ("record"或"recording") 的数据。 如果应用程序开始录制任何会议，则必须在调用 **updateRecordingStatus** API 之前结束录制，以指示录制已结束。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）      |
|:---------------------------------------|:-------------------------------------------------|
| 委派（工作或学校帐户）     | 不支持                                    |
| 委派（个人 Microsoft 帐户） | 不支持                                    |
| Application                            | Calls.JoinGroupCalls.All、Calls.AccessMedia.All  |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateRecordingStatus
POST /communications/calls/{id}/updateRecordingStatus
```
> **注意：**`/app` 路径已弃用。 今后将使用 `/communications` 路径。

## <a name="request-headers"></a>请求标头
| 名称          | 说明               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数       | 类型    | 说明                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| clientContext   | String  | 唯一的客户端上下文字符串。 最大限制为 256 个字符。                                 |
| 状态          | String  | 录制状态。 可能的值为： `notRecording`、 `recording`或 `failed`。  |

## <a name="response"></a>响应
此方法向为此 `200 OK` 请求创建的 [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) 对象返回响应代码和具有 URI 的位置标头。

## <a name="example"></a>示例
以下示例演示如何调用此 API。

### <a name="request"></a>请求
下面为请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-updateRecordingStatus"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/updateRecordingStatus
Content-Type: application/json
Content-Length: 79

{
  "clientContext": "clientContext-value",
  "status": "notRecording | recording | failed"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-updaterecordingstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/call-updaterecordingstatus-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/call-updaterecordingstatus-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "name": "call-updateRecordingStatus",
  "truncated": true,
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.updateRecordingStatusOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "resultInfo": null,
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: updateRecordingStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
