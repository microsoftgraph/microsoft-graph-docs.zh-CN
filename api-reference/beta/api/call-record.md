---
title: 调用： recordResponse
description: 记录来自呼叫者的简短音频响应。 如果 bot 希望在发出提示后从呼叫者处捕获语音响应，这将非常有用。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: af5d50c5d8e2422625d4ca10c7d87c8689bb8a68
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681580"
---
# <a name="call-recordresponse"></a><span data-ttu-id="24bd0-104">调用： recordResponse</span><span class="sxs-lookup"><span data-stu-id="24bd0-104">call: recordResponse</span></span>

<span data-ttu-id="24bd0-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24bd0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24bd0-106">记录来自呼叫者的简短音频响应。</span><span class="sxs-lookup"><span data-stu-id="24bd0-106">Record a short audio response from the caller.</span></span>

<span data-ttu-id="24bd0-107">在收到响应提示后，bot 可以使用此程序从呼叫者处捕获语音响应。</span><span class="sxs-lookup"><span data-stu-id="24bd0-107">A bot can use this to capture a voice response from a caller after they are prompted for a response.</span></span>

<span data-ttu-id="24bd0-108">有关如何处理操作的详细信息，请参阅[commsOperation](../resources/commsOperation.md)</span><span class="sxs-lookup"><span data-stu-id="24bd0-108">For more information about how to handle operations, see [commsOperation](../resources/commsOperation.md)</span></span>

><span data-ttu-id="24bd0-109">**注意：** 仅使用[serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)启动的[调用](../resources/call.md)支持此 API。</span><span class="sxs-lookup"><span data-stu-id="24bd0-109">**Note:** This API is only supported for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

<span data-ttu-id="24bd0-110">此操作不用于记录整个调用。</span><span class="sxs-lookup"><span data-stu-id="24bd0-110">This action is not intended to record the entire call.</span></span> <span data-ttu-id="24bd0-111">录制的最大长度为2分钟。</span><span class="sxs-lookup"><span data-stu-id="24bd0-111">The maximum length of recording is 2 minutes.</span></span> <span data-ttu-id="24bd0-112">录制不会由云通信平台永久保存，并且在呼叫结束后不久将被丢弃。</span><span class="sxs-lookup"><span data-stu-id="24bd0-112">The recording is not saved permanently by the by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="24bd0-113">在录制操作完成后，bot 必须使用已完成的通知中提供的 recordingLocation 值立即下载录制。</span><span class="sxs-lookup"><span data-stu-id="24bd0-113">The bot must download the recording promptly after the recording operation finishes by using the recordingLocation value that's given in the completed notification.</span></span>

