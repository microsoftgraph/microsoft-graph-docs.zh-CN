---
title: 参与者： configureMixer
description: 配置如何将音频混合的多方对话中的不同参与者。
author: VinodRavichandran
ms.openlocfilehash: e300d842ce0bad870160d2f3788b059de6d41784
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351987"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="1294a-103">参与者： configureMixer</span><span class="sxs-lookup"><span data-stu-id="1294a-103">participant: configureMixer</span></span>

> <span data-ttu-id="1294a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1294a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1294a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1294a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1294a-106">配置如何将音频混合的多方对话中的不同参与者。</span><span class="sxs-lookup"><span data-stu-id="1294a-106">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="1294a-107">权限</span><span class="sxs-lookup"><span data-stu-id="1294a-107">Permissions</span></span>
<span data-ttu-id="1294a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1294a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1294a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1294a-110">Permission type</span></span> | <span data-ttu-id="1294a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1294a-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="1294a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1294a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1294a-113">不支持</span><span class="sxs-lookup"><span data-stu-id="1294a-113">Not Supported</span></span>        |
| <span data-ttu-id="1294a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1294a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1294a-115">不支持</span><span class="sxs-lookup"><span data-stu-id="1294a-115">Not Supported</span></span>        |
| <span data-ttu-id="1294a-116">Application</span><span class="sxs-lookup"><span data-stu-id="1294a-116">Application</span></span>     | <span data-ttu-id="1294a-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="1294a-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1294a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1294a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /applications/{id}/calls/{id}/participants/configureMixer
```

## <a name="request-headers"></a><span data-ttu-id="1294a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1294a-119">Request headers</span></span>
| <span data-ttu-id="1294a-120">Name</span><span class="sxs-lookup"><span data-stu-id="1294a-120">Name</span></span>          | <span data-ttu-id="1294a-121">说明</span><span class="sxs-lookup"><span data-stu-id="1294a-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1294a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1294a-122">Authorization</span></span> | <span data-ttu-id="1294a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1294a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1294a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1294a-125">Request body</span></span>
<span data-ttu-id="1294a-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1294a-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1294a-127">参数</span><span class="sxs-lookup"><span data-stu-id="1294a-127">Parameter</span></span>      | <span data-ttu-id="1294a-128">Type</span><span class="sxs-lookup"><span data-stu-id="1294a-128">Type</span></span>    |<span data-ttu-id="1294a-129">说明</span><span class="sxs-lookup"><span data-stu-id="1294a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1294a-130">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="1294a-130">participantMixerLevels</span></span>|<span data-ttu-id="1294a-131">[participantMixerLevel](../resources/participantmixerlevel.md)集合</span><span class="sxs-lookup"><span data-stu-id="1294a-131">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="1294a-132">混音器配置为级别给定音频参与者。</span><span class="sxs-lookup"><span data-stu-id="1294a-132">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="1294a-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="1294a-133">clientContext</span></span>|<span data-ttu-id="1294a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="1294a-134">String</span></span>|<span data-ttu-id="1294a-135">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="1294a-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="1294a-136">响应</span><span class="sxs-lookup"><span data-stu-id="1294a-136">Response</span></span>
<span data-ttu-id="1294a-137">返回`202 Accepted`响应代码和具有[commsOperation](../resources/commsoperation.md)创建的此请求 uri 中的位置标头。</span><span class="sxs-lookup"><span data-stu-id="1294a-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="1294a-138">示例</span><span class="sxs-lookup"><span data-stu-id="1294a-138">Example</span></span>
<span data-ttu-id="1294a-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="1294a-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1294a-140">请求</span><span class="sxs-lookup"><span data-stu-id="1294a-140">Request</span></span>
<span data-ttu-id="1294a-141">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="1294a-141">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "participant_configureMixer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/configureMixer
Content-Type: application/json
Content-Length: 501

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "participantMixerLevels": [
    {
      "participant": "550fae72-d251-43ec-868c-373732c2704f",
      "exclusive": true,
      "ducking": {
        "rampActive": 50,
        "rampInactive": 50,
        "lowerLevel": 10,
        "upperLevel": 50
      },
      "sourceLevels": [
        {
          "participant": "632899f8-2ea1-4604-8413-27bd2892079f",
          "level": 50,
          "duckOthers": false
        }
      ]
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="1294a-142">响应</span><span class="sxs-lookup"><span data-stu-id="1294a-142">Response</span></span>

> <span data-ttu-id="1294a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1294a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="1294a-145">通知-完成的操作</span><span class="sxs-lookup"><span data-stu-id="1294a-145">Notification - operation completed</span></span>

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
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"1\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participant: configureMixer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
