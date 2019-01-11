---
title: 呼叫： 记录
description: 记录呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: afb74bb656eb6fcc09fdab71477843748bc5616d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859575"
---
# <a name="call-record"></a><span data-ttu-id="76429-103">呼叫： 记录</span><span class="sxs-lookup"><span data-stu-id="76429-103">call: record</span></span>

> <span data-ttu-id="76429-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="76429-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76429-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="76429-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76429-106">记录呼叫。</span><span class="sxs-lookup"><span data-stu-id="76429-106">Record the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="76429-107">权限</span><span class="sxs-lookup"><span data-stu-id="76429-107">Permissions</span></span>
<span data-ttu-id="76429-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76429-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76429-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="76429-110">Permission type</span></span> | <span data-ttu-id="76429-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76429-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="76429-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76429-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="76429-113">不支持</span><span class="sxs-lookup"><span data-stu-id="76429-113">Not Supported</span></span>        |
| <span data-ttu-id="76429-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76429-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76429-115">不支持</span><span class="sxs-lookup"><span data-stu-id="76429-115">Not Supported</span></span>        |
| <span data-ttu-id="76429-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="76429-116">Application</span></span>     | <span data-ttu-id="76429-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="76429-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="76429-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76429-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="76429-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="76429-119">Request headers</span></span>
| <span data-ttu-id="76429-120">名称</span><span class="sxs-lookup"><span data-stu-id="76429-120">Name</span></span>          | <span data-ttu-id="76429-121">说明</span><span class="sxs-lookup"><span data-stu-id="76429-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="76429-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="76429-122">Authorization</span></span> | <span data-ttu-id="76429-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="76429-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76429-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="76429-125">Request body</span></span>
<span data-ttu-id="76429-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="76429-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="76429-127">参数</span><span class="sxs-lookup"><span data-stu-id="76429-127">Parameter</span></span>      | <span data-ttu-id="76429-128">类型</span><span class="sxs-lookup"><span data-stu-id="76429-128">Type</span></span>    |<span data-ttu-id="76429-129">Description</span><span class="sxs-lookup"><span data-stu-id="76429-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76429-130">提示</span><span class="sxs-lookup"><span data-stu-id="76429-130">prompts</span></span>|<span data-ttu-id="76429-131">[mediaprompt](../resources/mediaprompt.md)集合</span><span class="sxs-lookup"><span data-stu-id="76429-131">[mediaprompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="76429-132">启动提示之前录制播放 （如果有） 的集合。</span><span class="sxs-lookup"><span data-stu-id="76429-132">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="76429-133">客户可以选择单独指定"playPrompt"操作，或者指定的"记录"的一部分主要的所有记录都都使用提示</span><span class="sxs-lookup"><span data-stu-id="76429-133">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt</span></span> |
|<span data-ttu-id="76429-134">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="76429-134">bargeInAllowed</span></span>|<span data-ttu-id="76429-135">布尔</span><span class="sxs-lookup"><span data-stu-id="76429-135">Boolean</span></span>| <span data-ttu-id="76429-136">允许用户提示完成之前输入的选择。</span><span class="sxs-lookup"><span data-stu-id="76429-136">Allow users to enter choice before prompt finishes.</span></span>                                                                 |
|<span data-ttu-id="76429-137">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="76429-137">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="76429-138">Int32</span><span class="sxs-lookup"><span data-stu-id="76429-138">Int32</span></span>| <span data-ttu-id="76429-139">从我们开始之前我们记录操作超时和失败操作的时间允许的最大初始静音。</span><span class="sxs-lookup"><span data-stu-id="76429-139">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="76429-140">如果我们播放提示时，提示完成后从开始此计时器。</span><span class="sxs-lookup"><span data-stu-id="76429-140">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> |
|<span data-ttu-id="76429-141">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="76429-141">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="76429-142">Int32</span><span class="sxs-lookup"><span data-stu-id="76429-142">Int32</span></span>| <span data-ttu-id="76429-143">最大无声超时秒数。</span><span class="sxs-lookup"><span data-stu-id="76429-143">The maximum silence timeout in seconds.</span></span>|
|<span data-ttu-id="76429-144">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="76429-144">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="76429-145">Int32</span><span class="sxs-lookup"><span data-stu-id="76429-145">Int32</span></span>| <span data-ttu-id="76429-146">最大记录持续时间，以秒为单位。</span><span class="sxs-lookup"><span data-stu-id="76429-146">The maximum record duration in seconds.</span></span>|
|<span data-ttu-id="76429-147">playBeep</span><span class="sxs-lookup"><span data-stu-id="76429-147">playBeep</span></span>|<span data-ttu-id="76429-148">布尔</span><span class="sxs-lookup"><span data-stu-id="76429-148">Boolean</span></span>| <span data-ttu-id="76429-149">播放提示音后播放提示。</span><span class="sxs-lookup"><span data-stu-id="76429-149">Plays a beep after playing the prompt.</span></span>|
|<span data-ttu-id="76429-150">streamWhileRecording</span><span class="sxs-lookup"><span data-stu-id="76429-150">streamWhileRecording</span></span>|<span data-ttu-id="76429-151">布尔</span><span class="sxs-lookup"><span data-stu-id="76429-151">Boolean</span></span>|<span data-ttu-id="76429-152">如果设置为 true，资源位置将提供一旦开始录制。</span><span class="sxs-lookup"><span data-stu-id="76429-152">If set to true, a resource location will be provided as soon as the recording starts.</span></span> |
|<span data-ttu-id="76429-153">stopTones</span><span class="sxs-lookup"><span data-stu-id="76429-153">stopTones</span></span>|<span data-ttu-id="76429-154">String 集合</span><span class="sxs-lookup"><span data-stu-id="76429-154">String collection</span></span>|<span data-ttu-id="76429-155">停止指定结束录制音。</span><span class="sxs-lookup"><span data-stu-id="76429-155">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="76429-156">clientContext</span><span class="sxs-lookup"><span data-stu-id="76429-156">clientContext</span></span>|<span data-ttu-id="76429-157">字符串</span><span class="sxs-lookup"><span data-stu-id="76429-157">String</span></span>|<span data-ttu-id="76429-158">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="76429-158">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="76429-159">响应</span><span class="sxs-lookup"><span data-stu-id="76429-159">Response</span></span>
<span data-ttu-id="76429-160">返回`202 Accepted`响应代码和具有[commsOperation](../resources/commsoperation.md)创建的此请求 uri 中的位置标头。</span><span class="sxs-lookup"><span data-stu-id="76429-160">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="76429-161">示例</span><span class="sxs-lookup"><span data-stu-id="76429-161">Example</span></span>
<span data-ttu-id="76429-162">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="76429-162">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="76429-163">请求</span><span class="sxs-lookup"><span data-stu-id="76429-163">Request</span></span>
<span data-ttu-id="76429-164">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="76429-164">The following example shows the request.</span></span>

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
      },
      "loop": 5
    }
  ],
  "maxRecordDurationInSeconds": 1800,
  "initialSilenceTimeoutInSeconds": 10,
  "maxSilenceTimeoutInSeconds": 2,
  "recordingFormat": "wav",
  "playBeep": true,
  "streamWhileRecording": true,
  "stopTones": [ "#", "11", "*" ]
}
```

##### <a name="response"></a><span data-ttu-id="76429-165">响应</span><span class="sxs-lookup"><span data-stu-id="76429-165">Response</span></span>

> <span data-ttu-id="76429-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="76429-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="76429-168">通知-完成的操作</span><span class="sxs-lookup"><span data-stu-id="76429-168">Notification - operation completed</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: record",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
