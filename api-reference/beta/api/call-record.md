---
title: call： record
description: 录制来自通话的短音频剪辑。 如果 bot 希望在出现提示后从呼叫者处捕获语音响应，这将非常有用。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2961bacfa9092aa580801e42e44aa1d2adbfaa97
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636699"
---
# <a name="call-record"></a><span data-ttu-id="355f6-104">call： record</span><span class="sxs-lookup"><span data-stu-id="355f6-104">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="355f6-105">从呼叫中录制简短的音频剪辑。</span><span class="sxs-lookup"><span data-stu-id="355f6-105">Record a short audio clip from a call.</span></span>
<span data-ttu-id="355f6-106">在收到响应提示后，bot 可以利用此程序从呼叫者处获取语音响应。</span><span class="sxs-lookup"><span data-stu-id="355f6-106">A bot can utilize this to capture a voice response from a caller after they are prompted for a response.</span></span>

<span data-ttu-id="355f6-107">有关如何处理操作的详细信息，请参阅[commsOperation](../resources/commsOperation.md)</span><span class="sxs-lookup"><span data-stu-id="355f6-107">For further information on how to handle operations, please review [commsOperation](../resources/commsOperation.md)</span></span>

><span data-ttu-id="355f6-108">**注意：** 只有使用[serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)启动的[调用](../resources/call.md)才支持这样做。</span><span class="sxs-lookup"><span data-stu-id="355f6-108">**Note:** This is only supported for [calls](../resources/call.md) which are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

<span data-ttu-id="355f6-109">此操作不用于记录整个调用。</span><span class="sxs-lookup"><span data-stu-id="355f6-109">This action is not intended to record the entire call.</span></span> <span data-ttu-id="355f6-110">录制的最大长度为5分钟。</span><span class="sxs-lookup"><span data-stu-id="355f6-110">The maximum length of recording is 5 minutes.</span></span> <span data-ttu-id="355f6-111">录制不会由云通信平台永久保存，并且在呼叫结束后不久将被丢弃。</span><span class="sxs-lookup"><span data-stu-id="355f6-111">The recording is not saved permanently by the by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="355f6-112">在录制操作完成后，bot 必须使用已完成的通知中提供的 recordingLocation 值立即下载录制。</span><span class="sxs-lookup"><span data-stu-id="355f6-112">The bot must download the recording promptly after the recording operation finishes by using the recordingLocation value that's given in the completed notification.</span></span>

