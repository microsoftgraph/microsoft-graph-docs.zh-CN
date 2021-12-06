---
title: call： recordResponse
description: 录制来自呼叫方的简短音频回复。 如果机器人希望按照提示从呼叫者捕获语音响应，这将非常有用。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 266c4541293ee0f6a38b2b15c1037fe4d1347412
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029706"
---
# <a name="call-recordresponse"></a>call： recordResponse

命名空间：microsoft.graph

录制来自呼叫方的简短音频回复。
机器人可以利用此功能在系统提示呼叫者做出响应后捕获来自呼叫者的语音响应。

若要进一步了解如何处理操作，请查看 [commsOperation](../resources/commsOperation.md)

>**注意：** 这仅 [支持通过](../resources/call.md)[serviceHostedMediaConfig 启动的呼叫](../resources/servicehostedmediaconfig.md)。

此操作不用于记录整个呼叫。 录制的最大长度为 2 分钟。 云通信平台不会永久保存录制，呼叫结束后将丢弃录制。 录制操作完成后，机器人必须使用已完成的通知中给出的 recordingLocation 值立即下载录制。

>**注意：** 收集的任何媒体 **可能无法** 保留。 在呼叫录制方面，请确保你遵守你地区的法律和法规。 有关详细信息，请咨询法律顾问。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
| :-------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | 不支持        |
| 委派（个人 Microsoft 帐户） | 不支持        |
| 应用程序     | Calls.AccessMedia.All                       |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/recordResponse
```

## <a name="request-headers"></a>请求标头
| 名称          | 说明               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数      | 类型    |说明|
|:---------------|:--------|:----------|
|prompts|[mediaPrompt](../resources/mediaprompt.md) 集合 | 要播放的提示。 支持的最大 mediaPrompt 集合大小为 1。|
|bargeInAllowed|布尔| 如果为 true，recordResponse 请求将插入其他现有的排队向上/当前处理的记录/playprompt 请求。 默认值 = false。 |
|initialSilenceTimeoutInSeconds | Int32| 在超时 (操作) 开始记录响应操作时，允许的最大初始静默和用户静默。 如果我们播放提示，则此计时器在提示完成后启动。 默认值 = 5 秒，最小值 = 1 秒，最大值 = 120 秒 |
|maxSilenceTimeoutInSeconds|Int32| 用户开始 (后) 允许的最大静默时间。 默认值 = 5 秒，最小值 = 1 秒，最大值 = 120 秒。|
|maxRecordDurationInSeconds|Int32| 在停止录制之前，recordResponse 操作的最大持续时间。 默认值 = 5 秒，最小值 = 1 秒，最大值 = 120 秒。|
|playBeep|布尔| 如果为 true，则播放一个嘟嘟声，以向用户指示他们可以开始录制其消息。 默认值 = true。|
|stopTones|String collection|结束录制指定的停止音调。|
|clientContext|String|唯一的客户端上下文字符串。 最大限制为 256 个字符。|

## <a name="response"></a>响应
此方法将响应代码和 Location 标头的 URI 返回到为此请求 `200 OK` 创建的[recordOperation。](../resources/recordoperation.md)

## <a name="example"></a>示例
以下示例演示如何调用此 API。

### <a name="example-1-records-a-short-audio-response-from-the-caller"></a>示例 1：录制来自呼叫者的简短音频响应

##### <a name="request"></a>请求
下面为请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-recordResponse"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/recordResponse
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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-recordresponse-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/call-recordresponse-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
以下示例显示了相应的响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.recordOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "running",
  "resultInfo": null,
  "recordingLocation": null,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---operation-completed"></a>通知 - 操作已完成

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
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 200,
          "subcode": 8515,
          "message": "Action completed, max record duration reached."
        },
        "recordingLocation": "https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
        "recordingAccessToken": "<access-token>"
      }
    }
  ]
}
```

### <a name="example-2-retrieving-the-recording-file"></a>示例 2：检索录制文件

>**注意：** You may NOT record or otherwise persist media content from calls or meetings that your application accesses， or data derived from that media content. 确保你遵守有关通信数据保护和机密性的法律和法规。 有关详细信息，请参阅[使用条款](/legal/microsoft-apis/terms-of-use)并咨询法律顾问。

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: record",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
