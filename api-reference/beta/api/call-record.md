---
title: 'call: record'
description: 录制呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4f20b096964b92db4ce393922efc635142698483
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317657"
---
# <a name="call-record"></a><span data-ttu-id="7f4fa-103">call: record</span><span class="sxs-lookup"><span data-stu-id="7f4fa-103">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f4fa-104">从呼叫中录制简短的音频剪辑。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-104">Record a short audio clip from the call.</span></span> <span data-ttu-id="7f4fa-105">如果 bot 希望在发出提示后从呼叫者处捕获语音响应, 这将非常有用。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-105">This is useful if the bot wants to capture a voice response from the caller following a prompt.</span></span>

> [!Note]
> <span data-ttu-id="7f4fa-106">只有使用[serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)启动的[调用](../resources/call.md)才支持 record 操作。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-106">The record action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span> <span data-ttu-id="7f4fa-107">此操作不会记录整个调用。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-107">This action does not record the entire call.</span></span> <span data-ttu-id="7f4fa-108">录制的最大长度为5分钟。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-108">The maximum length of the recording is 5 minutes.</span></span> <span data-ttu-id="7f4fa-109">录制不会由云通信平台 permamently 保存, 在呼叫结束后不久将被丢弃。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-109">The recording is not saved permamently by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="7f4fa-110">在录制操作完成后, 机器人必须立即下载录制 (使用已完成通知中给出的**recordingLocation**值)。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-110">The bot must download the recording promptly (using the **recordingLocation** value given in the completed notification) after the recording operation finishes.</span></span>


