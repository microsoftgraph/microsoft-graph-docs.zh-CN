---
title: 'call: record'
description: 录制呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fad06769f81b9840b89a43cf3e759c86454edef0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438627"
---
# <a name="call-record"></a><span data-ttu-id="882d2-103">call: record</span><span class="sxs-lookup"><span data-stu-id="882d2-103">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="882d2-104">录制呼叫。</span><span class="sxs-lookup"><span data-stu-id="882d2-104">Record the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="882d2-105">权限</span><span class="sxs-lookup"><span data-stu-id="882d2-105">Permissions</span></span>
<span data-ttu-id="882d2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="882d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="882d2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="882d2-108">Permission type</span></span> | <span data-ttu-id="882d2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="882d2-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="882d2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="882d2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="882d2-111">不支持</span><span class="sxs-lookup"><span data-stu-id="882d2-111">Not Supported</span></span>        |
| <span data-ttu-id="882d2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="882d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="882d2-113">不支持</span><span class="sxs-lookup"><span data-stu-id="882d2-113">Not Supported</span></span>        |
| <span data-ttu-id="882d2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="882d2-114">Application</span></span>     | <span data-ttu-id="882d2-115">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="882d2-115">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="882d2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="882d2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="882d2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="882d2-117">Request headers</span></span>
| <span data-ttu-id="882d2-118">名称</span><span class="sxs-lookup"><span data-stu-id="882d2-118">Name</span></span>          | <span data-ttu-id="882d2-119">说明</span><span class="sxs-lookup"><span data-stu-id="882d2-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="882d2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="882d2-120">Authorization</span></span> | <span data-ttu-id="882d2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="882d2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="882d2-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="882d2-123">Request body</span></span>
<span data-ttu-id="882d2-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="882d2-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="882d2-125">参数</span><span class="sxs-lookup"><span data-stu-id="882d2-125">Parameter</span></span>      | <span data-ttu-id="882d2-126">类型</span><span class="sxs-lookup"><span data-stu-id="882d2-126">Type</span></span>    |<span data-ttu-id="882d2-127">说明</span><span class="sxs-lookup"><span data-stu-id="882d2-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="882d2-128">提示</span><span class="sxs-lookup"><span data-stu-id="882d2-128">prompts</span></span>|<span data-ttu-id="882d2-129">[mediaPrompt](../resources/mediaprompt.md)集合</span><span class="sxs-lookup"><span data-stu-id="882d2-129">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="882d2-130">录制开始前要播放的提示集合 (如果有)。</span><span class="sxs-lookup"><span data-stu-id="882d2-130">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="882d2-131">客户可以选择单独指定 "playPrompt" 操作, 也可以指定为 "record" 的一部分-通常所有记录都由一个提示 preceeded</span><span class="sxs-lookup"><span data-stu-id="882d2-131">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt</span></span> |
|<span data-ttu-id="882d2-132">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="882d2-132">bargeInAllowed</span></span>|<span data-ttu-id="882d2-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="882d2-133">Boolean</span></span>| <span data-ttu-id="882d2-134">允许用户在提示完成前输入选项。</span><span class="sxs-lookup"><span data-stu-id="882d2-134">Allow users to enter choice before prompt finishes.</span></span>                                                                 |
|<span data-ttu-id="882d2-135">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="882d2-135">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="882d2-136">Int32</span><span class="sxs-lookup"><span data-stu-id="882d2-136">Int32</span></span>| <span data-ttu-id="882d2-137">允许从我们开始记录操作到超时和运行失败的时间开始的最大初始静音。</span><span class="sxs-lookup"><span data-stu-id="882d2-137">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="882d2-138">如果我们正在播放提示, 则此计时器在提示完成后启动。</span><span class="sxs-lookup"><span data-stu-id="882d2-138">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> |
|<span data-ttu-id="882d2-139">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="882d2-139">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="882d2-140">Int32</span><span class="sxs-lookup"><span data-stu-id="882d2-140">Int32</span></span>| <span data-ttu-id="882d2-141">最大无声超时 (秒)。</span><span class="sxs-lookup"><span data-stu-id="882d2-141">The maximum silence timeout in seconds.</span></span>|
|<span data-ttu-id="882d2-142">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="882d2-142">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="882d2-143">Int32</span><span class="sxs-lookup"><span data-stu-id="882d2-143">Int32</span></span>| <span data-ttu-id="882d2-144">以秒为单位的最大记录持续时间。</span><span class="sxs-lookup"><span data-stu-id="882d2-144">The maximum record duration in seconds.</span></span>|
|<span data-ttu-id="882d2-145">playBeep</span><span class="sxs-lookup"><span data-stu-id="882d2-145">playBeep</span></span>|<span data-ttu-id="882d2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="882d2-146">Boolean</span></span>| <span data-ttu-id="882d2-147">播放提示后播放嘟嘟声。</span><span class="sxs-lookup"><span data-stu-id="882d2-147">Plays a beep after playing the prompt.</span></span>|
|<span data-ttu-id="882d2-148">streamWhileRecording</span><span class="sxs-lookup"><span data-stu-id="882d2-148">streamWhileRecording</span></span>|<span data-ttu-id="882d2-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="882d2-149">Boolean</span></span>|<span data-ttu-id="882d2-150">如果设置为 true, 将在录制开始后提供资源位置。</span><span class="sxs-lookup"><span data-stu-id="882d2-150">If set to true, a resource location will be provided as soon as the recording starts.</span></span> |
|<span data-ttu-id="882d2-151">stopTones</span><span class="sxs-lookup"><span data-stu-id="882d2-151">stopTones</span></span>|<span data-ttu-id="882d2-152">String collection</span><span class="sxs-lookup"><span data-stu-id="882d2-152">String collection</span></span>|<span data-ttu-id="882d2-153">指定结束录音的停止音。</span><span class="sxs-lookup"><span data-stu-id="882d2-153">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="882d2-154">适用</span><span class="sxs-lookup"><span data-stu-id="882d2-154">clientContext</span></span>|<span data-ttu-id="882d2-155">String</span><span class="sxs-lookup"><span data-stu-id="882d2-155">String</span></span>|<span data-ttu-id="882d2-156">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="882d2-156">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="882d2-157">响应</span><span class="sxs-lookup"><span data-stu-id="882d2-157">Response</span></span>
<span data-ttu-id="882d2-158">返回`202 Accepted`响应代码和位置标头, 其中包含为此请求创建的[commsOperation](../resources/commsoperation.md)的 uri。</span><span class="sxs-lookup"><span data-stu-id="882d2-158">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="882d2-159">示例</span><span class="sxs-lookup"><span data-stu-id="882d2-159">Example</span></span>
<span data-ttu-id="882d2-160">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="882d2-160">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="882d2-161">请求</span><span class="sxs-lookup"><span data-stu-id="882d2-161">Request</span></span>
<span data-ttu-id="882d2-162">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="882d2-162">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="882d2-163">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="882d2-163">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="882d2-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="882d2-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-record-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="882d2-165">响应</span><span class="sxs-lookup"><span data-stu-id="882d2-165">Response</span></span>

> <span data-ttu-id="882d2-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="882d2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="882d2-168">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="882d2-168">Notification - operation completed</span></span>

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
