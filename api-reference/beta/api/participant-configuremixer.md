---
title: '参与者: configureMixer'
description: 为多方对话中的不同参与者配置音频的混合方式。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0f17d8c14b62e216495560e898801af72c94bb5d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35454032"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="f4300-103">参与者: configureMixer</span><span class="sxs-lookup"><span data-stu-id="f4300-103">participant: configureMixer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4300-104">为多方对话中的不同参与者配置音频的混合方式。</span><span class="sxs-lookup"><span data-stu-id="f4300-104">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4300-105">权限</span><span class="sxs-lookup"><span data-stu-id="f4300-105">Permissions</span></span>
<span data-ttu-id="f4300-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4300-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4300-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4300-108">Permission type</span></span> | <span data-ttu-id="f4300-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4300-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="f4300-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4300-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4300-111">不支持</span><span class="sxs-lookup"><span data-stu-id="f4300-111">Not Supported</span></span>        |
| <span data-ttu-id="f4300-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4300-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4300-113">不支持</span><span class="sxs-lookup"><span data-stu-id="f4300-113">Not Supported</span></span>        |
| <span data-ttu-id="f4300-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4300-114">Application</span></span>     | <span data-ttu-id="f4300-115">JoinGroupCalls、InitiateGroupCalls 和所有调用</span><span class="sxs-lookup"><span data-stu-id="f4300-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4300-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4300-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /applications/{id}/calls/{id}/participants/configureMixer
```

## <a name="request-headers"></a><span data-ttu-id="f4300-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4300-117">Request headers</span></span>
| <span data-ttu-id="f4300-118">名称</span><span class="sxs-lookup"><span data-stu-id="f4300-118">Name</span></span>          | <span data-ttu-id="f4300-119">说明</span><span class="sxs-lookup"><span data-stu-id="f4300-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f4300-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4300-120">Authorization</span></span> | <span data-ttu-id="f4300-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4300-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4300-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4300-123">Request body</span></span>
<span data-ttu-id="f4300-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f4300-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f4300-125">参数</span><span class="sxs-lookup"><span data-stu-id="f4300-125">Parameter</span></span>      | <span data-ttu-id="f4300-126">类型</span><span class="sxs-lookup"><span data-stu-id="f4300-126">Type</span></span>    |<span data-ttu-id="f4300-127">说明</span><span class="sxs-lookup"><span data-stu-id="f4300-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4300-128">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="f4300-128">participantMixerLevels</span></span>|<span data-ttu-id="f4300-129">[participantMixerLevel](../resources/participantmixerlevel.md)集合</span><span class="sxs-lookup"><span data-stu-id="f4300-129">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="f4300-130">指定的音频参与者的混音器级别配置。</span><span class="sxs-lookup"><span data-stu-id="f4300-130">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="f4300-131">适用</span><span class="sxs-lookup"><span data-stu-id="f4300-131">clientContext</span></span>|<span data-ttu-id="f4300-132">String</span><span class="sxs-lookup"><span data-stu-id="f4300-132">String</span></span>|<span data-ttu-id="f4300-133">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="f4300-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="f4300-134">响应</span><span class="sxs-lookup"><span data-stu-id="f4300-134">Response</span></span>
<span data-ttu-id="f4300-135">返回`202 Accepted`响应代码和位置标头, 其中包含为此请求创建的[commsOperation](../resources/commsoperation.md)的 uri。</span><span class="sxs-lookup"><span data-stu-id="f4300-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="f4300-136">示例</span><span class="sxs-lookup"><span data-stu-id="f4300-136">Example</span></span>
<span data-ttu-id="f4300-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="f4300-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f4300-138">请求</span><span class="sxs-lookup"><span data-stu-id="f4300-138">Request</span></span>
<span data-ttu-id="f4300-139">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4300-139">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f4300-140">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f4300-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f4300-141">C#</span><span class="sxs-lookup"><span data-stu-id="f4300-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-configuremixer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4300-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="f4300-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-configuremixer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f4300-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="f4300-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-configuremixer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f4300-144">响应</span><span class="sxs-lookup"><span data-stu-id="f4300-144">Response</span></span>

> <span data-ttu-id="f4300-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f4300-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="f4300-147">通知-操作已完成</span><span class="sxs-lookup"><span data-stu-id="f4300-147">Notification - operation completed</span></span>

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
  ]
}
-->