><span data-ttu-id="355f6-113">**注意：** 任何收集的媒体都**不**会保留。</span><span class="sxs-lookup"><span data-stu-id="355f6-113">**Note:** Any media collected may **not** be persisted.</span></span> <span data-ttu-id="355f6-114">请确保在呼叫录音时遵守地区的法律和法规。</span><span class="sxs-lookup"><span data-stu-id="355f6-114">Make sure you are compliant with the laws and regulations of your area when it comes to call recording.</span></span> <span data-ttu-id="355f6-115">有关详细信息，请咨询法律顾问。</span><span class="sxs-lookup"><span data-stu-id="355f6-115">Please consult with a legal counsel for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="355f6-116">Permissions</span><span class="sxs-lookup"><span data-stu-id="355f6-116">Permissions</span></span>
<span data-ttu-id="355f6-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="355f6-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="355f6-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="355f6-119">Permission type</span></span> | <span data-ttu-id="355f6-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="355f6-120">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="355f6-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="355f6-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="355f6-122">不支持</span><span class="sxs-lookup"><span data-stu-id="355f6-122">Not Supported</span></span>        |
| <span data-ttu-id="355f6-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="355f6-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="355f6-124">不支持</span><span class="sxs-lookup"><span data-stu-id="355f6-124">Not Supported</span></span>        |
| <span data-ttu-id="355f6-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="355f6-125">Application</span></span>     | <span data-ttu-id="355f6-126">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="355f6-126">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="355f6-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="355f6-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /communications/calls/{id}/record
```
> <span data-ttu-id="355f6-128">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="355f6-128">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="355f6-129">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="355f6-129">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="355f6-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="355f6-130">Request headers</span></span>
| <span data-ttu-id="355f6-131">名称</span><span class="sxs-lookup"><span data-stu-id="355f6-131">Name</span></span>          | <span data-ttu-id="355f6-132">说明</span><span class="sxs-lookup"><span data-stu-id="355f6-132">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="355f6-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="355f6-133">Authorization</span></span> | <span data-ttu-id="355f6-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="355f6-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="355f6-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="355f6-136">Request body</span></span>
<span data-ttu-id="355f6-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="355f6-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="355f6-138">参数</span><span class="sxs-lookup"><span data-stu-id="355f6-138">Parameter</span></span>      | <span data-ttu-id="355f6-139">类型</span><span class="sxs-lookup"><span data-stu-id="355f6-139">Type</span></span>    |<span data-ttu-id="355f6-140">说明</span><span class="sxs-lookup"><span data-stu-id="355f6-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="355f6-141">提示</span><span class="sxs-lookup"><span data-stu-id="355f6-141">prompts</span></span>|<span data-ttu-id="355f6-142">[mediaPrompt](../resources/mediaprompt.md)集合</span><span class="sxs-lookup"><span data-stu-id="355f6-142">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="355f6-143">录制开始前要播放的提示集合（如果有）。</span><span class="sxs-lookup"><span data-stu-id="355f6-143">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="355f6-144">客户可以选择单独指定 "playPrompt" 操作，也可以指定为 "record" 的一部分-几乎所有记录都通过提示进行 preceeded。</span><span class="sxs-lookup"><span data-stu-id="355f6-144">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt.</span></span> <span data-ttu-id="355f6-145">当前支持仅作为集合的一部分的单个提示。</span><span class="sxs-lookup"><span data-stu-id="355f6-145">Current support is only for a single prompt as part of the collection.</span></span> |
|<span data-ttu-id="355f6-146">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="355f6-146">bargeInAllowed</span></span>|<span data-ttu-id="355f6-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="355f6-147">Boolean</span></span>| <span data-ttu-id="355f6-148">如果为 true，则此记录请求将 barge 到其他现有的排队/当前处理的 record/playprompt 请求中。</span><span class="sxs-lookup"><span data-stu-id="355f6-148">If true, this record request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="355f6-149">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="355f6-149">Default = false.</span></span> |
|<span data-ttu-id="355f6-150">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="355f6-150">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="355f6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="355f6-151">Int32</span></span>| <span data-ttu-id="355f6-152">在我们开始进行记录操作之前，可以从开始时开始的最大初始静音（用户无声），并使操作失败。</span><span class="sxs-lookup"><span data-stu-id="355f6-152">Maximum initial silence (user silence) allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="355f6-153">如果我们正在播放提示，则此计时器在提示完成后启动。</span><span class="sxs-lookup"><span data-stu-id="355f6-153">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="355f6-154">默认值 = 5 秒，最小值 = 1 秒，最大值 = 300 秒</span><span class="sxs-lookup"><span data-stu-id="355f6-154">Default = 5 seconds, Min = 1 second, Max = 300 seconds</span></span> |
|<span data-ttu-id="355f6-155">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="355f6-155">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="355f6-156">Int32</span><span class="sxs-lookup"><span data-stu-id="355f6-156">Int32</span></span>| <span data-ttu-id="355f6-157">用户开始发言后允许的最大静音（暂停）时间。</span><span class="sxs-lookup"><span data-stu-id="355f6-157">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="355f6-158">默认值 = 5 秒，最小值 = 1 秒，最大值 = 300 秒。</span><span class="sxs-lookup"><span data-stu-id="355f6-158">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="355f6-159">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="355f6-159">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="355f6-160">Int32</span><span class="sxs-lookup"><span data-stu-id="355f6-160">Int32</span></span>| <span data-ttu-id="355f6-161">停止录制前的记录操作的最长持续时间。</span><span class="sxs-lookup"><span data-stu-id="355f6-161">Max duration for a record operation before stopping recording.</span></span> <span data-ttu-id="355f6-162">默认值 = 5 秒，最小值 = 1 秒，最大值 = 300 秒。</span><span class="sxs-lookup"><span data-stu-id="355f6-162">Default = 5 seconds, Min = 1 second, Max = 300 seconds.</span></span>|
|<span data-ttu-id="355f6-163">playBeep</span><span class="sxs-lookup"><span data-stu-id="355f6-163">playBeep</span></span>|<span data-ttu-id="355f6-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="355f6-164">Boolean</span></span>| <span data-ttu-id="355f6-165">如果为 true，则会播放提示音，指示用户可以开始记录其邮件。</span><span class="sxs-lookup"><span data-stu-id="355f6-165">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="355f6-166">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="355f6-166">Default = true.</span></span>|
|<span data-ttu-id="355f6-167">stopTones</span><span class="sxs-lookup"><span data-stu-id="355f6-167">stopTones</span></span>|<span data-ttu-id="355f6-168">String collection</span><span class="sxs-lookup"><span data-stu-id="355f6-168">String collection</span></span>|<span data-ttu-id="355f6-169">指定结束录音的停止音。</span><span class="sxs-lookup"><span data-stu-id="355f6-169">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="355f6-170">适用</span><span class="sxs-lookup"><span data-stu-id="355f6-170">clientContext</span></span>|<span data-ttu-id="355f6-171">String</span><span class="sxs-lookup"><span data-stu-id="355f6-171">String</span></span>|<span data-ttu-id="355f6-172">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="355f6-172">Unique Client Context string.</span></span> <span data-ttu-id="355f6-173">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="355f6-173">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="355f6-174">响应</span><span class="sxs-lookup"><span data-stu-id="355f6-174">Response</span></span>
<span data-ttu-id="355f6-175">此方法返回`200 OK`响应代码和位置标头，其中包含为此请求创建的[recordOperation](../resources/recordoperation.md)的 URI。</span><span class="sxs-lookup"><span data-stu-id="355f6-175">This method returns a `200 OK` response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="355f6-176">示例</span><span class="sxs-lookup"><span data-stu-id="355f6-176">Example</span></span>
<span data-ttu-id="355f6-177">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="355f6-177">The following example shows how to call this API.</span></span>

### <a name="example-1-record-a-short-audio-clip-from-a-call"></a><span data-ttu-id="355f6-178">示例1：从呼叫中录制简短的音频剪辑</span><span class="sxs-lookup"><span data-stu-id="355f6-178">Example 1: Record a short audio clip from a call</span></span>

##### <a name="request"></a><span data-ttu-id="355f6-179">请求</span><span class="sxs-lookup"><span data-stu-id="355f6-179">Request</span></span>
<span data-ttu-id="355f6-180">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="355f6-180">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="355f6-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="355f6-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-record"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/record
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="355f6-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="355f6-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-record-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="355f6-183">响应</span><span class="sxs-lookup"><span data-stu-id="355f6-183">Response</span></span>
<span data-ttu-id="355f6-184">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="355f6-184">The following example shows the response.</span></span>

> <span data-ttu-id="355f6-p115">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="355f6-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="355f6-187">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="355f6-187">Notification - operation completed</span></span>

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

### <a name="example-2-retrieving-the-recording-file"></a><span data-ttu-id="355f6-188">示例2：检索录制文件</span><span class="sxs-lookup"><span data-stu-id="355f6-188">Example 2: Retrieving the recording file</span></span>

> <span data-ttu-id="355f6-189">**注意：** 虽然您可以提取并处理录制，但您**必须**在以后将其删除。</span><span class="sxs-lookup"><span data-stu-id="355f6-189">**Note:** While you're able to fetch the recording and process it, you **must** delete it afterwards.</span></span> <span data-ttu-id="355f6-190">无法持久化媒体。</span><span class="sxs-lookup"><span data-stu-id="355f6-190">Media cannot be persisted.</span></span>

##### <a name="request"></a><span data-ttu-id="355f6-191">请求</span><span class="sxs-lookup"><span data-stu-id="355f6-191">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a><span data-ttu-id="355f6-192">响应</span><span class="sxs-lookup"><span data-stu-id="355f6-192">Response</span></span>

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