><span data-ttu-id="24bd0-114">**注意：** 您不能录制或以其他方式保留来自您的应用程序访问的呼叫或会议的媒体内容或从该媒体内容派生的数据。</span><span class="sxs-lookup"><span data-stu-id="24bd0-114">**Note:** You may not record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="24bd0-115">请确保您符合有关通信的数据保护和机密性的法律和法规。</span><span class="sxs-lookup"><span data-stu-id="24bd0-115">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="24bd0-116">有关详细信息，请参阅[使用条款](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use)并咨询法律顾问。</span><span class="sxs-lookup"><span data-stu-id="24bd0-116">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="24bd0-117">Permissions</span><span class="sxs-lookup"><span data-stu-id="24bd0-117">Permissions</span></span>
<span data-ttu-id="24bd0-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24bd0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24bd0-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="24bd0-120">Permission type</span></span> | <span data-ttu-id="24bd0-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24bd0-121">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="24bd0-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24bd0-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="24bd0-123">不支持</span><span class="sxs-lookup"><span data-stu-id="24bd0-123">Not Supported</span></span>        |
| <span data-ttu-id="24bd0-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24bd0-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24bd0-125">不支持</span><span class="sxs-lookup"><span data-stu-id="24bd0-125">Not Supported</span></span>        |
| <span data-ttu-id="24bd0-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="24bd0-126">Application</span></span>     | <span data-ttu-id="24bd0-127">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="24bd0-127">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="24bd0-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24bd0-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/recordResponse
POST /communications/calls/{id}/recordResponse
```
> <span data-ttu-id="24bd0-129">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="24bd0-129">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="24bd0-130">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="24bd0-130">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24bd0-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="24bd0-131">Request headers</span></span>
| <span data-ttu-id="24bd0-132">名称</span><span class="sxs-lookup"><span data-stu-id="24bd0-132">Name</span></span>          | <span data-ttu-id="24bd0-133">说明</span><span class="sxs-lookup"><span data-stu-id="24bd0-133">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="24bd0-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="24bd0-134">Authorization</span></span> | <span data-ttu-id="24bd0-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="24bd0-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24bd0-137">Content-type</span><span class="sxs-lookup"><span data-stu-id="24bd0-137">Content-type</span></span>| <span data-ttu-id="24bd0-p107">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="24bd0-p107">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24bd0-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="24bd0-140">Request body</span></span>
<span data-ttu-id="24bd0-141">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="24bd0-141">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="24bd0-142">参数</span><span class="sxs-lookup"><span data-stu-id="24bd0-142">Parameter</span></span>      | <span data-ttu-id="24bd0-143">类型</span><span class="sxs-lookup"><span data-stu-id="24bd0-143">Type</span></span>    |<span data-ttu-id="24bd0-144">Description</span><span class="sxs-lookup"><span data-stu-id="24bd0-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24bd0-145">提示</span><span class="sxs-lookup"><span data-stu-id="24bd0-145">prompts</span></span>|<span data-ttu-id="24bd0-146">[MediaPrompt](../resources/mediaprompt.md)集合</span><span class="sxs-lookup"><span data-stu-id="24bd0-146">[MediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="24bd0-147">要播放的提示。</span><span class="sxs-lookup"><span data-stu-id="24bd0-147">The prompts to be played.</span></span> <span data-ttu-id="24bd0-148">支持的最大 mediaPrompt 集合大小为1。</span><span class="sxs-lookup"><span data-stu-id="24bd0-148">The maximum supported mediaPrompt collection size is 1.</span></span>|
|<span data-ttu-id="24bd0-149">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="24bd0-149">bargeInAllowed</span></span>|<span data-ttu-id="24bd0-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="24bd0-150">Boolean</span></span>| <span data-ttu-id="24bd0-151">如果为 true，则 recordResponse 请求将 barge 到其他现有的排队/当前处理的 record/playprompt 请求中。</span><span class="sxs-lookup"><span data-stu-id="24bd0-151">If true, the recordResponse request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="24bd0-152">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="24bd0-152">Default = false.</span></span> |
|<span data-ttu-id="24bd0-153">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="24bd0-153">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="24bd0-154">Int32</span><span class="sxs-lookup"><span data-stu-id="24bd0-154">Int32</span></span>| <span data-ttu-id="24bd0-155">在我们开始进行记录响应操作并使操作失败之前，允许的最大初始静音（用户静默）。</span><span class="sxs-lookup"><span data-stu-id="24bd0-155">Maximum initial silence (user silence) allowed from the time we start the record response operation before we timeout and fail the operation.</span></span> <span data-ttu-id="24bd0-156">如果我们正在播放提示，则此计时器在提示完成后启动。</span><span class="sxs-lookup"><span data-stu-id="24bd0-156">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="24bd0-157">默认值 = 5 秒，最小值 = 1 秒，最大值 = 120 秒</span><span class="sxs-lookup"><span data-stu-id="24bd0-157">Default = 5 seconds, Min = 1 second, Max = 120 seconds</span></span> |
|<span data-ttu-id="24bd0-158">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="24bd0-158">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="24bd0-159">Int32</span><span class="sxs-lookup"><span data-stu-id="24bd0-159">Int32</span></span>| <span data-ttu-id="24bd0-160">用户开始发言后允许的最大静音（暂停）时间。</span><span class="sxs-lookup"><span data-stu-id="24bd0-160">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="24bd0-161">默认值 = 5 秒，最小值 = 1 秒，最大值 = 120 秒。</span><span class="sxs-lookup"><span data-stu-id="24bd0-161">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="24bd0-162">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="24bd0-162">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="24bd0-163">Int32</span><span class="sxs-lookup"><span data-stu-id="24bd0-163">Int32</span></span>| <span data-ttu-id="24bd0-164">停止录制前的 recordResponse 操作的最长持续时间。</span><span class="sxs-lookup"><span data-stu-id="24bd0-164">Max duration for the recordResponse operation before stopping recording.</span></span> <span data-ttu-id="24bd0-165">默认值 = 5 秒，最小值 = 1 秒，最大值 = 120 秒。</span><span class="sxs-lookup"><span data-stu-id="24bd0-165">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="24bd0-166">playBeep</span><span class="sxs-lookup"><span data-stu-id="24bd0-166">playBeep</span></span>|<span data-ttu-id="24bd0-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="24bd0-167">Boolean</span></span>| <span data-ttu-id="24bd0-168">如果为 true，则会播放提示音，指示用户可以开始记录其邮件。</span><span class="sxs-lookup"><span data-stu-id="24bd0-168">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="24bd0-169">默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="24bd0-169">Default = true.</span></span>|
|<span data-ttu-id="24bd0-170">stopTones</span><span class="sxs-lookup"><span data-stu-id="24bd0-170">stopTones</span></span>|<span data-ttu-id="24bd0-171">String collection</span><span class="sxs-lookup"><span data-stu-id="24bd0-171">String collection</span></span>|<span data-ttu-id="24bd0-172">指定结束录音的停止音。</span><span class="sxs-lookup"><span data-stu-id="24bd0-172">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="24bd0-173">适用</span><span class="sxs-lookup"><span data-stu-id="24bd0-173">clientContext</span></span>|<span data-ttu-id="24bd0-174">String</span><span class="sxs-lookup"><span data-stu-id="24bd0-174">String</span></span>|<span data-ttu-id="24bd0-175">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="24bd0-175">Unique Client Context string.</span></span> <span data-ttu-id="24bd0-176">最大限制为256个字符。</span><span class="sxs-lookup"><span data-stu-id="24bd0-176">Max limit is 256 chars.</span></span>|

> <span data-ttu-id="24bd0-177">**注意：** 最长录制时间从5分钟减少到2分钟。</span><span class="sxs-lookup"><span data-stu-id="24bd0-177">**Note:** The maximum recording time has been reduced from 5 minutes to 2 minutes.</span></span>

## <a name="response"></a><span data-ttu-id="24bd0-178">响应</span><span class="sxs-lookup"><span data-stu-id="24bd0-178">Response</span></span>
<span data-ttu-id="24bd0-179">此方法返回一个 `200 OK` HTTP 响应代码和一个位置标头，其中包含为此请求创建的[RECORDOPERATION](../resources/recordoperation.md)的 URI。</span><span class="sxs-lookup"><span data-stu-id="24bd0-179">This method returns a `200 OK` HTTP response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="24bd0-180">示例</span><span class="sxs-lookup"><span data-stu-id="24bd0-180">Example</span></span>
<span data-ttu-id="24bd0-181">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="24bd0-181">The following example shows how to call this API.</span></span>

### <a name="example-1-records-a-short-audio-response-from-the-caller"></a><span data-ttu-id="24bd0-182">示例1：记录来自呼叫者的短音频响应</span><span class="sxs-lookup"><span data-stu-id="24bd0-182">Example 1: Records a short audio response from the caller</span></span>

##### <a name="request"></a><span data-ttu-id="24bd0-183">请求</span><span class="sxs-lookup"><span data-stu-id="24bd0-183">Request</span></span>
<span data-ttu-id="24bd0-184">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="24bd0-184">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="24bd0-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="24bd0-185">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="24bd0-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24bd0-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-recordresponse-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="24bd0-187">C#</span><span class="sxs-lookup"><span data-stu-id="24bd0-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-recordresponse-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24bd0-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24bd0-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-recordresponse-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="24bd0-189">响应</span><span class="sxs-lookup"><span data-stu-id="24bd0-189">Response</span></span>
<span data-ttu-id="24bd0-190">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="24bd0-190">The following example shows the response.</span></span>

> <span data-ttu-id="24bd0-p115">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="24bd0-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="24bd0-193">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="24bd0-193">Notification - operation completed</span></span>

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

### <a name="example-2-retrieving-the-recording-file"></a><span data-ttu-id="24bd0-194">示例2：检索录制文件</span><span class="sxs-lookup"><span data-stu-id="24bd0-194">Example 2: Retrieving the recording file</span></span>

> <span data-ttu-id="24bd0-195">**注意：** 您不能录制或以其他方式保留来自您的应用程序访问的呼叫或会议的媒体内容或从该媒体内容派生的数据。</span><span class="sxs-lookup"><span data-stu-id="24bd0-195">**Note:** You may NOT record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="24bd0-196">请确保您符合有关通信的数据保护和机密性的法律和法规。</span><span class="sxs-lookup"><span data-stu-id="24bd0-196">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="24bd0-197">有关详细信息，请参阅[使用条款](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use)并咨询法律顾问。</span><span class="sxs-lookup"><span data-stu-id="24bd0-197">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

##### <a name="request"></a><span data-ttu-id="24bd0-198">请求</span><span class="sxs-lookup"><span data-stu-id="24bd0-198">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a><span data-ttu-id="24bd0-199">响应</span><span class="sxs-lookup"><span data-stu-id="24bd0-199">Response</span></span>

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

> <span data-ttu-id="24bd0-200">**注意：** 您不能录制或以其他方式保留来自您的应用程序访问的呼叫或会议的媒体内容或从该媒体内容派生的数据。</span><span class="sxs-lookup"><span data-stu-id="24bd0-200">**Note:** You may NOT record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="24bd0-201">请确保您符合有关通信的数据保护和机密性的法律和法规。</span><span class="sxs-lookup"><span data-stu-id="24bd0-201">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="24bd0-202">有关详细信息，请参阅[使用条款](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use)并咨询法律顾问。</span><span class="sxs-lookup"><span data-stu-id="24bd0-202">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

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
