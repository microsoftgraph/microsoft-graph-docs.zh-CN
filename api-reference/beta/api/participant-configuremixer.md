---
title: '参与者: configureMixer'
description: 为多方对话中的不同参与者配置音频的混合方式。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cf45c37ba01f32f1d8c494fef76521c20167e8a6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268507"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="78669-103">参与者: configureMixer</span><span class="sxs-lookup"><span data-stu-id="78669-103">participant: configureMixer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78669-104">为多方对话中的不同参与者配置音频的混合方式。</span><span class="sxs-lookup"><span data-stu-id="78669-104">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="78669-105">权限</span><span class="sxs-lookup"><span data-stu-id="78669-105">Permissions</span></span>
<span data-ttu-id="78669-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78669-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="78669-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="78669-108">Permission type</span></span> | <span data-ttu-id="78669-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78669-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="78669-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78669-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="78669-111">不支持</span><span class="sxs-lookup"><span data-stu-id="78669-111">Not Supported</span></span>        |
| <span data-ttu-id="78669-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78669-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78669-113">不支持</span><span class="sxs-lookup"><span data-stu-id="78669-113">Not Supported</span></span>        |
| <span data-ttu-id="78669-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="78669-114">Application</span></span>     | <span data-ttu-id="78669-115">JoinGroupCalls、InitiateGroupCalls 和所有调用</span><span class="sxs-lookup"><span data-stu-id="78669-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="78669-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78669-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /applications/{id}/calls/{id}/participants/configureMixer
```

## <a name="request-headers"></a><span data-ttu-id="78669-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="78669-117">Request headers</span></span>
| <span data-ttu-id="78669-118">名称</span><span class="sxs-lookup"><span data-stu-id="78669-118">Name</span></span>          | <span data-ttu-id="78669-119">说明</span><span class="sxs-lookup"><span data-stu-id="78669-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="78669-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="78669-120">Authorization</span></span> | <span data-ttu-id="78669-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78669-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78669-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="78669-123">Request body</span></span>
<span data-ttu-id="78669-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="78669-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="78669-125">参数</span><span class="sxs-lookup"><span data-stu-id="78669-125">Parameter</span></span>      | <span data-ttu-id="78669-126">类型</span><span class="sxs-lookup"><span data-stu-id="78669-126">Type</span></span>    |<span data-ttu-id="78669-127">说明</span><span class="sxs-lookup"><span data-stu-id="78669-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78669-128">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="78669-128">participantMixerLevels</span></span>|<span data-ttu-id="78669-129">[participantMixerLevel](../resources/participantmixerlevel.md)集合</span><span class="sxs-lookup"><span data-stu-id="78669-129">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="78669-130">指定的音频参与者的混音器级别配置。</span><span class="sxs-lookup"><span data-stu-id="78669-130">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="78669-131">适用</span><span class="sxs-lookup"><span data-stu-id="78669-131">clientContext</span></span>|<span data-ttu-id="78669-132">String</span><span class="sxs-lookup"><span data-stu-id="78669-132">String</span></span>|<span data-ttu-id="78669-133">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="78669-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="78669-134">响应</span><span class="sxs-lookup"><span data-stu-id="78669-134">Response</span></span>
<span data-ttu-id="78669-135">返回`202 Accepted`响应代码和位置标头, 其中包含为此请求创建的[commsOperation](../resources/commsoperation.md)的 uri。</span><span class="sxs-lookup"><span data-stu-id="78669-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="78669-136">示例</span><span class="sxs-lookup"><span data-stu-id="78669-136">Example</span></span>
<span data-ttu-id="78669-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="78669-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="78669-138">请求</span><span class="sxs-lookup"><span data-stu-id="78669-138">Request</span></span>
<span data-ttu-id="78669-139">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="78669-139">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "participant-configureMixer"
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

##### <a name="response"></a><span data-ttu-id="78669-140">响应</span><span class="sxs-lookup"><span data-stu-id="78669-140">Response</span></span>

> <span data-ttu-id="78669-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="78669-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="78669-143">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="78669-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="78669-144">C#</span><span class="sxs-lookup"><span data-stu-id="78669-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/participant-configureMixer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="78669-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="78669-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/participant-configureMixer-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="78669-146">目标-C</span><span class="sxs-lookup"><span data-stu-id="78669-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/participant-configureMixer-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="notification---operation-completed"></a><span data-ttu-id="78669-147">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="78669-147">Notification - operation completed</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "participant: configureMixer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/participant-configuremixer.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/participant-configuremixer.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/participant-configuremixer.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
