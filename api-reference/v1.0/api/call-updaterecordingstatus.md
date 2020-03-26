---
title: 调用： updateRecordingStatus
description: 更新与呼叫关联的应用程序的录制状态。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f1109cdaa02d5715335fd0948f64cff9bff8c4dd
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962524"
---
# <a name="call-updaterecordingstatus"></a>调用： updateRecordingStatus

命名空间：microsoft.graph

更新与呼叫关联的应用程序的录制状态。

> [!NOTE]
> **其他限制**：不能使用媒体访问 API 来记录或保留来自应用程序访问的呼叫或会议的媒体内容，或从该媒体内容派生的数据（"record" 或 "record"），而无需先调用**updateRecordingStatus** API 来指示已开始录制，并从该 api 接收成功答复。 如果您的应用程序开始录制任何会议，则它必须在调用**updateRecordingStatus** API 之前结束录制，以指示录制已结束。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）      |
|:---------------------------------------|:-------------------------------------------------|
| 委派（工作或学校帐户）     | 不支持                                    |
| 委派（个人 Microsoft 帐户） | 不支持                                    |
| 应用程序                            | JoinGroupCalls、AccessMedia 和所有调用  |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/updateRecordingStatus
```

## <a name="request-headers"></a>请求标头
| 名称          | 说明               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数       | 类型    | 说明                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| 适用   | String  | 唯一的客户端上下文字符串。 最大限制为256个字符。                                 |
| 状态          | String  | 录制状态。 可能的值包括`notRecording`： `recording`、或`failed`。  |

## <a name="response"></a>响应
此方法返回`200 OK`响应代码和位置标头，其中包含为此请求创建的[UPDATERECORDINGSTATUSOPERATION](../resources/updaterecordingstatusoperation.md)对象的 URI。

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
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/updateRecordingStatus
Content-Type: application/json
Content-Length: 79

{
  "clientContext": "clientContext-value",
  "status": "notRecording | recording | failed"
}
```
---

### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "name": "call-updateRecordingStatus",
  "truncated": true,
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

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
