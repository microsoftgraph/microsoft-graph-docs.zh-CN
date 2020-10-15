---
title: 调用： recordResponse
description: 录制来自呼叫方的简短音频回复。 如果 bot 希望在出现提示后从呼叫者处捕获语音响应，这将非常有用。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: fa4fe6698d788ac8588101e6f818fdd70712c1fb
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461313"
---
# <a name="call-recordresponse"></a><span data-ttu-id="9ff0b-104">调用： recordResponse</span><span class="sxs-lookup"><span data-stu-id="9ff0b-104">call: recordResponse</span></span>

<span data-ttu-id="9ff0b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ff0b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9ff0b-106">录制来自呼叫方的简短音频回复。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-106">Records a short audio response from the caller.</span></span>
<span data-ttu-id="9ff0b-107">在收到响应提示后，bot 可以利用此程序从呼叫者处获取语音响应。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-107">A bot can utilize this to capture a voice response from a caller after they are prompted for a response.</span></span>

<span data-ttu-id="9ff0b-108">有关如何处理操作的详细信息，请参阅 [commsOperation](../resources/commsOperation.md)</span><span class="sxs-lookup"><span data-stu-id="9ff0b-108">For further information on how to handle operations, please review [commsOperation](../resources/commsOperation.md)</span></span>

><span data-ttu-id="9ff0b-109">**注意：** 只有使用[serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)启动的[调用](../resources/call.md)才支持这样做。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-109">**Note:** This is only supported for [calls](../resources/call.md) which are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

<span data-ttu-id="9ff0b-110">此操作不用于记录整个调用。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-110">This action is not intended to record the entire call.</span></span> <span data-ttu-id="9ff0b-111">录制的最大长度为2分钟。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-111">The maximum length of recording is 2 minutes.</span></span> <span data-ttu-id="9ff0b-112">该录制不会被云通信平台永久保存，并且在呼叫结束后不久将被丢弃。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-112">The recording is not saved permanently by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="9ff0b-113">在录制操作完成后，bot 必须使用已完成的通知中提供的 recordingLocation 值立即下载录制。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-113">The bot must download the recording promptly after the recording operation finishes by using the recordingLocation value that's given in the completed notification.</span></span>

