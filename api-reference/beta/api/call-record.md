---
title: 调用： recordResponse
description: 记录来自呼叫者的简短音频响应。 如果 bot 希望在发出提示后从呼叫者处捕获语音响应，这将非常有用。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8aa5797c95ee3a9edc665f3d8d509ab58fe2dff5
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312349"
---
# <a name="call-recordresponse"></a>调用： recordResponse

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

记录来自呼叫者的简短音频响应。

在收到响应提示后，bot 可以使用此程序从呼叫者处捕获语音响应。

有关如何处理操作的详细信息，请参阅 [commsOperation](../resources/commsOperation.md)

>**注意：** 仅使用[serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)启动的[调用](../resources/call.md)支持此 API。

此操作不用于记录整个调用。 录制的最大长度为2分钟。 录制不会由云通信平台永久保存，并且在呼叫结束后不久将被丢弃。 在录制操作完成后，bot 必须使用已完成的通知中提供的 recordingLocation 值立即下载录制。

>**注意：** 您不能录制或以其他方式保留来自您的应用程序访问的呼叫或会议的媒体内容或从该媒体内容派生的数据。 请确保您符合有关通信的数据保护和机密性的法律和法规。 有关详细信息，请参阅[使用条款](/legal/microsoft-apis/terms-of-use)并咨询法律顾问。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
| :-------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | 不支持        |
| 委派（个人 Microsoft 帐户） | 不支持        |
| 应用程序     | Calls.AccessMedia.All                       |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/recordResponse
POST /communications/calls/{id}/recordResponse
```
> **注意：**`/app` 路径已弃用。 今后将使用 `/communications` 路径。

## <a name="request-headers"></a>请求标头
| 名称          | 说明               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |
| Content-type| application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数      | 类型    |说明|
|:---------------|:--------|:----------|
|提示|[MediaPrompt](../resources/mediaprompt.md) 集合 | 要播放的提示。 支持的最大 mediaPrompt 集合大小为1。|
|bargeInAllowed|Boolean| 如果为 true，则 recordResponse 请求将 barge 到其他现有的排队/当前处理的 record/playprompt 请求中。 默认值为 false。 |
|initialSilenceTimeoutInSeconds | Int32| 最大初始静音 (用户静音) 允许在我们超时之前开始记录响应操作并使操作失败。 如果我们正在播放提示，则此计时器在提示完成后启动。 默认值 = 5 秒，最小值 = 1 秒，最大值 = 120 秒 |
|maxSilenceTimeoutInSeconds|Int32| 最大无声 (暂停用户开始发言后允许的) 时间。 默认值 = 5 秒，最小值 = 1 秒，最大值 = 120 秒。|
|maxRecordDurationInSeconds|Int32| 停止录制前的 recordResponse 操作的最长持续时间。 默认值 = 5 秒，最小值 = 1 秒，最大值 = 120 秒。|
|playBeep|Boolean| 如果为 true，则会播放提示音，指示用户可以开始记录其邮件。 默认值为 true。|
|stopTones|String 集合|指定结束录音的停止音。|
|适用|字符串|唯一的客户端上下文字符串。 最大限制为256个字符。|

> **注意：** 最长录制时间从5分钟减少到2分钟。

## <a name="response"></a>响应
此方法返回一个 `200 OK` HTTP 响应代码和一个位置标头，其中包含为此请求创建的 [RECORDOPERATION](../resources/recordoperation.md) 的 URI。

## <a name="example"></a>示例
以下示例演示如何调用此 API。

### <a name="example-1-records-a-short-audio-response-from-the-caller"></a>示例1：记录来自呼叫者的短音频响应

##### <a name="request"></a>请求
下面为请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-recordResponse"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/recordResponse
Content-Type: application/json
Content-Length: 394

{
  "bargeInAllowed": true,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      }
    }
  ],
  "maxRecordDurationInSeconds": 10,
  "initialSilenceTimeoutInSeconds": 5,
  "maxSilenceTimeoutInSeconds": 2,
  "playBeep": true,
  "stopTones": [ "#", "1", "*" ]
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-recordresponse-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-recordresponse-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-recordresponse-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
以下示例显示了相应的响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.recordOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "completionReason": null,
  "resultInfo": null,
  "recordingLocation": null,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---operation-completed"></a>通知-操作已完成

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.recordOperation",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed",
        "recordingLocation": "https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
        "recordingAccessToken": "<access-token>",
        "completionReason": "stopToneDetected"
      }
    }
  ]
}
```

### <a name="example-2-retrieving-the-recording-file"></a>示例2：检索录制文件

> **注意：** 您不能录制或以其他方式保留来自您的应用程序访问的呼叫或会议的媒体内容或从该媒体内容派生的数据。 请确保您符合有关通信的数据保护和机密性的法律和法规。 有关详细信息，请参阅[使用条款](/legal/microsoft-apis/terms-of-use)并咨询法律顾问。

##### <a name="request"></a>请求

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a>响应

<!-- {
  "blockType": "ignored"
}-->

```http
HTTP/1.1 200 OK
Transfer-Encoding: chunked
Date: Thu, 17 Jan 2019 01:46:37 GMT
Content-Type: application/octet-stream

(application/octet-stream of size 160696 bytes)
```

> **注意：** 您不能录制或以其他方式保留来自您的应用程序访问的呼叫或会议的媒体内容或从该媒体内容派生的数据。 请确保您符合有关通信的数据保护和机密性的法律和法规。 有关详细信息，请参阅[使用条款](/legal/microsoft-apis/terms-of-use)并咨询法律顾问。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: recordResponse",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->