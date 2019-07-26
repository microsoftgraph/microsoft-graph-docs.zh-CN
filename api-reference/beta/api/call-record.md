---
title: 'call: record'
description: 录制呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 97f182c58af3ac75d816b3e8a0e7a6fb5f3af1d7
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908332"
---
# <a name="call-record"></a><span data-ttu-id="146e5-103">call: record</span><span class="sxs-lookup"><span data-stu-id="146e5-103">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="146e5-104">从呼叫中录制简短的音频剪辑。</span><span class="sxs-lookup"><span data-stu-id="146e5-104">Record a short audio clip from the call.</span></span> <span data-ttu-id="146e5-105">如果 bot 希望在发出提示后从呼叫者处捕获语音响应, 这将非常有用。</span><span class="sxs-lookup"><span data-stu-id="146e5-105">This is useful if the bot wants to capture a voice response from the caller following a prompt.</span></span>

> [!Note]
> <span data-ttu-id="146e5-106">仅使用[serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)启动的[呼叫](../resources/call.md)支持此记录操作。</span><span class="sxs-lookup"><span data-stu-id="146e5-106">This record action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span> <span data-ttu-id="146e5-107">此操作不会记录整个调用。</span><span class="sxs-lookup"><span data-stu-id="146e5-107">This action does not record the entire call.</span></span> <span data-ttu-id="146e5-108">录制的最大长度为5分钟。</span><span class="sxs-lookup"><span data-stu-id="146e5-108">The maximum length of the recording is 5 minutes.</span></span> <span data-ttu-id="146e5-109">录制不会由 bot 平台保存 permamently, 在呼叫结束后不久将被丢弃。</span><span class="sxs-lookup"><span data-stu-id="146e5-109">The recording is not saved permamently by the bot platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="146e5-110">在录制操作完成后, 机器人必须立即下载录制 (使用已完成通知中给出的**recordingLocation**值)。</span><span class="sxs-lookup"><span data-stu-id="146e5-110">The bot must download the recording promptly (using the **recordingLocation** value given in the completed notification) after the recording operation finishes.</span></span>


