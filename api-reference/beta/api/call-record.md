---
title: 呼叫： 记录
description: 录制呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1f119cfece969c01e68773e5985eab4010dc9874
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574857"
---
# <a name="call-record"></a><span data-ttu-id="9739c-103">呼叫： 记录</span><span class="sxs-lookup"><span data-stu-id="9739c-103">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9739c-104">录制呼叫。</span><span class="sxs-lookup"><span data-stu-id="9739c-104">Record the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="9739c-105">权限</span><span class="sxs-lookup"><span data-stu-id="9739c-105">Permissions</span></span>
<span data-ttu-id="9739c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9739c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9739c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9739c-108">Permission type</span></span> | <span data-ttu-id="9739c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9739c-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="9739c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9739c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9739c-111">不支持</span><span class="sxs-lookup"><span data-stu-id="9739c-111">Not Supported</span></span>        |
| <span data-ttu-id="9739c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9739c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9739c-113">不支持</span><span class="sxs-lookup"><span data-stu-id="9739c-113">Not Supported</span></span>        |
| <span data-ttu-id="9739c-114">Application</span><span class="sxs-lookup"><span data-stu-id="9739c-114">Application</span></span>     | <span data-ttu-id="9739c-115">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="9739c-115">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="9739c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9739c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="9739c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9739c-117">Request headers</span></span>
| <span data-ttu-id="9739c-118">名称</span><span class="sxs-lookup"><span data-stu-id="9739c-118">Name</span></span>          | <span data-ttu-id="9739c-119">说明</span><span class="sxs-lookup"><span data-stu-id="9739c-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9739c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9739c-120">Authorization</span></span> | <span data-ttu-id="9739c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9739c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9739c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9739c-123">Request body</span></span>
<span data-ttu-id="9739c-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9739c-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9739c-125">参数</span><span class="sxs-lookup"><span data-stu-id="9739c-125">Parameter</span></span>      | <span data-ttu-id="9739c-126">类型</span><span class="sxs-lookup"><span data-stu-id="9739c-126">Type</span></span>    |<span data-ttu-id="9739c-127">说明</span><span class="sxs-lookup"><span data-stu-id="9739c-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9739c-128">提示</span><span class="sxs-lookup"><span data-stu-id="9739c-128">prompts</span></span>|<span data-ttu-id="9739c-129">[mediaPrompt](../resources/mediaprompt.md)集合</span><span class="sxs-lookup"><span data-stu-id="9739c-129">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="9739c-130">启动提示之前录制播放 （如果有） 的集合。</span><span class="sxs-lookup"><span data-stu-id="9739c-130">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="9739c-131">客户可以选择单独指定"playPrompt"操作，或者指定的"记录"的一部分主要的所有记录都都使用提示</span><span class="sxs-lookup"><span data-stu-id="9739c-131">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt</span></span> |
|<span data-ttu-id="9739c-132">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="9739c-132">bargeInAllowed</span></span>|<span data-ttu-id="9739c-133">布尔值</span><span class="sxs-lookup"><span data-stu-id="9739c-133">Boolean</span></span>| <span data-ttu-id="9739c-134">允许用户提示完成之前输入的选择。</span><span class="sxs-lookup"><span data-stu-id="9739c-134">Allow users to enter choice before prompt finishes.</span></span>                                                                 |
|<span data-ttu-id="9739c-135">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="9739c-135">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="9739c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="9739c-136">Int32</span></span>| <span data-ttu-id="9739c-137">从我们开始之前我们记录操作超时和失败操作的时间允许的最大初始静音。</span><span class="sxs-lookup"><span data-stu-id="9739c-137">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="9739c-138">如果我们播放提示时，提示完成后从开始此计时器。</span><span class="sxs-lookup"><span data-stu-id="9739c-138">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> |
|<span data-ttu-id="9739c-139">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="9739c-139">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="9739c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9739c-140">Int32</span></span>| <span data-ttu-id="9739c-141">最大无声超时秒数。</span><span class="sxs-lookup"><span data-stu-id="9739c-141">The maximum silence timeout in seconds.</span></span>|
|<span data-ttu-id="9739c-142">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="9739c-142">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="9739c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9739c-143">Int32</span></span>| <span data-ttu-id="9739c-144">最大记录持续时间，以秒为单位。</span><span class="sxs-lookup"><span data-stu-id="9739c-144">The maximum record duration in seconds.</span></span>|
|<span data-ttu-id="9739c-145">playBeep</span><span class="sxs-lookup"><span data-stu-id="9739c-145">playBeep</span></span>|<span data-ttu-id="9739c-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="9739c-146">Boolean</span></span>| <span data-ttu-id="9739c-147">播放提示音后播放提示。</span><span class="sxs-lookup"><span data-stu-id="9739c-147">Plays a beep after playing the prompt.</span></span>|
|<span data-ttu-id="9739c-148">streamWhileRecording</span><span class="sxs-lookup"><span data-stu-id="9739c-148">streamWhileRecording</span></span>|<span data-ttu-id="9739c-149">布尔值</span><span class="sxs-lookup"><span data-stu-id="9739c-149">Boolean</span></span>|<span data-ttu-id="9739c-150">如果设置为 true，资源位置将提供一旦开始录制。</span><span class="sxs-lookup"><span data-stu-id="9739c-150">If set to true, a resource location will be provided as soon as the recording starts.</span></span> |
|<span data-ttu-id="9739c-151">stopTones</span><span class="sxs-lookup"><span data-stu-id="9739c-151">stopTones</span></span>|<span data-ttu-id="9739c-152">String 集合</span><span class="sxs-lookup"><span data-stu-id="9739c-152">String collection</span></span>|<span data-ttu-id="9739c-153">停止指定结束录制音。</span><span class="sxs-lookup"><span data-stu-id="9739c-153">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="9739c-154">clientContext</span><span class="sxs-lookup"><span data-stu-id="9739c-154">clientContext</span></span>|<span data-ttu-id="9739c-155">String</span><span class="sxs-lookup"><span data-stu-id="9739c-155">String</span></span>|<span data-ttu-id="9739c-156">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="9739c-156">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="9739c-157">响应</span><span class="sxs-lookup"><span data-stu-id="9739c-157">Response</span></span>
<span data-ttu-id="9739c-158">返回`202 Accepted`响应代码和具有[commsOperation](../resources/commsoperation.md)创建的此请求 uri 中的位置标头。</span><span class="sxs-lookup"><span data-stu-id="9739c-158">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="9739c-159">示例</span><span class="sxs-lookup"><span data-stu-id="9739c-159">Example</span></span>
<span data-ttu-id="9739c-160">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="9739c-160">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9739c-161">请求</span><span class="sxs-lookup"><span data-stu-id="9739c-161">Request</span></span>
<span data-ttu-id="9739c-162">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="9739c-162">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="9739c-163">响应</span><span class="sxs-lookup"><span data-stu-id="9739c-163">Response</span></span>

> <span data-ttu-id="9739c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9739c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="9739c-166">通知-完成的操作</span><span class="sxs-lookup"><span data-stu-id="9739c-166">Notification - operation completed</span></span>

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
    "Error: /api-reference/beta/api/call-record.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
