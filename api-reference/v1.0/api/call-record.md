---
title: call： recordResponse
description: 录制来自呼叫方的简短音频回复。 如果机器人希望按照提示从呼叫者捕获语音响应，这将非常有用。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8766f2764852354fc178c97bd632db550b183f81
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050582"
---
# <a name="call-recordresponse"></a><span data-ttu-id="158e2-104">call： recordResponse</span><span class="sxs-lookup"><span data-stu-id="158e2-104">call: recordResponse</span></span>

<span data-ttu-id="158e2-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="158e2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="158e2-106">录制来自呼叫方的简短音频回复。</span><span class="sxs-lookup"><span data-stu-id="158e2-106">Records a short audio response from the caller.</span></span>
<span data-ttu-id="158e2-107">机器人可以利用此功能在系统提示呼叫者做出响应后捕获来自呼叫者的语音响应。</span><span class="sxs-lookup"><span data-stu-id="158e2-107">A bot can utilize this to capture a voice response from a caller after they are prompted for a response.</span></span>

<span data-ttu-id="158e2-108">若要进一步了解如何处理操作，请查看 [commsOperation](../resources/commsOperation.md)</span><span class="sxs-lookup"><span data-stu-id="158e2-108">For further information on how to handle operations, please review [commsOperation](../resources/commsOperation.md)</span></span>

><span data-ttu-id="158e2-109">**注意：** 这仅 [支持通过](../resources/call.md)[serviceHostedMediaConfig 启动的呼叫](../resources/servicehostedmediaconfig.md)。</span><span class="sxs-lookup"><span data-stu-id="158e2-109">**Note:** This is only supported for [calls](../resources/call.md) which are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

<span data-ttu-id="158e2-110">此操作不用于记录整个呼叫。</span><span class="sxs-lookup"><span data-stu-id="158e2-110">This action is not intended to record the entire call.</span></span> <span data-ttu-id="158e2-111">录制的最大长度为 2 分钟。</span><span class="sxs-lookup"><span data-stu-id="158e2-111">The maximum length of recording is 2 minutes.</span></span> <span data-ttu-id="158e2-112">云通信平台不会永久保存录制，呼叫结束后将丢弃录制。</span><span class="sxs-lookup"><span data-stu-id="158e2-112">The recording is not saved permanently by the Cloud Communications Platform and is discarded shortly after the call ends.</span></span> <span data-ttu-id="158e2-113">录制操作完成后，自动程序必须使用已完成的通知中给出的 recordingLocation 值立即下载录制。</span><span class="sxs-lookup"><span data-stu-id="158e2-113">The bot must download the recording promptly after the recording operation finishes by using the recordingLocation value that's given in the completed notification.</span></span>