><span data-ttu-id="9ff0b-114">**注意：** 任何收集的媒体都 **不** 会保留。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-114">**Note:** Any media collected may **not** be persisted.</span></span> <span data-ttu-id="9ff0b-115">请确保在呼叫录音时遵守地区的法律和法规。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-115">Make sure you are compliant with the laws and regulations of your area when it comes to call recording.</span></span> <span data-ttu-id="9ff0b-116">有关详细信息，请咨询法律顾问。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-116">Please consult with a legal counsel for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ff0b-117">Permissions</span><span class="sxs-lookup"><span data-stu-id="9ff0b-117">Permissions</span></span>
<span data-ttu-id="9ff0b-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9ff0b-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ff0b-120">Permission type</span></span> | <span data-ttu-id="9ff0b-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ff0b-121">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="9ff0b-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ff0b-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ff0b-123">不支持</span><span class="sxs-lookup"><span data-stu-id="9ff0b-123">Not Supported</span></span>        |
| <span data-ttu-id="9ff0b-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ff0b-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ff0b-125">不支持</span><span class="sxs-lookup"><span data-stu-id="9ff0b-125">Not Supported</span></span>        |
| <span data-ttu-id="9ff0b-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ff0b-126">Application</span></span>     | <span data-ttu-id="9ff0b-127">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="9ff0b-127">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="9ff0b-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ff0b-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/recordResponse
```

## <a name="request-headers"></a><span data-ttu-id="9ff0b-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ff0b-129">Request headers</span></span>
| <span data-ttu-id="9ff0b-130">名称</span><span class="sxs-lookup"><span data-stu-id="9ff0b-130">Name</span></span>          | <span data-ttu-id="9ff0b-131">说明</span><span class="sxs-lookup"><span data-stu-id="9ff0b-131">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9ff0b-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ff0b-132">Authorization</span></span> | <span data-ttu-id="9ff0b-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ff0b-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ff0b-135">Request body</span></span>
<span data-ttu-id="9ff0b-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9ff0b-137">参数</span><span class="sxs-lookup"><span data-stu-id="9ff0b-137">Parameter</span></span>      | <span data-ttu-id="9ff0b-138">类型</span><span class="sxs-lookup"><span data-stu-id="9ff0b-138">Type</span></span>    |<span data-ttu-id="9ff0b-139">Description</span><span class="sxs-lookup"><span data-stu-id="9ff0b-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ff0b-140">提示</span><span class="sxs-lookup"><span data-stu-id="9ff0b-140">prompts</span></span>|<span data-ttu-id="9ff0b-141">[mediaPrompt](../resources/mediaprompt.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ff0b-141">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="9ff0b-142">要播放的提示。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-142">The prompts to be played.</span></span> <span data-ttu-id="9ff0b-143">支持的最大 mediaPrompt 集合大小为1。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-143">The maximum supported mediaPrompt collection size is 1.</span></span>|
|<span data-ttu-id="9ff0b-144">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="9ff0b-144">bargeInAllowed</span></span>|<span data-ttu-id="9ff0b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ff0b-145">Boolean</span></span>| <span data-ttu-id="9ff0b-146">如果为 true，则 recordResponse 请求将 barge 到其他现有的排队/当前处理的 record/playprompt 请求中。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-146">If true, the recordResponse request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="9ff0b-147">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-147">Default = false.</span></span> |
|<span data-ttu-id="9ff0b-148">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="9ff0b-148">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="9ff0b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9ff0b-149">Int32</span></span>| <span data-ttu-id="9ff0b-150">最大初始静音 (用户静音) 允许在我们超时之前开始记录响应操作并使操作失败。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-150">Maximum initial silence (user silence) allowed from the time we start the record response operation before we timeout and fail the operation.</span></span> <span data-ttu-id="9ff0b-151">如果我们正在播放提示，则此计时器在提示完成后启动。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-151">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="9ff0b-152">默认值 = 5 秒，最小值 = 1 秒，最大值 = 120 秒</span><span class="sxs-lookup"><span data-stu-id="9ff0b-152">Default = 5 seconds, Min = 1 second, Max = 120 seconds</span></span> |
|<span data-ttu-id="9ff0b-153">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="9ff0b-153">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="9ff0b-154">Int32</span><span class="sxs-lookup"><span data-stu-id="9ff0b-154">Int32</span></span>| <span data-ttu-id="9ff0b-155">最大无声 (暂停用户开始发言后允许的) 时间。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-155">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="9ff0b-156">默认值 = 5 秒，最小值 = 1 秒，最大值 = 120 秒。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-156">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="9ff0b-157">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="9ff0b-157">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="9ff0b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9ff0b-158">Int32</span></span>| <span data-ttu-id="9ff0b-159">停止录制前的 recordResponse 操作的最长持续时间。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-159">Max duration for the recordResponse operation before stopping recording.</span></span> <span data-ttu-id="9ff0b-160">默认值 = 5 秒，最小值 = 1 秒，最大值 = 120 秒。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-160">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="9ff0b-161">playBeep</span><span class="sxs-lookup"><span data-stu-id="9ff0b-161">playBeep</span></span>|<span data-ttu-id="9ff0b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ff0b-162">Boolean</span></span>| <span data-ttu-id="9ff0b-163">如果为 true，则会播放提示音，指示用户可以开始记录其邮件。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-163">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="9ff0b-164">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-164">Default = true.</span></span>|
|<span data-ttu-id="9ff0b-165">stopTones</span><span class="sxs-lookup"><span data-stu-id="9ff0b-165">stopTones</span></span>|<span data-ttu-id="9ff0b-166">String 集合</span><span class="sxs-lookup"><span data-stu-id="9ff0b-166">String collection</span></span>|<span data-ttu-id="9ff0b-167">指定结束录音的停止音。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-167">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="9ff0b-168">适用</span><span class="sxs-lookup"><span data-stu-id="9ff0b-168">clientContext</span></span>|<span data-ttu-id="9ff0b-169">字符串</span><span class="sxs-lookup"><span data-stu-id="9ff0b-169">String</span></span>|<span data-ttu-id="9ff0b-170">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-170">Unique Client Context string.</span></span> <span data-ttu-id="9ff0b-171">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-171">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="9ff0b-172">响应</span><span class="sxs-lookup"><span data-stu-id="9ff0b-172">Response</span></span>
<span data-ttu-id="9ff0b-173">此方法返回 `200 OK` 响应代码和位置标头，其中包含为此请求创建的 [RECORDOPERATION](../resources/recordoperation.md) 的 URI。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-173">This method returns a `200 OK` response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="9ff0b-174">示例</span><span class="sxs-lookup"><span data-stu-id="9ff0b-174">Example</span></span>
<span data-ttu-id="9ff0b-175">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-175">The following example shows how to call this API.</span></span>

### <a name="example-1-records-a-short-audio-response-from-the-caller"></a><span data-ttu-id="9ff0b-176">示例1：记录来自呼叫者的短音频响应</span><span class="sxs-lookup"><span data-stu-id="9ff0b-176">Example 1: Records a short audio response from the caller</span></span>

##### <a name="request"></a><span data-ttu-id="9ff0b-177">请求</span><span class="sxs-lookup"><span data-stu-id="9ff0b-177">Request</span></span>
<span data-ttu-id="9ff0b-178">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-178">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9ff0b-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ff0b-179">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="9ff0b-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ff0b-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-recordresponse-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="9ff0b-181">C#</span><span class="sxs-lookup"><span data-stu-id="9ff0b-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-recordresponse-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ff0b-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ff0b-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-recordresponse-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ff0b-183">Java</span><span class="sxs-lookup"><span data-stu-id="9ff0b-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-recordresponse-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9ff0b-184">响应</span><span class="sxs-lookup"><span data-stu-id="9ff0b-184">Response</span></span>
<span data-ttu-id="9ff0b-185">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-185">The following example shows the response.</span></span>

> <span data-ttu-id="9ff0b-p114">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="9ff0b-188">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="9ff0b-188">Notification - operation completed</span></span>

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

### <a name="example-2-retrieving-the-recording-file"></a><span data-ttu-id="9ff0b-189">示例2：检索录制文件</span><span class="sxs-lookup"><span data-stu-id="9ff0b-189">Example 2: Retrieving the recording file</span></span>

><span data-ttu-id="9ff0b-190">**注意：** 您不能录制或以其他方式保留来自您的应用程序访问的呼叫或会议的媒体内容或从该媒体内容派生的数据。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-190">**Note:** You may NOT record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="9ff0b-191">请确保您符合有关通信的数据保护和机密性的法律和法规。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-191">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="9ff0b-192">有关详细信息，请参阅[使用条款](/legal/microsoft-apis/terms-of-use)并咨询法律顾问。</span><span class="sxs-lookup"><span data-stu-id="9ff0b-192">Please see the [Terms of Use](/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

##### <a name="request"></a><span data-ttu-id="9ff0b-193">请求</span><span class="sxs-lookup"><span data-stu-id="9ff0b-193">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a><span data-ttu-id="9ff0b-194">响应</span><span class="sxs-lookup"><span data-stu-id="9ff0b-194">Response</span></span>

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