## <a name="permissions"></a><span data-ttu-id="7f4fa-111">权限</span><span class="sxs-lookup"><span data-stu-id="7f4fa-111">Permissions</span></span>
<span data-ttu-id="7f4fa-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f4fa-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f4fa-114">Permission type</span></span> | <span data-ttu-id="7f4fa-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f4fa-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="7f4fa-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f4fa-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f4fa-117">不支持</span><span class="sxs-lookup"><span data-stu-id="7f4fa-117">Not Supported</span></span>        |
| <span data-ttu-id="7f4fa-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f4fa-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f4fa-119">不支持</span><span class="sxs-lookup"><span data-stu-id="7f4fa-119">Not Supported</span></span>        |
| <span data-ttu-id="7f4fa-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f4fa-120">Application</span></span>     | <span data-ttu-id="7f4fa-121">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="7f4fa-121">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="7f4fa-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f4fa-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="7f4fa-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f4fa-123">Request headers</span></span>
| <span data-ttu-id="7f4fa-124">名称</span><span class="sxs-lookup"><span data-stu-id="7f4fa-124">Name</span></span>          | <span data-ttu-id="7f4fa-125">说明</span><span class="sxs-lookup"><span data-stu-id="7f4fa-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7f4fa-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f4fa-126">Authorization</span></span> | <span data-ttu-id="7f4fa-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f4fa-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f4fa-129">Request body</span></span>
<span data-ttu-id="7f4fa-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7f4fa-131">参数</span><span class="sxs-lookup"><span data-stu-id="7f4fa-131">Parameter</span></span>      | <span data-ttu-id="7f4fa-132">类型</span><span class="sxs-lookup"><span data-stu-id="7f4fa-132">Type</span></span>    |<span data-ttu-id="7f4fa-133">说明</span><span class="sxs-lookup"><span data-stu-id="7f4fa-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f4fa-134">提示</span><span class="sxs-lookup"><span data-stu-id="7f4fa-134">prompts</span></span>|<span data-ttu-id="7f4fa-135">[mediaPrompt](../resources/mediaprompt.md)集合</span><span class="sxs-lookup"><span data-stu-id="7f4fa-135">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="7f4fa-136">录制开始前要播放的提示集合 (如果有)。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-136">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="7f4fa-137">客户可以选择单独指定 "playPrompt" 操作, 也可以指定为 "record" 的一部分-几乎所有记录都通过提示进行 preceeded。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-137">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt.</span></span> <span data-ttu-id="7f4fa-138">当前支持仅作为集合的一部分的单个提示。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-138">Current support is only for a single prompt as part of the collection.</span></span> |
|<span data-ttu-id="7f4fa-139">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="7f4fa-139">bargeInAllowed</span></span>|<span data-ttu-id="7f4fa-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f4fa-140">Boolean</span></span>| <span data-ttu-id="7f4fa-141">如果为 true, 则此记录请求将 barge 到其他现有的排队/当前处理的 record/playprompt 请求中。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-141">If true, this record request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="7f4fa-142">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-142">Default = false.</span></span> |
|<span data-ttu-id="7f4fa-143">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="7f4fa-143">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="7f4fa-144">Int32</span><span class="sxs-lookup"><span data-stu-id="7f4fa-144">Int32</span></span>| <span data-ttu-id="7f4fa-145">在我们开始进行记录操作之前, 可以从开始时开始的最大初始静音 (用户无声), 并使操作失败。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-145">Maximum initial silence (user silence) allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="7f4fa-146">如果我们正在播放提示, 则此计时器在提示完成后启动。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-146">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="7f4fa-147">默认值 = 5 秒, 最小值 = 1 秒, 最大值 = 300 秒</span><span class="sxs-lookup"><span data-stu-id="7f4fa-147">Default = 5 seconds, Min = 1 second, Max = 300 seconds</span></span> |
|<span data-ttu-id="7f4fa-148">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="7f4fa-148">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="7f4fa-149">Int32</span><span class="sxs-lookup"><span data-stu-id="7f4fa-149">Int32</span></span>| <span data-ttu-id="7f4fa-150">用户开始发言后允许的最大静音 (暂停) 时间。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-150">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="7f4fa-151">默认值 = 5 秒, 最小值 = 1 秒, 最大值 = 300 秒。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-151">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="7f4fa-152">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="7f4fa-152">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="7f4fa-153">Int32</span><span class="sxs-lookup"><span data-stu-id="7f4fa-153">Int32</span></span>| <span data-ttu-id="7f4fa-154">停止录制前的记录操作的最长持续时间。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-154">Max duration for a record operation before stopping recording.</span></span> <span data-ttu-id="7f4fa-155">默认值 = 5 秒, 最小值 = 1 秒, 最大值 = 300 秒。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-155">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="7f4fa-156">playBeep</span><span class="sxs-lookup"><span data-stu-id="7f4fa-156">playBeep</span></span>|<span data-ttu-id="7f4fa-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f4fa-157">Boolean</span></span>| <span data-ttu-id="7f4fa-158">如果为 true, 则会播放提示音, 指示用户可以开始记录其邮件。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-158">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="7f4fa-159">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-159">Default = true.</span></span>|
|<span data-ttu-id="7f4fa-160">stopTones</span><span class="sxs-lookup"><span data-stu-id="7f4fa-160">stopTones</span></span>|<span data-ttu-id="7f4fa-161">String collection</span><span class="sxs-lookup"><span data-stu-id="7f4fa-161">String collection</span></span>|<span data-ttu-id="7f4fa-162">指定结束录音的停止音。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-162">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="7f4fa-163">适用</span><span class="sxs-lookup"><span data-stu-id="7f4fa-163">clientContext</span></span>|<span data-ttu-id="7f4fa-164">String</span><span class="sxs-lookup"><span data-stu-id="7f4fa-164">String</span></span>|<span data-ttu-id="7f4fa-165">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-165">Unique Client Context string.</span></span> <span data-ttu-id="7f4fa-166">最多可以有256个字符。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-166">Can have a maximum of 256 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="7f4fa-167">响应</span><span class="sxs-lookup"><span data-stu-id="7f4fa-167">Response</span></span>
<span data-ttu-id="7f4fa-168">此方法返回`200 OK`响应代码和位置标头, 其中包含为此请求创建的[recordOperation](../resources/recordoperation.md)的 URI。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-168">This method returns a `200 OK` response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="7f4fa-169">示例</span><span class="sxs-lookup"><span data-stu-id="7f4fa-169">Example</span></span>
<span data-ttu-id="7f4fa-170">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-170">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7f4fa-171">请求</span><span class="sxs-lookup"><span data-stu-id="7f4fa-171">Request</span></span>
<span data-ttu-id="7f4fa-172">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-172">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7f4fa-173">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7f4fa-173">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f4fa-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f4fa-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-record-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7f4fa-175">响应</span><span class="sxs-lookup"><span data-stu-id="7f4fa-175">Response</span></span>
<span data-ttu-id="7f4fa-176">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-176">The following example shows the response.</span></span>

> <span data-ttu-id="7f4fa-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="7f4fa-179">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="7f4fa-179">Notification - operation completed</span></span>

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

##### <a name="get-recording-file---request"></a><span data-ttu-id="7f4fa-180">获取录制文件-请求</span><span class="sxs-lookup"><span data-stu-id="7f4fa-180">Get recording file - Request</span></span>
<span data-ttu-id="7f4fa-181">下面的示例展示了获取录制内容的请求。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-181">The following example shows the request to get the content of the recording.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "download_recorded_file",
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="get-recording-file---response"></a><span data-ttu-id="7f4fa-182">获取录制文件-响应</span><span class="sxs-lookup"><span data-stu-id="7f4fa-182">Get recording file - Response</span></span>
<span data-ttu-id="7f4fa-183">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7f4fa-183">Here is an example of the response.</span></span> 

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
