---
title: 'call: record'
description: 录制呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 473816bb52d441b4111632a69d767319ff59a17e
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062007"
---
# <a name="call-record"></a>call: record

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从呼叫中录制简短的音频剪辑。 如果 bot 希望在发出提示后从呼叫者处捕获语音响应, 这将非常有用。

> [!Note]
> 只有使用[serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)启动的[调用](../resources/call.md)才支持 record 操作。 此操作不会记录整个调用。 录制的最大长度为5分钟。 录制不会由云通信平台 permamently 保存, 在呼叫结束后不久将被丢弃。 在录制操作完成后, 机器人必须立即下载录制 (使用已完成通知中给出的**recordingLocation**值)。


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
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a>请求标头
| 名称          | 说明               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数      | 类型    |说明|
|:---------------|:--------|:----------|
|提示|[mediaPrompt](../resources/mediaprompt.md)集合 | 录制开始前要播放的提示集合 (如果有)。 客户可以选择单独指定 "playPrompt" 操作, 也可以指定为 "record" 的一部分-几乎所有记录都通过提示进行 preceeded。 当前支持仅作为集合的一部分的单个提示。 |
|bargeInAllowed|Boolean| 如果为 true, 则此记录请求将 barge 到其他现有的排队/当前处理的 record/playprompt 请求中。 默认值为 false。 |
|initialSilenceTimeoutInSeconds | Int32| 在我们开始进行记录操作之前, 可以从开始时开始的最大初始静音 (用户无声), 并使操作失败。 如果我们正在播放提示, 则此计时器在提示完成后启动。 默认值 = 5 秒, 最小值 = 1 秒, 最大值 = 300 秒 |
|maxSilenceTimeoutInSeconds|Int32| 用户开始发言后允许的最大静音 (暂停) 时间。 默认值 = 5 秒, 最小值 = 1 秒, 最大值 = 300 秒。|
|maxRecordDurationInSeconds|Int32| 停止录制前的记录操作的最长持续时间。 默认值 = 5 秒, 最小值 = 1 秒, 最大值 = 300 秒。|
|playBeep|Boolean| 如果为 true, 则会播放提示音, 指示用户可以开始记录其邮件。 默认值为 true。|
|stopTones|String collection|指定结束录音的停止音。|
|适用|String|唯一的客户端上下文字符串。 最多可以有256个字符。|

## <a name="response"></a>响应
此方法返回`200 OK`响应代码和位置标头, 其中包含为此请求创建的[recordOperation](../resources/recordoperation.md)的 URI。

## <a name="example"></a>示例
以下示例演示如何调用此 API。

##### <a name="request"></a>请求
下面为请求示例。


# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-record"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/record
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
# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-record-javascript-snippets.md)]
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
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.recordOperation",
  "status": "running",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "completionReason": null,
  "resultInfo": null,
  "recordingLocation": null,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a>通知-操作已完成

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.recordOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
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

##### <a name="get-recording-file---request"></a>获取录制文件-请求
下面的示例展示了获取录制内容的请求。

<!-- {
  "blockType": "ignored",
  "name": "download_recorded_file",
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="get-recording-file---response"></a>获取录制文件-响应
下面是一个响应示例。 

<!-- {
  "blockType": "ignored",
  "name": "download_recorded_file",
  "truncated": true
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
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