## <a name="permissions"></a><span data-ttu-id="146e5-111">权限</span><span class="sxs-lookup"><span data-stu-id="146e5-111">Permissions</span></span>
<span data-ttu-id="146e5-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="146e5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="146e5-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="146e5-114">Permission type</span></span> | <span data-ttu-id="146e5-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="146e5-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="146e5-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="146e5-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="146e5-117">不支持</span><span class="sxs-lookup"><span data-stu-id="146e5-117">Not Supported</span></span>        |
| <span data-ttu-id="146e5-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="146e5-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="146e5-119">不支持</span><span class="sxs-lookup"><span data-stu-id="146e5-119">Not Supported</span></span>        |
| <span data-ttu-id="146e5-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="146e5-120">Application</span></span>     | <span data-ttu-id="146e5-121">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="146e5-121">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="146e5-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="146e5-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="146e5-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="146e5-123">Request headers</span></span>
| <span data-ttu-id="146e5-124">名称</span><span class="sxs-lookup"><span data-stu-id="146e5-124">Name</span></span>          | <span data-ttu-id="146e5-125">说明</span><span class="sxs-lookup"><span data-stu-id="146e5-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="146e5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="146e5-126">Authorization</span></span> | <span data-ttu-id="146e5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="146e5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="146e5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="146e5-129">Request body</span></span>
<span data-ttu-id="146e5-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="146e5-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="146e5-131">参数</span><span class="sxs-lookup"><span data-stu-id="146e5-131">Parameter</span></span>      | <span data-ttu-id="146e5-132">类型</span><span class="sxs-lookup"><span data-stu-id="146e5-132">Type</span></span>    |<span data-ttu-id="146e5-133">说明</span><span class="sxs-lookup"><span data-stu-id="146e5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="146e5-134">提示</span><span class="sxs-lookup"><span data-stu-id="146e5-134">prompts</span></span>|<span data-ttu-id="146e5-135">[mediaPrompt](../resources/mediaprompt.md)集合</span><span class="sxs-lookup"><span data-stu-id="146e5-135">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="146e5-136">录制开始前要播放的提示集合 (如果有)。</span><span class="sxs-lookup"><span data-stu-id="146e5-136">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="146e5-137">客户可以选择单独指定 "playPrompt" 操作, 也可以指定为 "record" 的一部分-几乎所有记录都通过提示进行 preceeded。</span><span class="sxs-lookup"><span data-stu-id="146e5-137">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt.</span></span> <span data-ttu-id="146e5-138">当前支持仅作为集合的一部分的单个提示。</span><span class="sxs-lookup"><span data-stu-id="146e5-138">Current support is only for a single prompt as part of the collection.</span></span> |
|<span data-ttu-id="146e5-139">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="146e5-139">bargeInAllowed</span></span>|<span data-ttu-id="146e5-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="146e5-140">Boolean</span></span>| <span data-ttu-id="146e5-141">如果为 true, 则此记录请求将 barge 到其他现有的排队/当前处理的 record/playprompt 请求中。</span><span class="sxs-lookup"><span data-stu-id="146e5-141">If true, this record request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="146e5-142">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="146e5-142">Default = false.</span></span> |
|<span data-ttu-id="146e5-143">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="146e5-143">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="146e5-144">Int32</span><span class="sxs-lookup"><span data-stu-id="146e5-144">Int32</span></span>| <span data-ttu-id="146e5-145">允许从我们开始记录操作到超时和运行失败的时间开始的最大初始静音。</span><span class="sxs-lookup"><span data-stu-id="146e5-145">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="146e5-146">如果我们正在播放提示, 则此计时器在提示完成后启动。</span><span class="sxs-lookup"><span data-stu-id="146e5-146">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="146e5-147">默认值 = 5 秒, 最小值 = 1 秒, 最大值 = 300 秒</span><span class="sxs-lookup"><span data-stu-id="146e5-147">Default = 5 seconds, Min = 1 second, Max = 300 seconds</span></span> |
|<span data-ttu-id="146e5-148">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="146e5-148">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="146e5-149">Int32</span><span class="sxs-lookup"><span data-stu-id="146e5-149">Int32</span></span>| <span data-ttu-id="146e5-150">用户开始发言后允许的最大静音 (暂停) 时间。</span><span class="sxs-lookup"><span data-stu-id="146e5-150">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="146e5-151">默认值 = 5 秒, 最小值 = 1 秒, 最大值 = 300 秒。</span><span class="sxs-lookup"><span data-stu-id="146e5-151">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="146e5-152">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="146e5-152">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="146e5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="146e5-153">Int32</span></span>| <span data-ttu-id="146e5-154">停止录制前的记录操作的最长持续时间。</span><span class="sxs-lookup"><span data-stu-id="146e5-154">Max duration for a record operation before stopping recording.</span></span> <span data-ttu-id="146e5-155">默认值 = 5 秒, 最小值 = 1 秒, 最大值 = 300 秒。</span><span class="sxs-lookup"><span data-stu-id="146e5-155">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="146e5-156">playBeep</span><span class="sxs-lookup"><span data-stu-id="146e5-156">playBeep</span></span>|<span data-ttu-id="146e5-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="146e5-157">Boolean</span></span>| <span data-ttu-id="146e5-158">如果为 true, 则会播放提示音, 指示用户可以开始记录其邮件。</span><span class="sxs-lookup"><span data-stu-id="146e5-158">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="146e5-159">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="146e5-159">Default = true.</span></span>|
|<span data-ttu-id="146e5-160">stopTones</span><span class="sxs-lookup"><span data-stu-id="146e5-160">stopTones</span></span>|<span data-ttu-id="146e5-161">String collection</span><span class="sxs-lookup"><span data-stu-id="146e5-161">String collection</span></span>|<span data-ttu-id="146e5-162">指定结束录音的停止音。</span><span class="sxs-lookup"><span data-stu-id="146e5-162">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="146e5-163">适用</span><span class="sxs-lookup"><span data-stu-id="146e5-163">clientContext</span></span>|<span data-ttu-id="146e5-164">String</span><span class="sxs-lookup"><span data-stu-id="146e5-164">String</span></span>|<span data-ttu-id="146e5-165">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="146e5-165">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="146e5-166">响应</span><span class="sxs-lookup"><span data-stu-id="146e5-166">Response</span></span>
<span data-ttu-id="146e5-167">此方法返回`200 OK`响应代码和位置标头, 其中包含为此请求创建的[commsOperation](../resources/commsoperation.md)的 URI。</span><span class="sxs-lookup"><span data-stu-id="146e5-167">This method returns a `200 OK` response code and a Location header with a URI to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="146e5-168">示例</span><span class="sxs-lookup"><span data-stu-id="146e5-168">Example</span></span>
<span data-ttu-id="146e5-169">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="146e5-169">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="146e5-170">请求</span><span class="sxs-lookup"><span data-stu-id="146e5-170">Request</span></span>
<span data-ttu-id="146e5-171">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="146e5-171">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="146e5-172">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="146e5-172">HTTP</span></span>](#tab/http)
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
  "stopTones": [ "#", "11", "*" ]
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="146e5-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="146e5-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-record-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="146e5-174">响应</span><span class="sxs-lookup"><span data-stu-id="146e5-174">Response</span></span>

> <span data-ttu-id="146e5-p111">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="146e5-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "status": "running",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}

```

##### <a name="notification---operation-completed"></a><span data-ttu-id="146e5-177">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="146e5-177">Notification - operation completed</span></span>

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
        "recordResourceLocation": "https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
        "recordResourceAccessToken": "<access-token>",
        "completionReason": "stopToneDetected"
      }
    }
  ]
}
```

##### <a name="get-recording-file---request"></a><span data-ttu-id="146e5-178">获取录制文件-请求</span><span class="sxs-lookup"><span data-stu-id="146e5-178">Get recording file - Request</span></span>
<span data-ttu-id="146e5-179">下面的示例展示了获取录制内容的请求。</span><span class="sxs-lookup"><span data-stu-id="146e5-179">The following example shows the request to get the content of the recording.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "download_recorded_file",
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="get-recording-file---response"></a><span data-ttu-id="146e5-180">获取录制文件-响应</span><span class="sxs-lookup"><span data-stu-id="146e5-180">Get recording file - Response</span></span>
<span data-ttu-id="146e5-181">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="146e5-181">Here is an example of the response.</span></span> 

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