><span data-ttu-id="158e2-114">**注意：** 收集的任何媒体 **可能无法** 保留。</span><span class="sxs-lookup"><span data-stu-id="158e2-114">**Note:** Any media collected may **not** be persisted.</span></span> <span data-ttu-id="158e2-115">在呼叫录制方面，请确保你遵守你地区的法律和法规。</span><span class="sxs-lookup"><span data-stu-id="158e2-115">Make sure you are compliant with the laws and regulations of your area when it comes to call recording.</span></span> <span data-ttu-id="158e2-116">有关详细信息，请咨询法律顾问。</span><span class="sxs-lookup"><span data-stu-id="158e2-116">Please consult with a legal counsel for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="158e2-117">权限</span><span class="sxs-lookup"><span data-stu-id="158e2-117">Permissions</span></span>
<span data-ttu-id="158e2-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="158e2-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="158e2-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="158e2-120">Permission type</span></span> | <span data-ttu-id="158e2-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="158e2-121">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="158e2-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="158e2-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="158e2-123">不支持</span><span class="sxs-lookup"><span data-stu-id="158e2-123">Not Supported</span></span>        |
| <span data-ttu-id="158e2-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="158e2-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="158e2-125">不支持</span><span class="sxs-lookup"><span data-stu-id="158e2-125">Not Supported</span></span>        |
| <span data-ttu-id="158e2-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="158e2-126">Application</span></span>     | <span data-ttu-id="158e2-127">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="158e2-127">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="158e2-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="158e2-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/recordResponse
```

## <a name="request-headers"></a><span data-ttu-id="158e2-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="158e2-129">Request headers</span></span>
| <span data-ttu-id="158e2-130">名称</span><span class="sxs-lookup"><span data-stu-id="158e2-130">Name</span></span>          | <span data-ttu-id="158e2-131">说明</span><span class="sxs-lookup"><span data-stu-id="158e2-131">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="158e2-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="158e2-132">Authorization</span></span> | <span data-ttu-id="158e2-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="158e2-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="158e2-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="158e2-135">Request body</span></span>
<span data-ttu-id="158e2-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="158e2-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="158e2-137">参数</span><span class="sxs-lookup"><span data-stu-id="158e2-137">Parameter</span></span>      | <span data-ttu-id="158e2-138">类型</span><span class="sxs-lookup"><span data-stu-id="158e2-138">Type</span></span>    |<span data-ttu-id="158e2-139">说明</span><span class="sxs-lookup"><span data-stu-id="158e2-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="158e2-140">prompts</span><span class="sxs-lookup"><span data-stu-id="158e2-140">prompts</span></span>|<span data-ttu-id="158e2-141">[mediaPrompt](../resources/mediaprompt.md) 集合</span><span class="sxs-lookup"><span data-stu-id="158e2-141">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="158e2-142">要播放的提示。</span><span class="sxs-lookup"><span data-stu-id="158e2-142">The prompts to be played.</span></span> <span data-ttu-id="158e2-143">支持的最大 mediaPrompt 集合大小为 1。</span><span class="sxs-lookup"><span data-stu-id="158e2-143">The maximum supported mediaPrompt collection size is 1.</span></span>|
|<span data-ttu-id="158e2-144">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="158e2-144">bargeInAllowed</span></span>|<span data-ttu-id="158e2-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="158e2-145">Boolean</span></span>| <span data-ttu-id="158e2-146">如果为 true，recordResponse 请求将插入其他现有的排队向上/当前处理的记录/playprompt 请求。</span><span class="sxs-lookup"><span data-stu-id="158e2-146">If true, the recordResponse request will barge into other existing queued-up/currently-processing record/playprompt requests.</span></span> <span data-ttu-id="158e2-147">默认值 = false。</span><span class="sxs-lookup"><span data-stu-id="158e2-147">Default = false.</span></span> |
|<span data-ttu-id="158e2-148">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="158e2-148">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="158e2-149">Int32</span><span class="sxs-lookup"><span data-stu-id="158e2-149">Int32</span></span>| <span data-ttu-id="158e2-150">在超时 (失败) ，从开始记录响应操作时，用户的最大初始静默表示用户静默。</span><span class="sxs-lookup"><span data-stu-id="158e2-150">Maximum initial silence (user silence) allowed from the time we start the record response operation before we timeout and fail the operation.</span></span> <span data-ttu-id="158e2-151">如果播放提示，则此计时器在提示完成后启动。</span><span class="sxs-lookup"><span data-stu-id="158e2-151">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> <span data-ttu-id="158e2-152">默认值 = 5 秒，最小值 = 1 秒，最大值 = 120 秒</span><span class="sxs-lookup"><span data-stu-id="158e2-152">Default = 5 seconds, Min = 1 second, Max = 120 seconds</span></span> |
|<span data-ttu-id="158e2-153">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="158e2-153">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="158e2-154">Int32</span><span class="sxs-lookup"><span data-stu-id="158e2-154">Int32</span></span>| <span data-ttu-id="158e2-155">用户开始 (后) 允许的最大静默时间。</span><span class="sxs-lookup"><span data-stu-id="158e2-155">Maximum silence (pause) time allowed after a user has started speaking.</span></span> <span data-ttu-id="158e2-156">默认值 = 5 秒，最小值 = 1 秒，最大值 = 120 秒。</span><span class="sxs-lookup"><span data-stu-id="158e2-156">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="158e2-157">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="158e2-157">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="158e2-158">Int32</span><span class="sxs-lookup"><span data-stu-id="158e2-158">Int32</span></span>| <span data-ttu-id="158e2-159">在停止录制之前，recordResponse 操作的最大持续时间。</span><span class="sxs-lookup"><span data-stu-id="158e2-159">Max duration for the recordResponse operation before stopping recording.</span></span> <span data-ttu-id="158e2-160">默认值 = 5 秒，最小值 = 1 秒，最大值 = 120 秒。</span><span class="sxs-lookup"><span data-stu-id="158e2-160">Default = 5 seconds, Min = 1 second, Max = 120 seconds.</span></span>|
|<span data-ttu-id="158e2-161">playBeep</span><span class="sxs-lookup"><span data-stu-id="158e2-161">playBeep</span></span>|<span data-ttu-id="158e2-162">布尔值</span><span class="sxs-lookup"><span data-stu-id="158e2-162">Boolean</span></span>| <span data-ttu-id="158e2-163">如果为 true，则播放一个嘟嘟声，以向用户指示他们可以开始录制其消息。</span><span class="sxs-lookup"><span data-stu-id="158e2-163">If true, plays a beep to indicate to the user that they can start recording their message.</span></span> <span data-ttu-id="158e2-164">默认值 = true。</span><span class="sxs-lookup"><span data-stu-id="158e2-164">Default = true.</span></span>|
|<span data-ttu-id="158e2-165">stopTones</span><span class="sxs-lookup"><span data-stu-id="158e2-165">stopTones</span></span>|<span data-ttu-id="158e2-166">字符串集合</span><span class="sxs-lookup"><span data-stu-id="158e2-166">String collection</span></span>|<span data-ttu-id="158e2-167">结束录制指定的停止音调。</span><span class="sxs-lookup"><span data-stu-id="158e2-167">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="158e2-168">clientContext</span><span class="sxs-lookup"><span data-stu-id="158e2-168">clientContext</span></span>|<span data-ttu-id="158e2-169">String</span><span class="sxs-lookup"><span data-stu-id="158e2-169">String</span></span>|<span data-ttu-id="158e2-170">唯一的客户端上下文字符串。</span><span class="sxs-lookup"><span data-stu-id="158e2-170">Unique Client Context string.</span></span> <span data-ttu-id="158e2-171">最大限制为 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="158e2-171">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="158e2-172">响应</span><span class="sxs-lookup"><span data-stu-id="158e2-172">Response</span></span>
<span data-ttu-id="158e2-173">此方法将响应代码和 Location 标头的 URI 返回到为此请求 `200 OK` 创建的[recordOperation。](../resources/recordoperation.md)</span><span class="sxs-lookup"><span data-stu-id="158e2-173">This method returns a `200 OK` response code and a Location header with a URI to the [recordOperation](../resources/recordoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="158e2-174">示例</span><span class="sxs-lookup"><span data-stu-id="158e2-174">Example</span></span>
<span data-ttu-id="158e2-175">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="158e2-175">The following example shows how to call this API.</span></span>

### <a name="example-1-records-a-short-audio-response-from-the-caller"></a><span data-ttu-id="158e2-176">示例 1：录制来自呼叫者的简短音频响应</span><span class="sxs-lookup"><span data-stu-id="158e2-176">Example 1: Records a short audio response from the caller</span></span>

##### <a name="request"></a><span data-ttu-id="158e2-177">请求</span><span class="sxs-lookup"><span data-stu-id="158e2-177">Request</span></span>
<span data-ttu-id="158e2-178">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="158e2-178">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="158e2-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="158e2-179">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="158e2-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="158e2-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-recordresponse-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="158e2-181">C#</span><span class="sxs-lookup"><span data-stu-id="158e2-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-recordresponse-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="158e2-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="158e2-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-recordresponse-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="158e2-183">Java</span><span class="sxs-lookup"><span data-stu-id="158e2-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-recordresponse-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="158e2-184">响应</span><span class="sxs-lookup"><span data-stu-id="158e2-184">Response</span></span>
<span data-ttu-id="158e2-185">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="158e2-185">The following example shows the response.</span></span>

> <span data-ttu-id="158e2-186">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="158e2-186">**Note:** The response object shown here might be shortened for readability.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="158e2-187">通知 - 操作已完成</span><span class="sxs-lookup"><span data-stu-id="158e2-187">Notification - operation completed</span></span>

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

### <a name="example-2-retrieving-the-recording-file"></a><span data-ttu-id="158e2-188">示例 2：检索录制文件</span><span class="sxs-lookup"><span data-stu-id="158e2-188">Example 2: Retrieving the recording file</span></span>

><span data-ttu-id="158e2-189">**注意：** You may NOT record or otherwise persist media content from calls or meetings that your application accesses， or data derived from that media content.</span><span class="sxs-lookup"><span data-stu-id="158e2-189">**Note:** You may NOT record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="158e2-190">确保你遵守有关通信数据保护和机密性的法律和法规。</span><span class="sxs-lookup"><span data-stu-id="158e2-190">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="158e2-191">有关详细信息，请参阅[使用条款](/legal/microsoft-apis/terms-of-use)并咨询法律顾问。</span><span class="sxs-lookup"><span data-stu-id="158e2-191">Please see the [Terms of Use](/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

##### <a name="request"></a><span data-ttu-id="158e2-192">请求</span><span class="sxs-lookup"><span data-stu-id="158e2-192">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Authorization: Bearer <recordingAccessToken>
```

##### <a name="response"></a><span data-ttu-id="158e2-193">响应</span><span class="sxs-lookup"><span data-stu-id="158e2-193">Response</span></span>

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
